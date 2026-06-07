# content-team Agent Pack

The `content-team` pack manages a knowledge base of guides, runbooks, and research summaries. It coordinates four specialized agent roles to research, write, edit, fact-check, and publish documentation.

## Roles

- **manager**: Triages incoming issues and events, routes them to the appropriate workflow, and coordinates all other roles. Entry point for all content work.
- **editor**: Writes and edits content for clarity, accuracy, and style. Drafts guides, runbooks, and playbooks using the established style guide and document templates.
- **researcher**: Investigates topics, gathers information from the codebase and external sources, and produces structured research summaries for editors to build on.
- **fact-checker**: Verifies claims, tests technical instructions, checks links, and validates accuracy before content is published.

## What this pack does

The `content-team` pack automates the full content lifecycle for a knowledge base:

1. A GitHub issue triggers the manager
2. The manager classifies the task and selects a workflow
3. Agents collaborate through research, drafting, fact-checking, and PR creation
4. The manager communicates status back via issue comments

Content lives in three directories:
- `guides/` — how-to guides for practitioners
- `runbooks/` — operational runbooks with step-by-step instructions
- `research/` — research summaries and investigation findings

## Workflows

- **content-lifecycle**: Full pipeline for creating or updating documentation
- **content-review**: Audit existing content for accuracy and freshness
- **research-task**: Pure research — investigate a topic and report findings

## Usage

```bash
modastack start content-team
```

This subscribes to GitHub issues in the configured repository and starts the manager agent. Label an issue with `agent`, `content`, or `research` to trigger the pack.
