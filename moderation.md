# 🛡️ Moderation Documentation

Detailed breakdown of all moderation and staff-related tools.

## 🎫 ModMail System

Marceline uses an "AI-First" ticket system to handle user inquiries efficiently.

### Commands
- **`/close`** (Alias: `.c`)
  - **Description**: Closes the current ticket channel and notifies the user.
  - **Permission**: `Manage Messages` (or Fake Perm: `ManageMessages`)
  - **Inputs**: None.
  - **Requirements**: Must be used within a channel starting with `ticket-`.
  - **Example**: `/close`

### Workflow
1. **User DM**: User sends a DM to the bot.
2. **AI FAQ**: Bot checks `modMailFAQ` settings. If an answer is found, the AI replies.
3. **Staff Request**: If user says "staff" or AI can't answer, a channel `ticket-[USER_ID]` is created in the `modmailCategory`.
4. **Communication**: 
   - Staff messages in the channel are forwarded to user DMs.
   - User DMs are forwarded to the ticket channel.
5. **Logging**: All messages are logged in the `modmailChannel`.

---

## 🔨 Moderation Commands

### `/ban` (Alias: `.b`)
- **Description**: Permanently ban a user from the server.
- **Permission**: `Ban Members` (or Fake Perm: `BanMembers`)
- **Inputs**:
  - `target` (User, Required): The user to ban.
  - `reason` (String, Optional): The reason for the ban.
- **Example**: `/ban target:@User reason:Breaking rules`

### `/kick` (Alias: `.k`)
- **Description**: Kick a user from the server.
- **Permission**: `Kick Members` (or Fake Perm: `KickMembers`)
- **Inputs**:
  - `target` (User, Required): The user to kick.
  - `reason` (String, Optional): The reason for the kick.
- **Example**: `/kick target:@User reason:Inappropriate behavior`

### `/warn` (Alias: `.w`)
- **Description**: Issue a formal warning to a member.
- **Permission**: `Moderate Members` (or Fake Perm: `ModerateMembers`)
- **Inputs**:
  - `target` (User, Required): The user to warn.
  - `reason` (String, Required): The reason for the warning.
- **Example**: `/warn target:@User reason:Spamming`

### `/warnings` (Alias: `.ws`)
- **Description**: View all warnings for a specific user.
- **Permission**: `none` (View), `Moderate Members` (Remove)
- **Inputs**:
  - `target` (User, Required): The user to check.
- **Example**: `/warnings target:@User`

### `/nuke` (Alias: `.n`)
- **Description**: Deletes the current channel and recreates it with the same permissions and settings.
- **Permission**: `Manage Channels` (or Fake Perm: `ManageChannels`)
- **Inputs**: None.
- **Example**: `/nuke`

### `/view` (Alias: `.v`)
- **Description**: View comprehensive moderation data for a user.
- **Permission**: `Moderate Members` (or Fake Perm: `ModerateMembers`)
- **Inputs**:
  - `target` (User, Required): The user to view.
- **Output**: Shows warnings, kicks, and active bans.
- **Example**: `/view target:@User`

### `/role` (Alias: `.r`)
- **Description**: Toggles a role for a user. If they have it, it's removed; if not, it's added.
- **Permission**: `Manage Roles` (or Fake Perm: `ManageRoles`)
- **Inputs**:
  - `target` (User, Required): The user to modify.
  - `role` (Role, Required): The role to toggle.
- **Example**: `/role target:@User role:@Moderator`

### `/fakeperms` (Alias: `.fp`)
- **Description**: Manage "Fake Permissions" that allow users to use bot commands without having the actual Discord permission.
- **Permission**: `Administrator`
- **Subcommands**:
  - `add`: Add a fake permission (e.g., `BanMembers`, `ManageMessages`).
  - `remove`: Remove a fake permission.
  - `list`: List all fake permissions for a user.
- **Example**: `/fakeperms add target:@User permission:BanMembers`

### `/infactiondm`
- **Description**: Toggle whether the bot DMs users when they receive a punishment.
- **Permission**: `Administrator`
- **Inputs**:
  - `status` (Boolean, Required): `True` to enable, `False` to disable.
- **Example**: `/infactiondm status:True`

---

## 🛡️ Anti-Abuse Configuration

Managed via the Bot Owner settings, but affects general server behavior:
- **Anti-Invite**: Automatically deletes messages containing Discord invites.
- **Anti-Mass Mention**: Deletes messages with too many user/role mentions.
- **Media Only**: Restricts certain channels to only allow attachments/links.
