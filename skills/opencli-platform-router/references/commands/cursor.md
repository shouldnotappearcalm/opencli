# cursor

Total commands: **10**

## Commands


### ask
- Description: Send a prompt and wait for the AI response (send + wait + read)
- Args:
  - `text` (required) — Prompt to send
  - `timeout` (optional) — default=30)'; Max seconds to wait for response (default: 30)
- Example: `opencli cursor ask -f json`

### composer
- Description: Send a prompt directly into Cursor Composer (Cmd+I shortcut)
- Args:
  - `text` (required) — Text to send into Composer
- Example: `opencli cursor composer -f json`

### dump
- Description: Dump the DOM and Accessibility tree of Cursor for reverse-engineering
- Args: none declared
- Example: `opencli cursor dump -f json`

### extract-code
- Description: Extract multi-line code blocks from the current Cursor conversation
- Args: none declared
- Example: `opencli cursor extract-code -f json`

### history
- Description: List recent chat sessions from the Cursor sidebar
- Args: none declared
- Example: `opencli cursor history -f json`

### model
- Description: Get or switch the currently active AI model in Cursor
- Args:
  - `model-name` (optional) — The ID of the model to switch to (e.g. claude-3.5-sonnet)
- Example: `opencli cursor model -f json`

### new
- Description: Start a new Cursor chat or Composer session
- Args: none declared
- Example: `opencli cursor new -f json`

### read
- Description: Read the current Cursor chat/composer conversation history
- Args: none declared
- Example: `opencli cursor read -f json`

### send
- Description: Send a prompt directly into Cursor Composer/Chat
- Args:
  - `text` (required) — Text to send into Cursor
- Example: `opencli cursor send -f json`

### status
- Description: Check active CDP connection to Cursor AI Editor
- Args: none declared
- Example: `opencli cursor status -f json`
