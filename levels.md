# 📈 Levels & Economy Documentation

Comprehensive guide to the ranking, currency, and business systems.

## 💎 Leveling System

### `/rank`
- **Description**: Displays your current level, total XP, and rank within the server.
- **Permission**: `none`
- **Inputs**:
  - `user` (User, Optional): View the rank of another user.
- **Example**: `/rank user:@Friend`

### `/leaderboard`
- **Description**: Shows the top 10 users in the server by XP.
- **Permission**: `none`
- **Inputs**: None.
- **Example**: `/leaderboard`

### `/daily`
- **Description**: Claim your daily XP reward.
- **Permission**: `none`
- **Inputs**: None.
- **Cooldown**: 24 Hours.
- **Bonus**: Reward increases based on your roles' "Role Income" settings.
- **Example**: `/daily`

### `/xp` (Staff Only)
- **Description**: Manage user XP.
- **Permission**: `Administrator`
- **Subcommands**:
  - `add`:
    - `target` (User, Required): User to give XP.
    - `amount` (Integer, Required): Amount of XP.
  - `remove`:
    - `target` (User, Required): User to take XP from.
    - `amount` (Integer, Required): Amount of XP.
  - `set`:
    - `target` (User, Required): User to set XP for.
    - `amount` (Integer, Required): Exact XP value.
- **Example**: `/xp add target:@User amount:1000`

---

## 🎲 Gambling & Games

### `/blackjack`
- **Description**: Play a game of Blackjack against the bot.
- **Permission**: `none`
- **Inputs**:
  - `bet` (Integer, Required): Amount of XP to wager.
- **Example**: `/blackjack bet:500`

### `/horserace`
- **Description**: Bet on a virtual horse race.
- **Permission**: `none`
- **Inputs**:
  - `bet` (Integer, Required): Amount of XP to wager.
- **Example**: `/horserace bet:200`

### `/coinflipduel`
- **Description**: Challenge another user to a coin flip.
- **Permission**: `none`
- **Inputs**:
  - `target` (User, Required): The opponent.
  - `bet` (Integer, Required): The amount both users will wager.
- **Example**: `/coinflipduel target:@User bet:1000`

### `/gamble`
- **Description**: Roll a 100-sided die. Roll > 50 to win.
- **Permission**: `none`
- **Inputs**:
  - `bet` (Integer, Required): Amount of XP to wager.
- **Example**: `/gamble bet:100`

### `/slots`
- **Description**: Spin the slot machine.
- **Permission**: `none`
- **Inputs**:
  - `bet` (Integer, Required): Amount of XP to wager.
- **Example**: `/slots bet:300`

### `/roulette`
- **Description**: Classic roulette gambling.
- **Permission**: `none`
- **Inputs**:
  - `bet` (Integer, Required): Amount of XP to wager.
  - `space` (String, Required): Where to bet (e.g., "Red", "Black", "1-18", "19-36").
- **Example**: `/roulette bet:500 space:Red`

---

## 📈 Advanced Economy

### `/stocks`
- **Description**: Interact with the simulated stock market.
- **Permission**: `none`
- **Subcommands**:
  - `buy`:
    - `symbol` (String, Required): Stock ticker (e.g., "AAPL", "BTC").
    - `amount` (Integer, Required): Number of shares.
  - `sell`:
    - `symbol` (String, Required): Stock ticker.
    - `amount` (Integer, Required): Number of shares.
  - `portfolio`: View your current holdings and profit/loss.
  - `view`:
    - `symbol` (String, Required): Check the current price of a stock.
- **Example**: `/stocks buy symbol:BTC amount:1`

### `/business`
- **Description**: Manage your virtual business for passive income.
- **Permission**: `none`
- **Subcommands**:
  - `create`:
    - `name` (String, Required): Name of your business.
  - `stats`: View your business's revenue and level.
  - `upgrade`: Use XP to increase your business's hourly earnings.
  - `collect`: Claim your accumulated business earnings.
- **Example**: `/business create name:MarceCorp`
