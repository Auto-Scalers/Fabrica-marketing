# Show HN: Fabrica — Agentic IDE with parallel agents and approval gates

Fabrica is an agentic IDE that runs multiple coding and business agents in parallel, each in its own isolated git worktree, with approval gates where consequential work pauses for review. Work is organized as tasks instead of a single long chat: brief → plan → review → run → output, with state visible across everything in flight.

We kept hitting the same wall. A single agent handles one task well, but a real project is a dozen tasks touching the same codebase. Run them in one working directory and they collide; queue them serially and capacity caps at one thing at a time. And when an agent was about to do something consequential, there was no natural point to stop and check it. So we built the orchestration around isolation and control instead of around chat.

Technically, the core is an orchestration layer that gives each task its own brief and context. For code work we create a separate git worktree per agent, so each agent gets a physically isolated working directory and branch — parallel changes never share state, and a failed run can be discarded without touching the main tree. Tasks move through explicit gates: plan review, diff review, budget checkpoints. A run halts at any gate that requires approval and only resumes when the reviewer approves; high-risk steps like merges, deploys, or spend past a cap are gated by default. Agents are model-agnostic — you bring your own keys and pay providers directly, so model spend stays visible and bounded.

What's different:

- **Parallel, not sequential** — agents run simultaneously in isolated worktrees instead of queuing in one thread.
- **Approval gates as designed control points** — the reviewer sees the plan and the diff before work moves forward, not after.
- **Visible work** — tasks and outputs live in one surface, not buried in chat history.
- **Bring-your-own-key** — no opaque credit pools; hard budget stops by default.

Early access is free. [fabrica.app](https://fabrica.app) — happy to answer questions in the thread.