# v2ex

Total commands: **11**

## Commands


### daily
- Description: V2EX 每日签到并领取铜币
- Args: none declared
- Example: `opencli v2ex daily -f json`

### hot
- Description: V2EX 热门话题
- Args:
  - `limit` (optional) — type=int; default=20; Number of topics
- Example: `opencli v2ex hot -f json`

### latest
- Description: V2EX 最新话题
- Args:
  - `limit` (optional) — type=int; default=20; Number of topics
- Example: `opencli v2ex latest -f json`

### me
- Description: V2EX 获取个人资料 (余额/未读提醒)
- Args: none declared
- Example: `opencli v2ex me -f json`

### member
- Description: V2EX 用户资料
- Args:
  - `username` (required) — type=str; Username
- Example: `opencli v2ex member -f json`

### node
- Description: V2EX 节点话题列表
- Args:
  - `name` (required) — type=str; Node name (e.g. python, javascript, apple)
  - `limit` (optional) — type=int; default=10; Number of topics (API returns max 20)
- Example: `opencli v2ex node -f json`

### nodes
- Description: V2EX 所有节点列表
- Args:
  - `limit` (optional) — type=int; default=30; Number of nodes
- Example: `opencli v2ex nodes -f json`

### notifications
- Description: V2EX 获取提醒 (回复/由于)
- Args:
  - `limit` (optional) — type=int; default=20; Number of notifications
- Example: `opencli v2ex notifications -f json`

### replies
- Description: V2EX 主题回复列表
- Args:
  - `id` (required) — type=str; Topic ID
  - `limit` (optional) — type=int; default=20; Number of replies
- Example: `opencli v2ex replies -f json`

### topic
- Description: V2EX 主题详情和回复
- Args:
  - `id` (required) — type=str; Topic ID
- Example: `opencli v2ex topic -f json`

### user
- Description: V2EX 用户发帖列表
- Args:
  - `username` (required) — type=str; Username
  - `limit` (optional) — type=int; default=10; Number of topics (API returns max 20)
- Example: `opencli v2ex user -f json`
