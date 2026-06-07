# modastack-dogfood

Dogfood repo for testing modastack's `software_team` agent pack.

## Quick start

```bash
modastack start software_team
```

This auto-discovers the GitHub repo from git remote and the Slack workspace from the bot token, subscribes to events, and starts a manager agent that triages issues, dispatches engineers, and communicates with humans on Slack.

## Structure

```
guides/       — how-to guides for modastack users
runbooks/     — operational runbooks
research/     — research summaries
```
