# modastack-dogfood

Dogfood repo for testing modastack's `content-team` agent pack. AI agents research, write, edit, and fact-check documentation — guides, runbooks, and research summaries.

This repo also serves as a **canonical example** of how to build a modastack agent pack.

## Quick start

```bash
modastack start content-team
```

This auto-discovers the GitHub repo from git remote, subscribes to events, and starts a manager agent that triages issues, dispatches content agents, and communicates status via GitHub comments.

## Agent Pack structure

This repo uses the Agent Pack format. Use it as a reference when building your own pack.

```
agents/
  registry.yaml                          # pack registry — name, version, description
  content-team/
    agent.md                             # pack overview — roles, workflows, usage
    defaults.yaml                        # entry-point role, event sources, config
    roles/
      manager.md                         # triages issues, dispatches agents
      editor.md                          # writes and edits content
      researcher.md                      # investigates topics, produces summaries
      fact-checker.md                    # verifies accuracy before publishing
    workflows/
      content-lifecycle.yaml             # full pipeline: research → draft → verify → PR
      content-review.yaml                # audit existing content for freshness
      research-task.yaml                 # pure research and investigation
```

**Key files:**
- `registry.yaml` — registers the pack so `modastack start <pack-name>` can find it
- `agent.md` — human-readable overview of what the pack does
- `defaults.yaml` — declares the entry-point role and event sources
- `roles/*.md` — one file per agent role, containing the role's prompt and instructions
- `workflows/*.yaml` — define multi-step pipelines that the manager dispatches

## Content directories

```
guides/       — how-to guides for modastack users
runbooks/     — operational runbooks
research/     — research summaries
```
