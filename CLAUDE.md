# modastack-dogfood

Dogfood repo for testing modastack's content-review agent pack.

## Quick start

```bash
modastack start content-review
```

This auto-discovers the GitHub repo from git remote, subscribes to
events, and starts a manager agent that triages issues, dispatches
researchers/editors/fact-checkers, and communicates with humans.

## Structure

```
agents/content-review/   — agent pack (roles, tools, workflows)
guides/                  — how-to guides for modastack users
runbooks/                — operational runbooks
research/                — research summaries
```
