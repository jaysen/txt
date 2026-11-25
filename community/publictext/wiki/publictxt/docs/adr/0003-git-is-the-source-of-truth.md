---
mirror_remote: publictext
mirror_repo: https://github.com/publictxt/publictext
mirror_path: wiki/publictxt/docs/adr/0003-git-is-the-source-of-truth.md
mirror_branch: main
mirror_commit: 4a7bca560ddc5e103536577b04cb9780b24ec70a
mirror_blob: 66ed078d5a036b0f865c4a3eb2e7b5ecbffe35e8
mirror_date: 2026-11-25T23:46:06+02:00
---
# 0003. Git is the only source of truth; derived data is never committed

- **Status:** Proposed
- **Date:** 2026-10-13

## Context

- The README layout commits `indexes/` and `tags/` folders.
- Generated files in Git go stale, conflict on merges and add noise to every diff.
- The project already prefers view-time reconciliation to write-time normalization (ADR-0006). Committed indexes contradict that.

## Decision

- A repository holds authored content and the manifest only.
- Databases, indexes, tag pages and search data are projections. Each is keyed by commit SHA and can be deleted and rebuilt at any time.
- Projections update incrementally from `git diff --name-only <old>..<new>`.

## Consequences

- + No merge conflicts on generated files, and nothing on disk can drift out of sync.
- + The local database is a cache, so "delete it and resync" is always safe.
- − Every consumer computes its own projections. This is cheap at the expected scale of text repos with thousands of files.
- ! Known conflict: `resource_id` in front matter is derived from the `bookmark` URL. A change to URL normalization would make every stored value stale. Spec §8 lists the options; resolve this before 0.1 is final.
- ! The same question applies to `author` and `source_repo` in front matter (spec §5).
- + Authored provenance is not derived data. Fork provenance (`fork_*`, ADR-0012) records a choice at a point in time and can't be recomputed, so it belongs on disk.
