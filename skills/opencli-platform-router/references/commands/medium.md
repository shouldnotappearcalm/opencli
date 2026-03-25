# medium

Total commands: **3**

## Commands


### feed
- Description: Medium 热门文章 Feed
- Args:
  - `topic` (optional) — default=''; 话题标签（如 technology, programming, ai）
  - `limit` (optional) — type=int; default=20; 返回的文章数量
- Example: `opencli medium feed -f json`

### search
- Description: 搜索 Medium 文章
- Args:
  - `keyword` (required) — 搜索关键词
  - `limit` (optional) — type=int; default=20; 返回的文章数量
- Example: `opencli medium search -f json`

### user
- Description: 获取 Medium 用户的文章列表
- Args:
  - `username` (required) — Medium 用户名（如 @username 或 username）
  - `limit` (optional) — type=int; default=20; 返回的文章数量
- Example: `opencli medium user -f json`
