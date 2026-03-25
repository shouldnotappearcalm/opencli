# xiaoyuzhou

Total commands: **3**

## Commands


### episode
- Description: View details of a Xiaoyuzhou podcast episode
- Args:
  - `id` (required) — Episode ID (eid from podcast-episodes output)
- Example: `opencli xiaoyuzhou episode -f json`

### podcast
- Description: View a Xiaoyuzhou podcast profile
- Args:
  - `id` (required) — Podcast ID (from xiaoyuzhoufm.com URL)
- Example: `opencli xiaoyuzhou podcast -f json`

### podcast-episodes
- Description: List recent episodes of a Xiaoyuzhou podcast (up to 15, SSR limit)
- Args:
  - `id` (required) — Podcast ID (from xiaoyuzhoufm.com URL)
  - `limit` (optional) — type=int; default=15; Max episodes to show (up to 15, SSR limit)
- Example: `opencli xiaoyuzhou podcast-episodes -f json`
