# instagram

Total commands: **14**

## Commands


### comment
- Description: Comment on an Instagram post
- Args:
  - `username` (required) — type=str; Username of the post author
  - `text` (required) — type=str; Comment text
  - `index` (optional) — type=int; default=1; Post index (1 = most recent)
- Example: `opencli instagram comment -f json`

### explore
- Description: Instagram explore/discover trending posts
- Args:
  - `limit` (optional) — type=int; default=20; Number of posts
- Example: `opencli instagram explore -f json`

### follow
- Description: Follow an Instagram user
- Args:
  - `username` (required) — type=str; Instagram username to follow
- Example: `opencli instagram follow -f json`

### followers
- Description: List followers of an Instagram user
- Args:
  - `username` (required) — type=str; Instagram username
  - `limit` (optional) — type=int; default=20; Number of followers
- Example: `opencli instagram followers -f json`

### following
- Description: List accounts an Instagram user is following
- Args:
  - `username` (required) — type=str; Instagram username
  - `limit` (optional) — type=int; default=20; Number of accounts
- Example: `opencli instagram following -f json`

### like
- Description: Like an Instagram post
- Args:
  - `username` (required) — type=str; Username of the post author
  - `index` (optional) — type=int; default=1; Post index (1 = most recent)
- Example: `opencli instagram like -f json`

### profile
- Description: Get Instagram user profile info
- Args:
  - `username` (required) — type=str; Instagram username
- Example: `opencli instagram profile -f json`

### save
- Description: Save (bookmark) an Instagram post
- Args:
  - `username` (required) — type=str; Username of the post author
  - `index` (optional) — type=int; default=1; Post index (1 = most recent)
- Example: `opencli instagram save -f json`

### saved
- Description: Get your saved Instagram posts
- Args:
  - `limit` (optional) — type=int; default=20; Number of saved posts
- Example: `opencli instagram saved -f json`

### search
- Description: Search Instagram users
- Args:
  - `query` (required) — type=str; Search query
  - `limit` (optional) — type=int; default=10; Number of results
- Example: `opencli instagram search -f json`

### unfollow
- Description: Unfollow an Instagram user
- Args:
  - `username` (required) — type=str; Instagram username to unfollow
- Example: `opencli instagram unfollow -f json`

### unlike
- Description: Unlike an Instagram post
- Args:
  - `username` (required) — type=str; Username of the post author
  - `index` (optional) — type=int; default=1; Post index (1 = most recent)
- Example: `opencli instagram unlike -f json`

### unsave
- Description: Unsave (remove bookmark) an Instagram post
- Args:
  - `username` (required) — type=str; Username of the post author
  - `index` (optional) — type=int; default=1; Post index (1 = most recent)
- Example: `opencli instagram unsave -f json`

### user
- Description: Get recent posts from an Instagram user
- Args:
  - `username` (required) — type=str; Instagram username
  - `limit` (optional) — type=int; default=12; Number of posts
- Example: `opencli instagram user -f json`
