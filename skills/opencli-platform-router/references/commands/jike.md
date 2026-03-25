# jike

Total commands: **10**

## Commands


### comment
- Description: 评论即刻帖子
- Args:
  - `id` (required) — type=string; 帖子 ID
  - `text` (required) — type=string; 评论内容
- Example: `opencli jike comment -f json`

### create
- Description: 发布即刻动态
- Args:
  - `text` (required) — type=string; 动态正文内容
- Example: `opencli jike create -f json`

### feed
- Description: 即刻首页动态流
- Args:
  - `limit` (optional) — type=int; default=20
- Example: `opencli jike feed -f json`

### like
- Description: 点赞即刻帖子
- Args:
  - `id` (required) — type=string; 帖子 ID
- Example: `opencli jike like -f json`

### notifications
- Description: 即刻通知
- Args:
  - `limit` (optional) — type=int; default=20
- Example: `opencli jike notifications -f json`

### post
- Description: 即刻帖子详情及评论
- Args:
  - `id` (required) — type=string; Post ID (from post URL)
- Example: `opencli jike post -f json`

### repost
- Description: 转发即刻帖子
- Args:
  - `id` (required) — type=string; 帖子 ID
  - `text` (optional) — type=string; 转发附言（可选）
- Example: `opencli jike repost -f json`

### search
- Description: 搜索即刻帖子
- Args:
  - `query` (required) — type=string
  - `limit` (optional) — type=int; default=20
- Example: `opencli jike search -f json`

### topic
- Description: 即刻话题/圈子帖子
- Args:
  - `id` (required) — type=string; Topic ID (from topic URL, e.g. 553870e8e4b0cafb0a1bef68)
  - `limit` (optional) — type=int; default=20; Number of posts
- Example: `opencli jike topic -f json`

### user
- Description: 即刻用户动态
- Args:
  - `username` (required) — type=string; Username from profile URL (e.g. wenhao1996)
  - `limit` (optional) — type=int; default=20; Number of posts
- Example: `opencli jike user -f json`
