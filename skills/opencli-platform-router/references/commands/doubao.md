# doubao

Total commands: **5**

## Commands


### ask
- Description: Send a prompt and wait for the Doubao response
- Args:
  - `text` (required) — Prompt to send
  - `timeout` (optional) — default=60)'; Max seconds to wait (default: 60)
- Example: `opencli doubao ask -f json`

### new
- Description: Start a new conversation in Doubao web chat
- Args: none declared
- Example: `opencli doubao new -f json`

### read
- Description: Read the current Doubao conversation history
- Args: none declared
- Example: `opencli doubao read -f json`

### send
- Description: Send a message to Doubao web chat
- Args:
  - `text` (required) — Message to send
- Example: `opencli doubao send -f json`

### status
- Description: Check Doubao chat page availability and login state
- Args: none declared
- Example: `opencli doubao status -f json`
