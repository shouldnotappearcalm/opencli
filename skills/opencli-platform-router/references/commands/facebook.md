# facebook

Total commands: **10**

## Commands


### add-friend
- Description: Send a friend request on Facebook
- Args:
  - `username` (required) — type=str; Facebook username or profile URL
- Example: `opencli facebook add-friend -f json`

### events
- Description: Browse Facebook event categories
- Args:
  - `limit` (optional) — type=int; default=15; Number of categories
- Example: `opencli facebook events -f json`

### feed
- Description: Get your Facebook news feed
- Args:
  - `limit` (optional) — type=int; default=10; Number of posts
- Example: `opencli facebook feed -f json`

### friends
- Description: Get Facebook friend suggestions
- Args:
  - `limit` (optional) — type=int; default=10; Number of friend suggestions
- Example: `opencli facebook friends -f json`

### groups
- Description: List your Facebook groups
- Args:
  - `limit` (optional) — type=int; default=20; Number of groups
- Example: `opencli facebook groups -f json`

### join-group
- Description: Join a Facebook group
- Args:
  - `group` (required) — type=str; Group ID or URL path (e.g. '1876150192925481' or group name)
- Example: `opencli facebook join-group -f json`

### memories
- Description: Get your Facebook memories (On This Day)
- Args:
  - `limit` (optional) — type=int; default=10; Number of memories
- Example: `opencli facebook memories -f json`

### notifications
- Description: Get recent Facebook notifications
- Args:
  - `limit` (optional) — type=int; default=15; Number of notifications
- Example: `opencli facebook notifications -f json`

### profile
- Description: Get Facebook user/page profile info
- Args:
  - `username` (required) — type=str; Facebook username or page name
- Example: `opencli facebook profile -f json`

### search
- Description: Search Facebook for people, pages, or posts
- Args:
  - `query` (required) — type=str; Search query
  - `limit` (optional) — type=int; default=10; Number of results
- Example: `opencli facebook search -f json`
