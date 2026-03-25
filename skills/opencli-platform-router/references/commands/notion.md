# notion

Total commands: **8**

## Commands


### export
- Description: Export the current Notion page as Markdown
- Args:
  - `output` (optional) — default=/tmp/notion-export.md)'; Output file (default: /tmp/notion-export.md)
- Example: `opencli notion export -f json`

### favorites
- Description: List pages from the Notion Favorites section in the sidebar
- Args: none declared
- Example: `opencli notion favorites -f json`

### new
- Description: Create a new page in Notion
- Args:
  - `title` (optional) — Page title (optional)
- Example: `opencli notion new -f json`

### read
- Description: Read the content of the currently open Notion page
- Args: none declared
- Example: `opencli notion read -f json`

### search
- Description: Search pages and databases in Notion via Quick Find (Cmd+P)
- Args:
  - `query` (required) — Search query
- Example: `opencli notion search -f json`

### sidebar
- Description: List pages and databases from the Notion sidebar
- Args: none declared
- Example: `opencli notion sidebar -f json`

### status
- Description: Check active CDP connection to Notion Desktop
- Args: none declared
- Example: `opencli notion status -f json`

### write
- Description: Append text content to the currently open Notion page
- Args:
  - `text` (required) — Text to append to the page
- Example: `opencli notion write -f json`
