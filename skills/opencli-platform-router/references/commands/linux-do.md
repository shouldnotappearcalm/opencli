# linux-do

Total commands: **6**

## Commands


### categories
- Description: linux.do 分类列表
- Args:
  - `limit` (optional) — type=int; default=20; Number of categories
- Example: `opencli linux-do categories -f json`

### category
- Description: linux.do 分类内话题
- Args:
  - `slug` (required) — type=str; Category slug (use 'categories' command to find)
  - `id` (required) — type=int; Category ID (use 'categories' command to find)
  - `limit` (optional) — type=int; default=20; Number of topics
- Example: `opencli linux-do category -f json`

### hot
- Description: linux.do 热门话题
- Args:
  - `limit` (optional) — type=int; default=20; Number of topics
  - `period` (optional) — type=str; default=weekly; Time period
- Example: `opencli linux-do hot -f json`

### latest
- Description: linux.do 最新话题
- Args:
  - `limit` (optional) — type=int; default=20; Number of topics
- Example: `opencli linux-do latest -f json`

### search
- Description: 搜索 linux.do
- Args:
  - `query` (required) — type=str; Search query
  - `limit` (optional) — type=int; default=20; Number of results
- Example: `opencli linux-do search -f json`

### topic
- Description: linux.do 帖子详情和回复（首页）
- Args:
  - `id` (required) — type=int; Topic ID
- Example: `opencli linux-do topic -f json`
