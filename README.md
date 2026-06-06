# modastack-dogfood

Dogfood repo for testing [modastack](https://github.com/moda-labs)'s `software_team` agent pack. This repo serves as a living testbed where modastack's AI agents triage GitHub issues, dispatch work to engineer agents, and communicate with humans on Slack.

## Quick start

```bash
modastack start software_team
```

This auto-discovers the GitHub repo from git remote and the Slack workspace from the bot token, subscribes to events, and starts a manager agent that triages issues, dispatches engineers, and communicates with humans on Slack.

## Repository structure

```
guides/       — how-to guides for modastack users
runbooks/     — operational runbooks
research/     — research summaries
```

## Prerequisites

- A GitHub repo with issues enabled
- A Slack bot token configured for your workspace
- The `modastack` CLI installed

## License

Internal use only.
