# doubao-app

Total commands: **7**

## Commands


### ask
- Description: Send a message to Doubao desktop app and wait for the AI response
- Args:
  - `text` (required) — Prompt to send
  - `timeout` (optional) — type=int; default=30; Max seconds to wait for response
- Example: `opencli doubao-app ask -f json`

### dump
- Description: Dump Doubao desktop app DOM and snapshot to /tmp for debugging
- Args: none declared
- Example: `opencli doubao-app dump -f json`

### new
- Description: Start a new chat in Doubao desktop app
- Args: none declared
- Example: `opencli doubao-app new -f json`

### read
- Description: Read chat history from Doubao desktop app
- Args: none declared
- Example: `opencli doubao-app read -f json`

### screenshot
- Description: Capture a screenshot of the Doubao desktop app window
- Args:
  - `output` (optional) — default=/tmp/doubao-screenshot.png)'; Output file path (default: /tmp/doubao-screenshot.png)
- Example: `opencli doubao-app screenshot -f json`

### send
- Description: Send a message to Doubao desktop app
- Args:
  - `text` (required) — Message text to send
- Example: `opencli doubao-app send -f json`

### status
- Description: Check CDP connection to Doubao desktop app
- Args: none declared
- Example: `opencli doubao-app status -f json`
