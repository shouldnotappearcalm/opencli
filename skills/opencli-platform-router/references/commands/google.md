# google

Total commands: **4**

## Commands


### news
- Description: Get Google News headlines
- Args:
  - `keyword` (optional) — Search query (omit for top stories)
  - `limit` (optional) — type=int; default=10; Number of results
  - `lang` (optional) — default='en'; Language short code (e.g. en, zh)
  - `region` (optional) — default='US'; Region code (e.g. US, CN)
- Example: `opencli google news -f json`

### search
- Description: Search Google
- Args:
  - `keyword` (required) — Search query
  - `limit` (optional) — type=int; default=10; Number of results (1-100)
  - `lang` (optional) — default='en'; Language short code (e.g. en, zh)
- Example: `opencli google search -f json`

### suggest
- Description: Get Google search suggestions
- Args:
  - `keyword` (required) — Search query
  - `lang` (optional) — default='zh-CN'; Language code
- Example: `opencli google suggest -f json`

### trends
- Description: Get Google Trends daily trending searches
- Args:
  - `region` (optional) — default='US'; Region code (e.g. US, CN, JP)
  - `limit` (optional) — type=int; default=20; Number of results
- Example: `opencli google trends -f json`
