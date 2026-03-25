# hackernews

Total commands: **8**

## Commands


### ask
- Description: Hacker News Ask HN posts
- Args:
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli hackernews ask -f json`

### best
- Description: Hacker News best stories
- Args:
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli hackernews best -f json`

### jobs
- Description: Hacker News job postings
- Args:
  - `limit` (optional) — type=int; default=20; Number of job postings
- Example: `opencli hackernews jobs -f json`

### new
- Description: Hacker News newest stories
- Args:
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli hackernews new -f json`

### search
- Description: Search Hacker News stories
- Args:
  - `query` (required) — type=str; Search query
  - `limit` (optional) — type=int; default=20; Number of results
  - `sort` (optional) — type=str; default=relevance; Sort by relevance or date
- Example: `opencli hackernews search -f json`

### show
- Description: Hacker News Show HN posts
- Args:
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli hackernews show -f json`

### top
- Description: Hacker News top stories
- Args:
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli hackernews top -f json`

### user
- Description: Hacker News user profile
- Args:
  - `username` (required) — type=str; HN username
- Example: `opencli hackernews user -f json`
