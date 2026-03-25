# chatwise

Total commands: **9**

## Commands


### ask
- Description: Send a prompt and wait for the AI response (send + wait + read)
- Args:
  - `text` (required) — Prompt to send
  - `timeout` (optional) — default=30)'; Max seconds to wait (default: 30)
- Example: `opencli chatwise ask -f json`

### export
- Description: Export the current ChatWise conversation to a Markdown file
- Args:
  - `output` (optional) — default=/tmp/chatwise-export.md)'; Output file (default: /tmp/chatwise-export.md)
- Example: `opencli chatwise export -f json`

### history
- Description: List conversation history in ChatWise sidebar
- Args: none declared
- Example: `opencli chatwise history -f json`

### model
- Description: Get or switch the active AI model in ChatWise
- Args:
  - `model-name` (optional) — Model to switch to (e.g. gpt-4, claude-3)
- Example: `opencli chatwise model -f json`

### new
- Description: Start a new conversation in ChatWise
- Args: none declared
- Example: `opencli chatwise new -f json`

### read
- Description: Read the current ChatWise conversation history
- Args: none declared
- Example: `opencli chatwise read -f json`

### screenshot
- Description: Capture a snapshot of the current ChatWise window (DOM + Accessibility tree)
- Args:
  - `output` (optional) — default=/tmp/chatwise-snapshot)'; Output file path (default: /tmp/chatwise-snapshot)
- Example: `opencli chatwise screenshot -f json`

### send
- Description: Send a message to the active ChatWise conversation
- Args:
  - `text` (required) — Message to send
- Example: `opencli chatwise send -f json`

### status
- Description: Check active CDP connection to ChatWise Desktop
- Args: none declared
- Example: `opencli chatwise status -f json`
