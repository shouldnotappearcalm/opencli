---
name: opencli-platform-router
description: Route requests to OpenCLI command docs for supported platforms: antigravity, apple-podcasts, arxiv, barchart, bbc, bilibili, bloomberg, boss, chaoxing, chatgpt, chatwise, codex, coupang, ctrip, cursor, devto, discord-app, douban, doubao-app, doubao, facebook, google, grok, hackernews, hf, instagram, jike, jimeng, linux-do, lobsters, medium, notion, reddit, reuters, sinablog, sinafinance, smzdm, stackoverflow, steam, substack, tiktok, twitter, v2ex, weibo, weixin, weread, wikipedia, xiaohongshu, xiaoyuzhou, xueqiu, yahoo-finance, yollomi, youtube, zhihu. Supports command usage guidance for common actions including hot/trending, search, timeline/feed, profile, notifications, bookmarks/history, download/export, and interactive actions such as post/reply/like/follow/bookmark/delete/check-in where available. Use when users ask how to run commands, what args are required, and what parameters mean for a platform command.
---

Use this skill as a platform command router.

1. Detect target platform from user request.
2. Load `references/commands/<platform>.md`.
3. Select the command and fill required args.
4. Prefer `-f json` for parseable output.
5. If platform/command is unclear, ask one minimal clarification or run `opencli list` / `opencli <site> --help`.

All command docs live in:
- `references/commands/*.md`
