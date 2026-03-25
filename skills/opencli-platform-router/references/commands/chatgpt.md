# chatgpt

Total commands: **5**

## Commands


### ask
- Description: Send a prompt and wait for the AI response (send + wait + read)
- Args:
  - `text` (required) — Prompt to send
  - `timeout` (optional) — default=30)'; Max seconds to wait for response (default: 30)
- Example: `opencli chatgpt ask -f json`

### new
- Description: Open a new chat in ChatGPT Desktop App
- Args: none declared
- Example: `opencli chatgpt new -f json`

### read
- Description: Read the last visible message from the focused ChatGPT Desktop window
- Args: none declared
- Example: `opencli chatgpt read -f json`

### send
- Description: Send a message to the active ChatGPT Desktop App window
- Args:
  - `text` (required) — Message to send
- Example: `opencli chatgpt send -f json`

### status
- Description: Check if ChatGPT Desktop App is running natively on macOS
- Args: none declared
- Example: `opencli chatgpt status -f json`
