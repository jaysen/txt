---
bookmark: https://github.com/publictxt/publictxt-pages
tags:
  - publictxt
  - publictxt-pages
  - docs
mirror_remote: publictext
mirror_repo: https://github.com/publictxt/publictext
mirror_path: wiki/publictxt/projects/publictxt-pages/PublicTxt-Pages.md
mirror_branch: main
mirror_commit: 4a7bca560ddc5e103536577b04cb9780b24ec70a
mirror_blob: 9a8e70ad32f4b04d8a6ba0a55044bb9564225668
mirror_date: 2026-11-25T23:46:09+02:00
---
# PublicTxt-Pages

A zero-backend static site for browsing and searching a PublicTxt repository, or any Obsidian / Markdown vault. Formerly Txt-Hugo. This site is built with it — see [Publishing](Publishing.md).

## What it does

- **Static and free to host** — Hugo build, deployed to GitHub Pages or any static host. No server, no hosted search.
- **Works on plain Obsidian vaults** — relative Markdown links build as a working site with no conversion step.
- **Full-text search and facets** — [Pagefind](https://pagefind.app/) search; filter lists and results by collection and tags, including combinations, with include / exclude chips. Pages from repos you follow filter by source, source rating and copy (forked or mirrored).
- **Hashtags** — inline `#hashtags` merge with front matter `tags`; nested tags (`dev/web`) too.
- **Collections** — top-level folders (wiki, blog, posts, notes, bookmarks) plus `collections:` and `bookmark:` front matter. See [Repository structure](../../Repository-Structure.md).
- **Dates from the path and Git** — `created` / `updated` derived, no front matter needed.
- **Navigation** — sections, tag cloud, folder trees for the wiki, timelines for the blog.

## How

- Python pre-processing (no dependencies): content sync, titles, dates, hashtags
- Hugo templates; browse lists and facets in plain ES modules, bundled by Hugo
- Pagefind for search

## Documentation

In the [repository](https://github.com/publictxt/publictxt-pages)'s `docs/`. Its pages are also mirrored here under `community/publictxt-pages/`.

| For | Read |
|---|---|
| Publishing a repo | [User guide](https://github.com/publictxt/publictxt-pages/blob/main/docs/user/README.md): [setup](https://github.com/publictxt/publictxt-pages/blob/main/docs/user/setup.md), [configuration](https://github.com/publictxt/publictxt-pages/blob/main/docs/user/configuration.md) (`settings/site.toml`), [writing](https://github.com/publictxt/publictxt-pages/blob/main/docs/user/writing.md) (folders, front matter, tags, links), [the published site](https://github.com/publictxt/publictxt-pages/blob/main/docs/user/site.md), [other editors](https://github.com/publictxt/publictxt-pages/blob/main/docs/user/other-editors.md) |
| What it does, and what's not built | [SPEC.md](https://github.com/publictxt/publictxt-pages/blob/main/docs/SPEC.md) |
| Working on the code | [Map](https://github.com/publictxt/publictxt-pages/blob/main/docs/wiki/index.md) of scripts, templates and tests; [traps](https://github.com/publictxt/publictxt-pages/blob/main/docs/wiki/traps.md) |
| Planned changes | [plans/](https://github.com/publictxt/publictxt-pages/tree/main/docs/plans) |

This repository's own setup: [Publishing](Publishing.md).

## Planned

- **`[[wikilinks]]` at sync**: rewrite each wikilink as a relative Markdown link, resolved as Obsidian does (shortest unique path), with a never-published report of dangling and ambiguous links. Planned in slices; on hold until a repo in hand needs it. [Plan](https://github.com/publictxt/publictxt-pages/blob/main/docs/plans/wikilinks.md).
- **Folder pages by any name**: let a folder's page have a real name, converted to Hugo's `_index.md` at sync, so it reads well in Obsidian and in other people's mirrors. Pages reads only `_index.md` for now.
- **Subscribe to tags by RSS**.
- **Sort by author or source**.
- From SPEC.md's list: backlinks, related pages by tag co-occurrence, category pages, `author` and `source_repo` filters once there is multi-author content. Multi-repo fan-in is left to PublicTxt's aggregation, not the site.

## Issues
see [PublicTxt-Pages Issues](PublicTxt-Pages%20Issues.md)


Upstream list: [docs/wiki/issues.md](https://github.com/publictxt/publictxt-pages/blob/main/docs/wiki/issues.md).

## Links

- [Repository](https://github.com/publictxt/publictxt-pages)
- Live: this site, [publictxt.github.io/publictext](https://publictxt.github.io/publictext/)
