---
mirror_remote: publictext
mirror_repo: https://github.com/publictxt/publictext
mirror_path: wiki/publictxt/docs/adr/0005-follow-repos-filter-at-query-time.md
mirror_branch: main
mirror_commit: 4a7bca560ddc5e103536577b04cb9780b24ec70a
mirror_blob: 37023cdb04af004033e4dbb13a324292c9776493
mirror_date: 2026-11-25T23:46:06+02:00
---
# 0005. Follow whole repos and filter at query time; no topic branches

- **Status:** Accepted (subscription model). Proposed (removing topic branches).
- **Date:** 2026-10-13, recording an earlier decision

## Context

- del.icio.us offered per-tag subscriptions cheaply because it was centralized. In a Git model, fetching per tag (for example, sparse checkout per tag) is expensive and fragile.
- The README proposes topic branches with shared naming standards, so readers can follow one aspect of a repo. Branches diverge, the author has to keep merging them, and every author has to agree on branch names.

## Decision

- Readers follow whole repositories, listed under `follows` in their manifest. Superseded by ADR-0014: one note per follow in `follows/`.
- Filtering happens at query time, through saved filters.
- Published content lives on the default branch. Other branches are for drafts and pull requests.

## Consequences

- + One fetch per followed repo, and no coordination between authors on branch names.
- + The follow list is plaintext, so the social graph is public text too.
- − Readers fetch more than they read. That's fine for text. Repos with large media need guidance, such as partial clone (`--filter=blob:none`) or LFS.
- − The `follows` filter grammar is still open (spec §13).
