# Steam Deck Bot
Discord bot for Steam Deck Discord specific use.

## Usage
```
pip install -r requirements.txt
python bot.py
```

## Configuration
A config.json file is required for the bot to run. An example is supplied in the `config.json.example` file.

## Commands
### reload
- Allows live reloading of cogs. Useful for testing and debugging.
- Requires `BOT_DEV` role.
- Usage: `>reload cogs.<cogname>`
- Example: `>reload cogs.helper_role`

### sitdown
- Gives the mentioned users the sit-down role specified in the config.
- Requires `HELPER` role.
- Usage: `>sitdown <user1> <user2> <user3>...`
- Example: `>sitdown @TestUser#1234`

### sitdownrelease
- Removes the sit-down role from the mentioned users.
- Requires `HELPER` role.
- Usage: `>sitdownrelease <user1> <user2> <user3>...`
- Example: `>sitdownrelease @TestUser#1234`

### scoopnotification
- Notifies the `NEWSJUNKIE` role members in the `SCOOP` channel. Can only be used every hour.
- Requires `RESEARCHER` role.
- Usage: `>scoopnotification`
