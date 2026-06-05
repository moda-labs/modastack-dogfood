# modastack-dogfood

Dogfood repo for testing modastack with non-engineering workflows.
This is a knowledge base managed by AI content agents (researcher,
editor, fact-checker) rather than software engineers.

## Structure

```
guides/       — how-to guides for modastack users
runbooks/     — operational runbooks with step-by-step procedures
research/     — research summaries produced by researcher agents
```

## Content standards

- Guides: clear purpose, prerequisites, numbered steps, troubleshooting
- Runbooks: trigger condition, step-by-step with expected outcomes, escalation path
- Research: structured summary, key findings, sources cited

## Modastack config

Custom roles in `.modastack/agents/`:
- `researcher` — investigates topics, produces research summaries
- `editor` — writes and edits content following the style guide
- `fact-checker` — verifies accuracy, tests instructions, checks links

Custom workflows in `.modastack/workflows/`:
- `content-lifecycle` — full content creation pipeline
- `research-task` — pure research and investigation
- `content-review` — audit existing content for freshness
