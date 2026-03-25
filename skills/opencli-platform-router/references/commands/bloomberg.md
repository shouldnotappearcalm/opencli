# bloomberg

Total commands: **10**

## Commands


### businessweek
- Description: Bloomberg Businessweek top stories (RSS)
- Args:
  - `limit` (optional) — type=int; default=1; Number of feed items to return (max 20)
- Example: `opencli bloomberg businessweek -f json`

### economics
- Description: Bloomberg Economics top stories (RSS)
- Args:
  - `limit` (optional) — type=int; default=1; Number of feed items to return (max 20)
- Example: `opencli bloomberg economics -f json`

### feeds
- Description: List the Bloomberg RSS feed aliases used by the adapter
- Args: none declared
- Example: `opencli bloomberg feeds -f json`

### industries
- Description: Bloomberg Industries top stories (RSS)
- Args:
  - `limit` (optional) — type=int; default=1; Number of feed items to return (max 20)
- Example: `opencli bloomberg industries -f json`

### main
- Description: Bloomberg homepage top stories (RSS)
- Args:
  - `limit` (optional) — type=int; default=1; Number of feed items to return (max 20)
- Example: `opencli bloomberg main -f json`

### markets
- Description: Bloomberg Markets top stories (RSS)
- Args:
  - `limit` (optional) — type=int; default=1; Number of feed items to return (max 20)
- Example: `opencli bloomberg markets -f json`

### news
- Description: Read a Bloomberg story/article page and return title, full content, and media links
- Args:
  - `link` (required) — Bloomberg story/article URL or relative Bloomberg path
- Example: `opencli bloomberg news -f json`

### opinions
- Description: Bloomberg Opinion top stories (RSS)
- Args:
  - `limit` (optional) — type=int; default=1; Number of feed items to return (max 20)
- Example: `opencli bloomberg opinions -f json`

### politics
- Description: Bloomberg Politics top stories (RSS)
- Args:
  - `limit` (optional) — type=int; default=1; Number of feed items to return (max 20)
- Example: `opencli bloomberg politics -f json`

### tech
- Description: Bloomberg Tech top stories (RSS)
- Args:
  - `limit` (optional) — type=int; default=1; Number of feed items to return (max 20)
- Example: `opencli bloomberg tech -f json`
