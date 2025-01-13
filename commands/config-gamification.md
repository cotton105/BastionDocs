# `/config gamification <messages> <channel> <message> <multiplier>`
Gamification refers to Guild XP & Leaderboards.

## Arguments
### `messages`
*boolean*
- Whether to enable Gamification in the server.

### `channel`
*text channel*
- The text channel to send "level-up" messages to. If unspecified, it will use the same channel as the user who leveled up.

### `message`
*string*
- A custom message to display when a user levels up. Supports tokens, emojis & markdown.
- Supported tokens are:
  - ***%level%*** - the new level of the user.
  - ***%username%*** - the user's name.
  - ***%message%*** - the message which triggered the level-up.
  - ***%date%*** - the UTC date on which the level-up occurred.
  - ***%time%*** - the UTC time at which the level-up occurred.
- Default:
  > You've leveled up to **Level %level%**!
  
  Or, your Guild's equivalent locale translation.

### `multiplier`
*number*
- Specifies a ratio of XP required per level.
- Lower values mean more XP is required to level-up.
- Default: `0.42`
