# tiktok

Total commands: **15**

## Commands


### comment
- Description: Comment on a TikTok video
- Args:
  - `url` (required) — type=str; TikTok video URL
  - `text` (required) — type=str; Comment text
- Example: `opencli tiktok comment -f json`

### explore
- Description: Get trending TikTok videos from explore page
- Args:
  - `limit` (optional) — type=int; default=20; Number of videos
- Example: `opencli tiktok explore -f json`

### follow
- Description: Follow a TikTok user
- Args:
  - `username` (required) — type=str; TikTok username (without @)
- Example: `opencli tiktok follow -f json`

### following
- Description: List accounts you follow on TikTok
- Args:
  - `limit` (optional) — type=int; default=20; Number of accounts
- Example: `opencli tiktok following -f json`

### friends
- Description: Get TikTok friend suggestions
- Args:
  - `limit` (optional) — type=int; default=20; Number of suggestions
- Example: `opencli tiktok friends -f json`

### like
- Description: Like a TikTok video
- Args:
  - `url` (required) — type=str; TikTok video URL
- Example: `opencli tiktok like -f json`

### live
- Description: Browse live streams on TikTok
- Args:
  - `limit` (optional) — type=int; default=10; Number of streams
- Example: `opencli tiktok live -f json`

### notifications
- Description: Get TikTok notifications (likes, comments, mentions, followers)
- Args:
  - `limit` (optional) — type=int; default=15; Number of notifications
  - `type` (optional) — type=str; default=all; Notification type
- Example: `opencli tiktok notifications -f json`

### profile
- Description: Get TikTok user profile info
- Args:
  - `username` (required) — type=str; TikTok username (without @)
- Example: `opencli tiktok profile -f json`

### save
- Description: Add a TikTok video to Favorites
- Args:
  - `url` (required) — type=str; TikTok video URL
- Example: `opencli tiktok save -f json`

### search
- Description: Search TikTok videos
- Args:
  - `query` (required) — type=str; Search query
  - `limit` (optional) — type=int; default=10; Number of results
- Example: `opencli tiktok search -f json`

### unfollow
- Description: Unfollow a TikTok user
- Args:
  - `username` (required) — type=str; TikTok username (without @)
- Example: `opencli tiktok unfollow -f json`

### unlike
- Description: Unlike a TikTok video
- Args:
  - `url` (required) — type=str; TikTok video URL
- Example: `opencli tiktok unlike -f json`

### unsave
- Description: Remove a TikTok video from Favorites
- Args:
  - `url` (required) — type=str; TikTok video URL
- Example: `opencli tiktok unsave -f json`

### user
- Description: Get recent videos from a TikTok user
- Args:
  - `username` (required) — type=str; TikTok username (without @)
  - `limit` (optional) — type=int; default=10; Number of videos
- Example: `opencli tiktok user -f json`
