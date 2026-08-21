# Fabrica-marketing — Worker Instructions (AGENTS.md)

## What This Folder Is

This is the **Fabrica marketing repo** — launch copy, brand assets, social media, press materials, blog posts, and campaign resources. You are a worker dispatched by the top-level orchestrator to complete a task in this repo.

## What You Should Know

- This is a rebrand from Orca to Fabrica
- Brand voice: technical but accessible, founder-led, anti-hype
- Target audience: technical founders, small business owners, non-technical entrepreneurs
- Key message: "Your business, automated"

## What You Do NOT Do

- **Do NOT edit** `.backup/` or `_sources/` — frozen reference copies
- **Do NOT commit or push** — make changes only, orchestrator handles git

## Key Directories

```
.Fabrica-marketing-board/ — Task file (single source of truth)

internal/             — Team strategy & planning
  brand/                — Brand guidelines, positioning statement
  research/             — Competitor landscape analysis
  planning/             — Content calendar, thread templates

external/             — Publishable content (sent/published externally)
  launch/               — Blog post, Product Hunt, Show HN, waitlist page
  email/                — Launch sequence, nurture sequence
  press/                — Press kit
  content/              — Founder story
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

## Orchestration IDs

Your task file's Session Ledger tracks these IDs for every worker session:

| ID | Format | When You Get It | How to Use It |
|----|--------|-----------------|---------------|
| `task_xxx` | `task_` + hex | `task-create --json` → `result.task.id` | Resume a stuck worker: `worker-start --task <task_id> --retry-of <dispatch_id>` |
| `ctx_xxx` | `ctx_` + hex | `worker-start --json` → `result.dispatchId` | Read worker output: `worker-read --dispatch <ctx_xxx>`. Resume: `--retry-of <ctx_xxx>` |
| `term_xxx` | `term_` + uuid | `worker-start --json` → `effects[terminal].id` | Send message to worker: `terminal send --terminal <term_xxx>`. Read output: `terminal read --terminal <term_xxx>` |
