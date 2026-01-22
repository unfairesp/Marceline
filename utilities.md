# 🛠️ Utilities Documentation

Full breakdown of AI, productivity, and information tools.

## 🤖 AI Features

### `/recap`
- **Description**: AI-generated summary of recent channel conversation.
- **Permission**: `none`
- **Inputs**:
  - `limit` (Integer, Optional): Number of messages to read (10-100). Default: 50.
- **Output**: A concise summary of topics discussed.
- **Example**: `/recap limit:30`

### `/vision`
- **Description**: Ask the AI questions about an image.
- **Permission**: `none`
- **Inputs**:
  - `image` (Attachment, Required): The image to analyze.
  - `question` (String, Required): What you want to know about the image.
- **Example**: `/vision image:[Upload] question:What color is the car?`

### `/translate`
- **Description**: Translate text using AI.
- **Permission**: `none`
- **Inputs**:
  - `text` (String, Required): The content to translate.
  - `to` (String, Required): Target language (e.g., "English", "Spanish", "Japanese").
- **Example**: `/translate text:Hola mundo to:English`

---

## 📋 General Tools

### `/help` (Alias: `.h`)
- **Description**: Displays all available commands or detailed info about a specific command.
- **Example**: `/help` or `/help command:ban`

### `/embed`
- **Description**: Create a custom embedded message.
- **Permission**: `Manage Messages`
- **Inputs**:
  - `title` (String, Required): Title of the embed.
  - `description` (String, Required): Body text.
  - `color` (String, Optional): Hex color code (e.g., "#ff0000").
  - `image` (Attachment, Optional): Image to display.
  - `thumbnail` (Attachment, Optional): Small side image.
  - `footer` (String, Optional): Text at the bottom.
- **Example**: `/embed title:Welcome description:Please read the rules color:#00ff00`

### `/suggest`
- **Description**: Send a suggestion directly to the Bot Owner's DMs.
- **Permission**: `none`
- **Inputs**:
  - `suggestion` (String, Required): Your feedback/idea.
- **Example**: `/suggest Add more colors to the embed command!`

### `/remind`
- **Description**: Set a personal reminder.
- **Permission**: `none`
- **Inputs**:
  - `time` (String, Required): When to remind you (e.g., "1h", "30m", "1d").
  - `reason` (String, Required): What the reminder is for.
- **Example**: `/remind time:2h reason:Check the oven`

### `/poll`
- **Description**: Create a simple reaction-based poll.
- **Permission**: `none`
- **Inputs**:
  - `question` (String, Required): The topic of the poll.
  - `options` (String, Required): Options separated by commas (max 10).
- **Example**: `/poll question:Pizza or Burgers? options:Pizza, Burgers`

### `/sticky`
- **Description**: Keeps a message pinned to the bottom of the channel.
- **Permission**: `Manage Messages`
- **Inputs**:
  - `message` (String, Required): The text to keep sticky.
- **Example**: `/sticky message:Remember to use the correct channel!`

### `/afk`
- **Description**: Set an AFK status that will be shown when you are mentioned.
- **Permission**: `none`
- **Inputs**:
  - `reason` (String, Optional): Why you are AFK.
- **Example**: `/afk reason:Studying for exams`

### `/snipe`
- **Description**: Retrieve the last deleted message in the current channel.
- **Permission**: `none`
- **Example**: `/snipe`

### `/confess`
- **Description**: Send an anonymous confession to a designated channel.
- **Permission**: `none`
- **Inputs**:
  - `confession` (String, Required): Your anonymous message.
- **Example**: `/confess confession:I actually like pineapple on pizza.`

---

## 📊 Information & Stats

### `/serverinfo`
- **Description**: Displays detailed information about the current server.
- **Example**: `/serverinfo`

### `/userinfo`
- **Description**: Displays detailed information about a user.
- **Inputs**:
  - `target` (User, Optional): The user to check. Defaults to yourself.
- **Example**: `/userinfo target:@User`

### `/avatar`
- **Description**: Shows the avatar of a user.
- **Inputs**:
  - `target` (User, Optional): The user to check. Defaults to yourself.
- **Example**: `/avatar target:@User`

### `/ping`
- **Description**: Checks the bot's latency and heartbeat.
- **Example**: `/ping`

### `/uptime`
- **Description**: Shows how long the bot has been online.
- **Example**: `/uptime`

### `/botstats`
- **Description**: Displays technical statistics about the bot's performance.
- **Example**: `/botstats`

---

## 🤖 Bot Management

### `/bot pfp`
- **Description**: Change the bot's server-specific profile picture (Per-Server Avatar).
- **Permission**: `Server Owner` or `Bot Owner`
- **Inputs**:
  - `image` (Attachment, Optional): The new profile picture.
  - `reset` (Literal String): Type "reset" as a URL or argument to revert to the global avatar.
- **Requirements**: Server must be **Boost Level 2**.
- **Example**: `/bot pfp image:[Upload]` or `.bot pfp reset`

---


### `/google`
- **Description**: Search Google.
- **Permission**: `none`
- **Inputs**:
  - `query` (String, Required): Search terms.
- **Example**: `/google query:Discord.js documentation`

### `/weather`
- **Description**: Get current weather.
- **Permission**: `none`
- **Inputs**:
  - `location` (String, Required): City/Country name.
- **Example**: `/weather location:London`

### `/crypto`
- **Description**: Get cryptocurrency prices.
- **Permission**: `none`
- **Inputs**:
  - `coin` (String, Required): Coin symbol (e.g., "BTC", "ETH").
- **Example**: `/crypto coin:BTC`

### `/dictionary`
- **Description**: Look up a word definition.
- **Permission**: `none`
- **Inputs**:
  - `word` (String, Required): Word to define.
- **Example**: `/dictionary word:Ephemeral`
