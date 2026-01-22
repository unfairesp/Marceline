# Marceline - Private Server Assistant

Marceline is a multi-purpose, high-performance Discord bot designed specifically for private server management, engagement, and advanced AI-powered interactions. This bot is a **private source** project, built to provide a seamless and feature-rich experience for its users.

## 🌟 Key Features

- **Advanced AI Integration**: Powered by Hugging Face models, Marceline features a unique personality (Yui), AI-powered ModMail with FAQ capabilities, channel summarization (/recap), and vision-based image analysis.
- **Robust Moderation**: Comprehensive toolset for server staff including a dedicated ModMail ticket system with category support, infraction tracking, and automated anti-abuse systems.
- **Dynamic Economy & Leveling**: Engaging XP-based system with role-based income, daily rewards, and a variety of gambling/mini-games.
- **Personalized Profiles**: Customizable user profiles with badge shops, reputation systems, and a pet system that tracks growth and interactions.
- **Detailed Analytics**: Track message activity, voice channel usage, and peak server activity hours with visual stats.
- **Advanced Logging**: A granular system that tracks message edits/deletions, member changes, channel updates, and more, including who caused the action.
- **Utility & Fun**: A massive collection of utility tools (QR generators, translators, currency converters) and fun commands (Roleplay, Animals, Games).

## 📜 Recent Changes (Changelog)

### [2026-01-22]
- **Added Advanced Logging System**:
    - New `/logs setup` command to auto-generate 6 specialized logging channels.
    - Deep integration with Discord Audit Logs to track executors (who deleted/edited/created) across all major events.
    - Security-first permissions: Log categories now automatically deny `Manage Messages` for safety.
- **Fixed & Enhanced Bot PFP Management**:
    - Fixed error in `/bot pfp` command for server-specific avatars.
    - Updated permissions: `/bot pfp` is now restricted to **Server Owners** and **Bot Owners** only.
    - Added `reset` functionality to revert to the bot's global profile picture.
- **Slash Command Optimization**:
    - Removed Slash Commands for: `Roleplay`, `Animals`, `Games`, `Levels`, `Fun`, and `Economy` (including Pets and Clubs).
    - These commands remain fully functional via **Prefix Syntax** (`.command`).
    - This reduces slash command clutter and improves bot responsiveness.
- **Documentation Overhaul**: Updated all `.md` files in the `github/` directory to reflect the new prefix-only status for relevant categories.

---

## 💡 Suggestion System (`/suggest`)

The bot features a direct line of communication between users and the server owner.

- **Command**: `/suggest`
- **Inputs**:
  - `suggestion` (String, Required): The content of your suggestion or feedback.
- **How it works**:
  - When a user runs `/suggest`, the bot creates a professional embed containing the suggestion.
  - This embed is **Directly Messaged (DM)** to the Bot Owner, ensuring that your feedback is seen personally by the administration.
  - The user receives an ephemeral confirmation that their suggestion has been delivered.
- **Example**: `/suggest Add a new channel for pet pictures!`

## 📚 Detailed Documentation

Detailed documentation for each feature category can be found in the following files. These files contain a full breakdown of every command, including required options, subcommands, and usage examples.

- [🛡️ Moderation](moderation.md) - Staff tools and ModMail system.
- [📈 Levels & Economy](levels.md) - XP, Ranking, and Gambling systems.
- [👤 Profiles & Badges](profiles.md) - User profiles and customization.
- [💍 Social & Community](social.md) - Social interactions and community tools.
- [🛠️ Utilities](utilities.md) - AI Recaps, Vision, and general tools.
- [🎮 Games](games.md) - Interactive mini-games and gambling.
- [📊 Statistics](stats.md) - Server analytics and leaderboards.
- [🔍 Search & Info](search.md) - Web-based search and info commands.
- [🎭 Roleplay](roleplay.md) - Interactive social commands.
- [🐶 Animals](animals.md) - Fun animal-themed commands.
- [✨ Booster Features](booster.md) - Exclusive perks for server boosters.
- [⚙️ Custom Systems](custom.md) - Server-specific custom triggers.
- [🎉 Fun Commands](fun.md) - Games, jokes, and random generators.

---

*Marceline is a private project and is not intended for public distribution. All rights reserved.*
