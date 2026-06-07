# modastack-dogfood

Dogfood repo for testing modastack's `content-team` agent pack. AI agents research, write, edit, and fact-check documentation — guides, runbooks, and research summaries.

## Quick start

```bash
modastack start content-team
```

This auto-discovers the GitHub repo from git remote, subscribes to events, and starts a manager agent that triages issues, dispatches content agents, and communicates status via GitHub comments.

## Structure

```
guides/       — how-to guides for modastack users
runbooks/     — operational runbooks
research/     — research summaries
```
