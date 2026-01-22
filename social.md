# 💍 Social & Community Systems

Build relationships, form exclusive clubs, and track your standing with Yui.

---

## 💍 Marriage System

Commit to another user or even attempt to win Yui's heart.

### `/marry`
- **Description**: Propose to another user. If they accept, you will both appear on each other's `/profile`.
- **Special**: You can propose to **Yui**. This requires a **Friendship Level of 100**.
- **Permission**: `none`
- **Inputs**:
  - `target` (User, Required): The person you want to marry.
- **Example**: `/marry target:@Senpai`

### `/divorce`
- **Description**: End your current marriage.
- **Permission**: `none`
- **Inputs**: None.
- **Example**: `/divorce`

---

## ♣️ Server Clubs

Create exclusive private spaces for your friends.

### `/club create`
- **Description**: Create a private text channel for your club.
- **Cost**: **50,000 XP** (Deducted from your balance).
- **Permission**: `none`
- **Inputs**:
  - `name` (String, Required): The name of your club.
- **Example**: `/club create name:Gamer-Squad`

### `/club invite`
- **Description**: Invite a user to your club's private channel.
- **Permission**: `none`
- **Inputs**:
  - `target` (User, Required): The user to invite.
- **Example**: `/club invite target:@Friend`

---

## ✨ Yui's Friendship

Track how much Yui likes (or loathes) the server members.

### `/friendship`
- **Description**: View the Friendship Leaderboard. Displays the top 10 "Favorite Senpais" and the top 5 "Biggest Nuisances".
- **Permission**: `none`
- **Inputs**: None.
- **Example**: `/friendship`

---

*Social interactions are recorded and may affect how Yui treats you in the AI Chat!*
