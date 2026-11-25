---
mirror_remote: publictext
mirror_repo: https://github.com/publictxt/publictext
mirror_path: wiki/publictxt/docs/adr/0009-single-author-per-repo.md
mirror_branch: main
mirror_commit: 4a7bca560ddc5e103536577b04cb9780b24ec70a
mirror_blob: 6365297426003ece89ef48b40612844681d42ac6
mirror_date: 2026-11-25T23:46:06+02:00
---
# 0009. One author per repository

- **Status:** Accepted
- **Date:** 2026-10-13, recording an earlier decision (CuratedCommons storage revision)

## Context

The earlier storage model used one file per (author, resource, tag) assertion so that many authors could share a repo. It was complex and fought Git's merge model.

## Decision

- Each repository has exactly one author. A repository is an identity.
- Multi-author views come from aggregating repositories.
- Contributing to someone else's repo is an ordinary pull request, and the owner stays the author.

## Consequences

- + No authorship conflicts inside a repo; Git handles any merge.
- + Per-file author fields are unnecessary because the manifest states the author once (spec §5 open question).
- − Group and community repos will need their own model later (`community/`, see IDEAS.md).
