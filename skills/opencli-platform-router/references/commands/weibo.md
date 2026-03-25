# weibo

Total commands: **2**

## Commands


### hot
- Description: 微博热搜
- Args:
  - `limit` (optional) — type=int; default=30; Number of items (max 50)
- Example: `opencli weibo hot -f json`

### search
- Description: 搜索微博
- Args:
  - `keyword` (required) — Search keyword
  - `limit` (optional) — type=int; default=10; Number of results (max 50)
- Example: `opencli weibo search -f json`
