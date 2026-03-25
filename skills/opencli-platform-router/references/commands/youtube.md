# youtube

Total commands: **3**

## Commands


### search
- Description: Search YouTube videos
- Args:
  - `query` (required) — Search query
  - `limit` (optional) — type=int; default=20; Max results (max 50)
- Example: `opencli youtube search -f json`

### transcript
- Description: Get YouTube video transcript/subtitles
- Args: none declared
- Example: `opencli youtube transcript -f json`

### video
- Description: Get YouTube video metadata (title, views, description, etc.)
- Args:
  - `url` (required) — YouTube video URL or video ID
- Example: `opencli youtube video -f json`
