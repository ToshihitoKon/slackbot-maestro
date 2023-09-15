# Slackbot Maestro

Slackbot maestro is a Slack bot that can be configured with a yaml config file.

# How to use

```
./slackbot-maestro --config config.yaml
```

# Download

TODO: release architect URL

# Configurations sample

```yaml
slack:
  bot_token: xorb-XXX
  bot_user_id: UXXX
hooks:
  # @[bot] sample [arg1]
  - event: app.mention
    subcommand: "sample"
    execute: "/etc/slackbot-maestro/script/smaple.sh"
    min_args: 0
    max_args: 1

  # @[bot] ping
  - event: app.mention
    subcommand: "ping"
    execute: "/etc/slackbot-maestro/script/ping.sh"
    min_args: 0
    max_args: 0
```

# Updating

# Authors

Toshihito Kon https://github.com/ToshihitoKon

# License

MIT
