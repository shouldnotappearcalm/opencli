# stackoverflow

Total commands: **4**

## Commands


### bounties
- Description: Active bounties on Stack Overflow
- Args:
  - `limit` (optional) — type=int; default=10; Max number of results
- Example: `opencli stackoverflow bounties -f json`

### hot
- Description: Hot Stack Overflow questions
- Args:
  - `limit` (optional) — type=int; default=10; Max number of results
- Example: `opencli stackoverflow hot -f json`

### search
- Description: Search Stack Overflow questions
- Args:
  - `query` (required) — type=string; Search query
  - `limit` (optional) — type=int; default=10; Max number of results
- Example: `opencli stackoverflow search -f json`

### unanswered
- Description: Top voted unanswered questions on Stack Overflow
- Args:
  - `limit` (optional) — type=int; default=10; Max number of results
- Example: `opencli stackoverflow unanswered -f json`
