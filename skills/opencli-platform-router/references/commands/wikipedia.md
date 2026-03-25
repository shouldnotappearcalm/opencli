# wikipedia

Total commands: **4**

## Commands


### random
- Description: Get a random Wikipedia article
- Args:
  - `lang` (optional) — default='en'; Language code (e.g. en, zh, ja)
- Example: `opencli wikipedia random -f json`

### search
- Description: Search Wikipedia articles
- Args:
  - `query` (required) — Search keyword
  - `limit` (optional) — type=int; default=10; Max results
  - `lang` (optional) — default='en'; Language code (e.g. en, zh, ja)
- Example: `opencli wikipedia search -f json`

### summary
- Description: Get Wikipedia article summary
- Args:
  - `title` (required) — Article title (e.g.
  - `lang` (optional) — default='en'; Language code (e.g. en, zh, ja)
- Example: `opencli wikipedia summary -f json`

### trending
- Description: Most-read Wikipedia articles (yesterday)
- Args:
  - `limit` (optional) — type=int; default=10; Max results
  - `lang` (optional) — default='en'; Language code (e.g. en, zh, ja)
- Example: `opencli wikipedia trending -f json`
