# substack

Total commands: **3**

## Commands


### feed
- Description: Substack 热门文章 Feed
- Args:
  - `category` (optional) — default='all'; 文章分类: all, tech, business, culture, politics, science, health
  - `limit` (optional) — type=int; default=20; 返回的文章数量
- Example: `opencli substack feed -f json`

### publication
- Description: 获取特定 Substack Newsletter 的最新文章
- Args:
  - `url` (required) — Newsletter URL（如 https://example.substack.com）
  - `limit` (optional) — type=int; default=20; 返回的文章数量
- Example: `opencli substack publication -f json`

### search
- Description: 搜索 Substack 文章和 Newsletter
- Args:
  - `keyword` (required) — 搜索关键词
  - `type` (optional) — default='posts'; 搜索类型（posts=文章, publications=Newsletter）
  - `limit` (optional) — type=int; default=20; 返回结果数量
- Example: `opencli substack search -f json`
