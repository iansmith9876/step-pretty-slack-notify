# Slack Notify Step
Posts wercker build status to a [Slack Channel](https://slack.com/).

### REQUIREMENTS

* `team` - Your Slack team subdomain.
* `token` - Your Slack integration token.
* `channel` - The Slack channel you want to send message for. (without #).

Options

* `username` - The name of your bot. (default `Wercker`)

### EXAMPLE USAGE

```yml
build:
    after-steps:
        - iansmith9876/pretty-slack-notify:
            team: mycompany
            token: $SLACK_API_TOKEN
            channel: dev
            username: cibot
```

Although this code still works (*as of June 2016*) it's not actively maintained. The original repository it was forked from has been fixed and much improved, you can find it here: https://github.com/wantedly/step-pretty-slack-notify
