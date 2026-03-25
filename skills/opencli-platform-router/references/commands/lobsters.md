# lobsters

Total commands: **4**

## Commands


### active
- Description: Lobste.rs most active discussions
- Args:
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli lobsters active -f json`

### hot
- Description: Lobste.rs hottest stories
- Args:
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli lobsters hot -f json`

### newest
- Description: Lobste.rs newest stories
- Args:
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli lobsters newest -f json`

### tag
- Description: Lobste.rs stories by tag
- Args:
  - `tag` (required) — type=str; "Tag name (e.g. programming, rust, security, ai)"
  - `limit` (optional) — type=int; default=20; Number of stories
- Example: `opencli lobsters tag -f json`
