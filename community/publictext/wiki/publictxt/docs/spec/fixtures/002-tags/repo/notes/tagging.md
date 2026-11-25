---
tags:
  - PublicTxt
  - "#Obsidian"
mirror_remote: publictext
mirror_repo: https://github.com/publictxt/publictext
mirror_path: wiki/publictxt/docs/spec/fixtures/002-tags/repo/notes/tagging.md
mirror_branch: main
mirror_commit: 4a7bca560ddc5e103536577b04cb9780b24ec70a
mirror_blob: f995872882d05060e1a25dccc9eead3e8078b222
mirror_date: 2026-11-25T23:46:07+02:00
---
# Tag edge cases

Inline #dotnet and #DotNet (duplicate by match) and #publictxt (duplicate of front matter).
Nested #lang/csharp works. Unicode #café works. Underscores #snake_case work.
Numeric #2026 is not a tag. Neither is a#b mid-word.

## Not a tag

A URL fragment https://example.com/page#section is not a tag.

`#inline-code` is ignored.

```
#fenced is ignored
```

Trailing punctuation is dropped: #end.
