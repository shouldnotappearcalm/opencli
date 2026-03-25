# xiaohongshu

Total commands: **11**

## Commands


### creator-note-detail
- Description: 小红书单篇笔记详情页数据 (笔记信息 + 核心/互动数据 + 观看来源 + 观众画像 + 趋势数据)
- Args:
  - `note-id` (required) — type=string; Note ID (from creator-notes or note-detail page URL)
- Example: `opencli xiaohongshu creator-note-detail -f json`

### creator-notes
- Description: 小红书创作者笔记列表 + 每篇数据 (标题/日期/观看/点赞/收藏/评论)
- Args:
  - `limit` (optional) — type=int; default=20; Number of notes to return
- Example: `opencli xiaohongshu creator-notes -f json`

### creator-notes-summary
- Description: 小红书最近笔记批量摘要 (列表 + 单篇关键数据汇总)
- Args:
  - `limit` (optional) — type=int; default=3; Number of recent notes to summarize
- Example: `opencli xiaohongshu creator-notes-summary -f json`

### creator-profile
- Description: 小红书创作者账号信息 (粉丝/关注/获赞/成长等级)
- Args: none declared
- Example: `opencli xiaohongshu creator-profile -f json`

### creator-stats
- Description: 小红书创作者数据总览 (观看/点赞/收藏/评论/分享/涨粉，含每日趋势)
- Args:
  - `period` (optional) — type=string; default='seven'; Stats period: seven or thirty
- Example: `opencli xiaohongshu creator-stats -f json`

### download
- Description: 下载小红书笔记中的图片和视频
- Args:
  - `note-id` (required) — Note ID (from URL)
  - `output` (optional) — default='./xiaohongshu-downloads'; Output directory
- Example: `opencli xiaohongshu download -f json`

### feed
- Description: 小红书首页推荐 Feed (via Pinia Store Action)
- Args:
  - `limit` (optional) — type=int; default=20; Number of items to return
- Example: `opencli xiaohongshu feed -f json`

### notifications
- Description: 小红书通知 (mentions/likes/connections)
- Args:
  - `type` (optional) — type=str; default=mentions; "Notification type: mentions, likes, or connections"
  - `limit` (optional) — type=int; default=20; Number of notifications to return
- Example: `opencli xiaohongshu notifications -f json`

### publish
- Description: 小红书发布图文笔记 (creator center UI automation)
- Args:
  - `title` (required) — 笔记标题 (最多20字)
  - `content` (required) — 笔记正文
  - `images` (optional) — 图片路径，逗号分隔，最多9张 (jpg/png/gif/webp)
  - `topics` (optional) — 话题标签，逗号分隔，不含 # 号
  - `draft` (optional) — type=bool; default=false; 保存为草稿，不直接发布
- Example: `opencli xiaohongshu publish -f json`

### search
- Description: 搜索小红书笔记
- Args:
  - `query` (required) — Search keyword
  - `limit` (optional) — type=int; default=20; Number of results
- Example: `opencli xiaohongshu search -f json`

### user
- Description: Get public notes from a Xiaohongshu user profile
- Args:
  - `id` (required) — type=string; User id or profile URL
  - `limit` (optional) — type=int; default=15; Number of notes to return
- Example: `opencli xiaohongshu user -f json`
