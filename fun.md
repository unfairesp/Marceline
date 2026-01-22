# 🎉 Fun, Games & Roleplay Documentation

Everything you need to know about the social and entertainment side of Marceline.

## 🎭 Roleplay Actions

All roleplay commands support mentioning a user and feature custom GIF/Embed responses.

### Basic Social
- **`/hug`**
  - **Permission**: `none`
  - **Inputs**: `target` (User, Required).
- **`/kiss`**
  - **Permission**: `none`
  - **Inputs**: `target` (User, Required).
- **`/cuddle`**
  - **Permission**: `none`
  - **Inputs**: `target` (User, Required).
- **`/pat`**
  - **Permission**: `none`
  - **Inputs**: `target` (User, Required).
- **`/slap`**
  - **Permission**: `none`
  - **Inputs**: `target` (User, Required).
- **`/punch`**
  - **Permission**: `none`
  - **Inputs**: `target` (User, Required).
- **`/yeet`**
  - **Permission**: `none`
  - **Inputs**: `target` (User, Required).

### Expressions (Solo or Target)
- **`/blush`**, **`/cry`**, **`/smile`**, **`/pout`**, **`/facepalm`**, **`/shrug`**
  - **Permission**: `none`
  - **Inputs**: `target` (User, Optional).
  - **Example**: `/blush target:@User` (Blushes at user) or `/blush` (Just blushes).

---

## 🎲 Interactive Games

### `/tictactoe`
- **Description**: Play a 3x3 game of X's and O's.
- **Permission**: `none`
- **Inputs**:
  - `opponent` (User, Required): The person you want to challenge.
- **Example**: `/tictactoe opponent:@Friend`

### `/connect4`
- **Description**: Drop chips to align four in a row.
- **Permission**: `none`
- **Inputs**:
  - `opponent` (User, Required): The person you want to challenge.
- **Example**: `/connect4 opponent:@Friend`

### `/trivia`
- **Description**: Answer multiple-choice questions for XP.
- **Permission**: `none`
- **Inputs**:
  - `difficulty` (String, Optional): "Easy", "Medium", "Hard".
- **Example**: `/trivia difficulty:Medium`

### `/wordguess`
- **Description**: Guess the hidden word.
- **Permission**: `none`
- **Inputs**: None.
- **Example**: `/wordguess`

---

## ✨ Fun & Random

### `/8ball`
- **Description**: Ask a question to the magic 8-ball.
- **Permission**: `none`
- **Inputs**:
  - `question` (String, Required): Your yes/no question.
- **Example**: `/8ball question:Will I win the lottery?`

### `/choose`
- **Description**: Let the bot pick between options.
- **Permission**: `none`
- **Inputs**:
  - `options` (String, Required): Options separated by commas.
- **Example**: `/choose options:Netflix, Gaming, Sleeping`

### `/lovecalc`
- **Description**: Check the compatibility between two users.
- **Permission**: `none`
- **Inputs**:
  - `user1` (User, Required).
  - `user2` (User, Optional). Default: Yourself.
- **Example**: `/lovecalc user1:@Person1 user2:@Person2`

### `/roast`
- **Description**: Deliver a random roast.
- **Permission**: `none`
- **Inputs**:
  - `target` (User, Required).
- **Example**: `/roast target:@User`

### `/raid`
- **Description**: Start a Boss Raid in the channel. Every message sent deals damage!
- **Permission**: `none`
- **Inputs**: None.
- **Example**: `/raid` (Shared XP reward for participants upon defeat).

### `/iqtest`
- **Description**: Get your "totally real" IQ score.
- **Permission**: `none`
- **Inputs**:
  - `user` (User, Optional). Default: Yourself.
- **Example**: `/iqtest user:@User`

### `/hack`
- **Description**: Run a fake hacking simulation on a user.
- **Permission**: `none`
- **Inputs**:
  - `target` (User, Required).
- **Example**: `/hack target:@User`
