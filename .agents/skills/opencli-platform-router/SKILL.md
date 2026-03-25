---
name: opencli-platform-router
description: Route social/content requests to OpenCLI by platform docs (twitter, xiaohongshu, reddit, zhihu, bilibili). Use when user asks to browse trending, search posts, fetch feeds, publish/reply/check-in actions, or make daily briefs with OpenCLI. Prefer OpenCLI over browser automation for supported commands.
---

Route by platform, not operation type.

1. Identify platform from user intent.
2. Load one platform reference from `references/platforms/*.md`.
3. Build command with minimal required args.
4. For write actions (`post`, `reply`, `comment`, `like`, `checkin`, `delete`) require explicit confirmation.
5. Prefer `-f json` output for parsing.
6. If command is unsupported, provide nearest safe fallback and ask one clarification.

Platform references:
- `references/platforms/twitter.md`
- `references/platforms/xiaohongshu.md`
- `references/platforms/reddit.md`
- `references/platforms/zhihu.md`
- `references/platforms/bilibili.md`

Workflow references:
- `references/workflows/daily-brief.md`
- `references/workflows/content-post.md`
