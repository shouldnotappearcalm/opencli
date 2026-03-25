---
name: opencli-platform-router
description: Route social/content requests to OpenCLI by platform command docs. Use when user asks to browse trending, search content, fetch feeds, check bookmarks/history, or run platform commands on supported sites.
---

Use this skill as command router.

1. Detect platform from user request.
2. Load `references/commands/<platform>.md`.
3. Choose the exact command and fill required args.
4. Prefer `-f json` for parseable output.
5. If platform/command is unclear, ask one minimal clarification or run `opencli list` / `opencli <site> --help`.

Workflow docs (load on demand):
- `references/workflows/daily-brief.md`
- `references/workflows/content-post.md`

All platform command docs live in:
- `references/commands/*.md`
