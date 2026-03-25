# devto

Total commands: **3**

## Commands


### tag
- Description: Latest DEV.to articles for a specific tag
- Args:
  - `tag` (required) — type=str; "Tag name (e.g. javascript, python, webdev)"
  - `limit` (optional) — type=int; default=20; Number of articles
- Example: `opencli devto tag -f json`

### top
- Description: Top DEV.to articles of the day
- Args:
  - `limit` (optional) — type=int; default=20; Number of articles
- Example: `opencli devto top -f json`

### user
- Description: Recent DEV.to articles from a specific user
- Args:
  - `username` (required) — type=str; "DEV.to username (e.g. ben, thepracticaldev)"
  - `limit` (optional) — type=int; default=20; Number of articles
- Example: `opencli devto user -f json`
