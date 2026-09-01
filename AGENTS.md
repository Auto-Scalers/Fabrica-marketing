# Fabrica-marketing — Worker Instructions (AGENTS.md)

## What This Folder Is

Brand guidelines, positioning, and competitor research for Fabrica. You are a worker dispatched by the top-level orchestrator to complete a task in this repo.

## What You Should Know

- Brand voice: direct, commanding, builder-first
- Target audience: founders, solo builders, lean teams
- Key message: "The Next AI Exit"

## Tech Stack

- Plain Markdown documents (no build step, no framework)
- Everything is reviewable as text — write clean, well-structured Markdown

## Commands

No build or test tooling. Before claiming DONE:

- Proofread every deliverable (spelling, brand voice, blacklist terms absent).
- Verify every claim traces to the internal brand files.
- Confirm no Orca/Stably leftovers: search `internal/` for `orca`/`stablyai`.

## Definition of Done

A task is DONE only when ALL of these hold:

1. **Deliverable complete:** the file exists in the correct `internal/` folder, follows brand voice, respects the blacklist.
2. **No Orca/Stably leftovers** in any content.
3. **Tracking files updated in the same edit:** task status + Rollup recount in `.Fabrica-marketing-board/Fabrica-marketing-tasks.md`, Checkpoint table, Session Ledger row.

## What You Do NOT Do

- **Do NOT commit or push** — make changes only, orchestrator handles git

## Key Directories

```
.Fabrica-marketing-board/ — Task file (single source of truth)

internal/
  brand/                — Brand guidelines, positioning statement
  research/             — Competitor landscape analysis
```

## Task File

Your task file is `.Fabrica-marketing-board/Fabrica-marketing-tasks.md` — the single source of truth for all marketing work.

## How to Send Results

When your task is complete, send `worker_done`:

```bash
orca orchestration send --type worker_done --subject "Task complete" --body "Summary of what was done" --task-id <task_id> --dispatch-id <dispatch_id> --outcome succeeded --files-modified "path/a,path/b" --json
```

If blocked:
```bash
orca orchestration send --type escalation --subject "Blocked" --body "What happened and what's needed" --task-id <task_id> --dispatch-id <dispatch_id> --json
```
