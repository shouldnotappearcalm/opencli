# weread

Total commands: **7**

## Commands


### book
- Description: View book details on WeRead
- Args:
  - `book-id` (required) — Book ID (numeric, from search or shelf results)
- Example: `opencli weread book -f json`

### highlights
- Description: List your highlights (underlines) in a book
- Args:
  - `book-id` (required) — Book ID (from shelf or search results)
  - `limit` (optional) — type=int; default=20; Max results
- Example: `opencli weread highlights -f json`

### notebooks
- Description: List books that have highlights or notes
- Args: none declared
- Example: `opencli weread notebooks -f json`

### notes
- Description: List your notes (thoughts) on a book
- Args:
  - `book-id` (required) — Book ID (from shelf or search results)
  - `limit` (optional) — type=int; default=20; Max results
- Example: `opencli weread notes -f json`

### ranking
- Description: WeRead book rankings by category
- Args:
  - `category` (optional) — default='all'; Category: all (default), rising, or numeric category ID
  - `limit` (optional) — type=int; default=20; Max results
- Example: `opencli weread ranking -f json`

### search
- Description: Search books on WeRead
- Args:
  - `query` (required) — Search keyword
  - `limit` (optional) — type=int; default=10; Max results
- Example: `opencli weread search -f json`

### shelf
- Description: List books on your WeRead bookshelf
- Args:
  - `limit` (optional) — type=int; default=20; Max results
- Example: `opencli weread shelf -f json`
