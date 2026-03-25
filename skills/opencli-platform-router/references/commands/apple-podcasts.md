# apple-podcasts

Total commands: **3**

## Commands


### episodes
- Description: List recent episodes of an Apple Podcast (use ID from search)
- Args:
  - `id` (required) — Podcast ID (collectionId from search output)
  - `limit` (optional) — type=int; default=15; Max episodes to show
- Example: `opencli apple-podcasts episodes -f json`

### search
- Description: Search Apple Podcasts
- Args:
  - `query` (required) — Search keyword
  - `limit` (optional) — type=int; default=10; Max results
- Example: `opencli apple-podcasts search -f json`

### top
- Description: Top podcasts chart on Apple Podcasts
- Args:
  - `limit` (optional) — type=int; default=20; Number of podcasts (max 100)
  - `country` (optional) — default='us'; Country code (e.g. us, cn, gb, jp)
- Example: `opencli apple-podcasts top -f json`
