---
name: opencli-platform-router
description: Route requests to OpenCLI command docs for supported platforms: antigravity, apple-podcasts, arxiv, barchart, bbc, bilibili, bloomberg, boss, chaoxing, chatgpt, chatwise, codex, coupang, ctrip, cursor, devto, discord-app, douban, doubao-app, doubao, facebook, google, grok, hackernews, hf, instagram, jike, jimeng, linux-do, lobsters, medium, notion, reddit, reuters, sinablog, sinafinance, smzdm, stackoverflow, steam, substack, tiktok, twitter, v2ex, weibo, weixin, weread, wikipedia, xiaohongshu, xiaoyuzhou, xueqiu, yahoo-finance, yollomi, youtube, zhihu. Supports command usage guidance for common actions including hot/trending, search, timeline/feed, profile, notifications, bookmarks/history, download/export, and interactive actions such as post/reply/like/follow/bookmark/delete/check-in where available. Use when users ask how to run commands, what args are required, and what parameters mean for a platform command.
---

Use this skill as a platform command router.

Prerequisites and bootstrap:

- Ensure `opencli` is available. If missing, install:
  - `npm install -g @jackwener/opencli`
  - verify: `opencli --version`
- Before first real command, run:
  - `opencli doctor`
- If doctor reports extension/browser connectivity issue, prompt user to install Chrome Browser Bridge extension manually:
  1. Open `chrome://extensions`
  2. Enable Developer mode
  3. Click "Load unpacked"
  4. Select the `extension/` directory from the OpenCLI repo (or install release zip from OpenCLI releases)
  5. Keep Chrome open and logged in, then rerun `opencli doctor`

1. Detect target platform from user request.
2. Load `references/commands/<platform>.md`.
3. Select the command and fill required args.
4. Prefer `-f json` for parseable output.
5. If platform/command is unclear, ask one minimal clarification or run `opencli list` / `opencli <site> --help`.

All command docs live in:
- `references/commands/*.md`

Setup and manual extension install guide:
- `README.md`
