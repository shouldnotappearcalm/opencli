# discord-app

Total commands: **7**

## Commands


### channels
- Description: List channels in the current Discord server
- Args: none declared
- Example: `opencli discord-app channels -f json`

### members
- Description: List online members in the current Discord channel
- Args: none declared
- Example: `opencli discord-app members -f json`

### read
- Description: Read recent messages from the active Discord channel
- Args:
  - `count` (optional) — default=20)'; Number of messages to read (default: 20)
- Example: `opencli discord-app read -f json`

### search
- Description: Search messages in the current Discord server/channel (Cmd+F)
- Args:
  - `query` (required) — Search query
- Example: `opencli discord-app search -f json`

### send
- Description: Send a message in the active Discord channel
- Args:
  - `text` (required) — Message to send
- Example: `opencli discord-app send -f json`

### servers
- Description: List all Discord servers (guilds) in the sidebar
- Args: none declared
- Example: `opencli discord-app servers -f json`

### status
- Description: Check active CDP connection to Discord Desktop
- Args: none declared
- Example: `opencli discord-app status -f json`
