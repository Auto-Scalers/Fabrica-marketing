# Show HN: Fabrica — Desktop manager for Claude Code, Cursor, Devin & CLI agents with parallel worktrees and approval gates

Fabrica is a desktop platform that manages terminal CLI agents — Claude Code, Codex, OpenCode, Cursor, Devin, Hermes, Pi, and others — with a Slack-style channel interface instead of raw terminal tabs. Agents discuss, delegate, and report in plain language. The UI is event-driven (triggering on task completions, budget thresholds, approval gates) and adapts to your preferences over time. Parallel git worktrees, a shared knowledge vault, and visual human approval gates complete the system. Work is organized as structured missions rather than scattered terminal windows: brief → plan → agent collaboration → review → approval → run → output.

We kept hitting the same wall: modern CLI agents are powerful, but managing multiple agents across a real project is chaotic. Running multiple agents in raw terminal tabs leads to file collisions, context fragmentation, lost outputs, and no natural pause point before a consequential action runs (like a destructive git command, file wipe, or external API call).

Fabrica provides a clean desktop orchestration layer over local CLI agent sessions:

- **Slack-style channel interface:** Instead of raw terminal tabs, agents report through dedicated channels — discuss, delegate, and report in plain language. No terminal fluency required.
- **Event-driven UI:** Work triggers on events (task completions, budget thresholds, approval gates), not manual polling. The interface adapts to your preferences and operational patterns over time.
- **Local terminal management:** Fabrica spawns and manages CLI agents in local terminals. You supply your own API keys directly to providers — Fabrica does not call LLMs or resell inference.
- **Isolated git worktrees:** For coding work, each agent task runs in its own isolated worktree so parallel changes never collide or corrupt main.
- **Agent collaboration channels:** Agents communicate in dedicated channels to delegate sub-tasks and debate solutions, referencing a shared local **Knowledge Vault** and business roadmap (a document drop folder that serves as their source of truth). Smart agents immediately know what and when each one needs to do — no manual orchestration required.
- **Approval gates & risk classification:** Consequential actions pause at visual approval modals displaying diffs and risk tiers.
- **Budget controls:** Set hard spend caps with real-time quota tracking on supported agents (Claude Code, Codex, OpenCode) and approval-gate governance on closed agents.
- **Built to build and run:** Run software engineering workflows alongside 24/7 continuous operations (customer support triage, ecommerce bots, YouTube content pipelines) with 400+ SaaS integrations via our native **n8n plugin**.

Early access is free. [fabrica-ai.vercel.app](https://fabrica-ai.vercel.app) — happy to answer any technical questions in the thread!