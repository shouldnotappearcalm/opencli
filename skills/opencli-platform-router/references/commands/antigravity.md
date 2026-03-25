# antigravity

Total commands: **8**

## Commands


### dump
- Description: Dump the DOM to help AI understand the UI
- Args: none declared
- Example: `opencli antigravity dump -f json`

### extract-code
- Description: Extract multi-line code blocks from the current Antigravity conversation
- Args: none declared
- Example: `opencli antigravity extract-code -f json`

### model
- Description: Switch the active LLM model in Antigravity
- Args:
  - `name` (required) — Target model name (e.g. claude, gemini, o1)
- Example: `opencli antigravity model -f json`

### new
- Description: Start a new conversation / clear context in Antigravity
- Args: none declared
- Example: `opencli antigravity new -f json`

### read
- Description: Read the latest chat messages from Antigravity AI
- Args:
  - `last` (optional) — Number of recent messages to read (not fully implemented due to generic structure, currently returns full history text or latest chunk)
- Example: `opencli antigravity read -f json`

### send
- Description: Send a message to Antigravity AI via the internal Lexical editor
- Args:
  - `message` (required) — The message text to send
- Example: `opencli antigravity send -f json`

### status
- Description: Check Antigravity CDP connection and get current page state
- Args: none declared
- Example: `opencli antigravity status -f json`

### watch
- Description: Stream new chat messages from Antigravity in real-time
- Args: none declared
- Example: `opencli antigravity watch -f json`
