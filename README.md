# Slack Notify Step
Posts wercker build status to a [Slack Channel](https://slack.com/).

## REQUIREMENTS

* `team` - Your Slack team subdomain.
* `token` - Your Slack integration token.
* `channel` - The Slack channel you want to send message for. (without #).

Options

* `username` - The name of your bot. (default `Wercker`)

## EXAMPLE USAGE

```yml
build:
    after-steps:
        - iansmith9876/pretty-slack-notify:
            team: mycompany
            token: $SLACK_API_TOKEN
            channel: dev
            username: cibot
```

