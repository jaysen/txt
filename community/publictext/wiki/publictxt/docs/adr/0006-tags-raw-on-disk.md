---
mirror_remote: publictext
mirror_repo: https://github.com/publictxt/publictext
mirror_path: wiki/publictxt/docs/adr/0006-tags-raw-on-disk.md
mirror_branch: main
mirror_commit: 4a7bca560ddc5e103536577b04cb9780b24ec70a
mirror_blob: 4b6dcd62ee98a0b928087c6146a69be069117f0e
mirror_date: 2026-11-25T23:46:06+02:00
---
# 0006. Tags stay raw on disk; normalization and aliases happen at view time

- **Status:** Accepted
- **Date:** 2026-10-13, recording an earlier decision

## Context

- Authors tag freely: `DotNet`, `dotnet`, `dot-net`.
- A reader can't rewrite other people's repos. Rewriting your own tags into a normalized form destroys what you wrote.
- A global vocabulary needs a central authority, which the project rules out.

## Decision

- Tags are stored as written (`raw`).
- The comparison form (`match`) is computed when reading and never written back.
- Each reader keeps a personal alias file mapping variants to the tag they prefer. Views apply it; stored data never changes.

## Consequences

- + No write-time churn, and the author's intent is preserved.
- + Each reader controls their own vocabulary.
- − Every implementation must compute `match` identically. Spec §7.3 and fixture 002 enforce this.
- − Alias files don't spread by themselves. Sharing them could later work like following a repo.
