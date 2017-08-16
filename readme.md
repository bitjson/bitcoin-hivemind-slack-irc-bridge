# bitcoin-hivemind-slack-irc-bridge

Add `config.json` to top-level, replacing `IRC_NICKNAME`, `SLACK_TOKEN`, and `IRC_PASSWORD`:

```json
{
  "nickname": "IRC_NICKNAME",
  "server": "irc.freenode.org",
  "token": "SLACK_TOKEN",
  "avatarUrl": "https://robohash.org/$username.png?size=48x48",
  "autoSendCommands": [["PRIVMSG", "NickServ", "IDENTIFY IRC_PASSWORD"]],
  "channelMapping": {
    "#drivechain-dev-irc": "#drivechain-dev"
  }
}
```