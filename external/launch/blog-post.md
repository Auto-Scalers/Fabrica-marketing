# Launch Blog Post — Fabrica

> Builder-to-builder launch post. Tone: direct, founder-led, anti-hype. Status:
> draft for founder review. No fabricated metrics, quotes, or logos (see
> brand-guidelines.md §5).

---

# You're Building With AI, but You're Still the Bottleneck

You picked up the AI tools so you could move faster. You got a faster way to
type. What you didn't get is a faster way to ship — because between every brief
and every result, there's still one person doing the routing, the re-explaining,
and the waiting: you.

I built Fabrica because I kept watching myself do the same thing. I'd open a
chat, paste a brief, wait for a response, copy the output somewhere, then paste
it back into the next tool. One task had to finish before the next could start.
The AI was doing work. I was still the coordination layer.

This post is about what that bottleneck actually is, and the tool I'm building
to remove it without removing the judgment call.

---

## The Problem: Autocomplete Is Not Orchestration

Here's a question worth sitting with for a second. When you use a coding tool
today, what are you actually doing?

For most of us, the answer is: writing code with a very aggressive autocomplete.
The tool predicts the next chunk of your file. It's genuinely useful — it
finishes functions, fills in boilerplate, catches syntax you'd otherwise retype.
But it's still anchored to a single cursor, a single conversation, a single
person driving line by line.

That's not orchestration. That's a more efficient you.

The thing founders actually need — and this is the part the tools don't solve —
is not help writing a file. It's help moving *work*. Research, marketing copy,
a landing page, a feature branch, a pricing analysis, a support reply. Those
aren't cursor movements. They're jobs. And right now, each job has the same
dependencies: your time, your context, your attention, in sequence.

What that produces is a wall. You want to ship three things this week, but you
can only move one thing at a time. The AI removed the typing. It did nothing
about the serialization. So the bottleneck never moved — it just got a better
keyboard.

There's a second problem hiding in here, and it's the one nobody admits out
loud: delegation without control is just outsourcing your mistakes. The moment
you let an agent run unattended, you're betting the output will be right
without you looking. Sometimes it is. When it isn't, you find out after the
work shipped, not before. A lot of builders respond to this by never letting
anything run unattended — which means they're back to doing everything
themselves. The tools that want to be "autonomous" either take your judgment
out of the loop or leave you babysitting a chat window. Neither is a founder's
operating system.

The pattern is the same across every product I've watched founders reach for.
Cursor and Copilot optimize for writing code faster inside an editor. They make
you faster at the keyboard and leave the coordination to you. Agent products
take a task and disappear with it, returning hours later with output you didn't
get to steer. Both designs have the same hole in the middle: no place where
several specialized agents work in parallel, stay visible, and wait at
checkpoints for a human decision.

That hole is what Fabrica is built for.

---

## Introducing Fabrica: A Desktop Management Platform for Your CLI Agents

Fabrica is not another coding assistant, and it's not a black box you hand a task to. It's a desktop management platform that runs in your local environment: a single operating floor where you spawn, manage, and coordinate specialist CLI agents — Claude Code, Codex, OpenCode, Cursor, Devin, Hermes, Pi, and others — across your code and your business operations.

Instead of raw terminal tabs, Fabrica gives you a **Slack-style channel interface**. Each channel is a workspace where agents discuss approaches, delegate sub-tasks, and report progress in plain language. You don't need terminal fluency to direct Claude Code or Devin — you read their updates like messages from a teammate, reply in plain language, and watch the work move.

The UI is **event-driven and adaptive**. Work triggers on events — a task completing, a budget threshold approaching, an approval gate opening — not manual polling. You don't babysit terminal windows. And over time, the interface learns from your behaviors, preferences, and operational patterns to surface the most relevant views, priority alerts, and controls that matter most. The more you use Fabrica, the more the interface reflects how you actually work.

Four architectural pillars make it different:

1. **Local CLI agent orchestration.** Fabrica runs real CLI agents in local terminals. You supply your model keys directly to providers; Fabrica never calls LLMs directly, resells tokens, or marks up inference. You pay your provider for the fuel; you use Fabrica for the management floor.
2. **Agent collaboration channels & Knowledge Vault.** Instead of running isolated prompt boxes, agents talk to each other in dedicated Slack-like channels to debate approaches and delegate sub-tasks. Every agent has shared access to your **Knowledge Vault** — a simple folder of documents you drop in that serves as the single source of truth for the entire company — plus a business roadmap so agents never drift off context. Smart agents immediately know what and when each one needs to do; you don't orchestrate manually.
3. **Built to build AND run 24/7.** For software development, each task runs in an isolated git worktree so parallel changes never collide. For operations, Fabrica supports persistent daemons running 24/7 workflows — customer support triage, ecommerce management, YouTube content pipelines, HR intake — and connects to 400+ SaaS tools through our native **n8n plugin**.
4. **Governed by default.** Consequential actions pause at visual approval gates. Hard budget caps stop runaway spend before it happens, with real-time quota tracking on supported agents (Claude Code, Codex, OpenCode) and approval gates protecting everything else.

The brand promise behind all of it is simple: **your business, automated. Your judgment, still in the loop.** Fabrica doesn't replace your judgment or your team. It manages the agents so work moves continuously, keeping you where you belong — making the decisions that matter.

---

## How It Works

The shape of a Fabrica workflow is four steps, whether you're a software engineer or a business operator.

**1. Brief the agents.** Pick a role — researcher, developer, marketer, analyst, operations — and provide a brief in plain language. Drop relevant background documents into the Knowledge Vault. Fabrica spins up the right CLI agent sessions with the tools and context they need.

**2. Watch them collaborate in channels.** Agents debate approaches, delegate sub-tasks, and execute in dedicated Slack-style channels. You see updates arrive like messages — no terminal tabs to switch between. With the **Forge Pulse** activity indicator, you see at a glance what is running, waiting, or paused across all active sessions. The UI triggers alerts on events: a task completing, a budget threshold approaching, an approval gate opening.

**3. Review and approve at the gate.** Before a consequential step — merging code, pushing to production, sending an external email, or exceeding a budget threshold — the work pauses at an approval gate. You see the diff, the cost estimate, and the proposed action in Geist Mono. You approve, revise, or stop the run with a single click.

**4. Deploy and run continuously.** Approved changes merge cleanly into git worktrees or deploy via n8n workflows. For ongoing jobs like customer support or content pipelines, agents run 24/7, pausing only when a customer escalation or policy exception triggers your gate.

---

## Who It's For

**Technical founders & solo builders.** Run multiple feature branches in parallel without terminal chaos. Let Claude Code handle a database refactor while Devin writes tests in an isolated worktree, all governed by diff review before merge.

**Project managers & operators (Runners).** Direct 24/7 business workflows — customer support triage, ecommerce store management, YouTube content pipelines, HR intake — without writing code or managing raw terminal scripts.

**Lean teams & agencies.** Run multi-agent crews across multiple client projects with isolated credentials, strict per-project budget caps, and unified mobile oversight.

---

## Direct Your Agents. Run Your Business. Keep Total Control.

The tools winning today are the ones that made you faster at what you were already doing — typing code, one line at a time. Fabrica is building for the next step: the moment you move from typing every line yourself to directing and operating an entire crew of AI agents.

When you're ready to stop being the bottleneck between the brief and the result, Fabrica is open.

**[Join the Early Access Program →](https://fabrica-ai.vercel.app)**


---

## Notes

- Word count: ~1,650 including front-matter and headings (within 1,200–1,800 target).
- CTA link placeholder: replace `[Join the Fabrica waitlist]` with the actual
  waitlist URL before publish.
- No metrics, testimonials, or logos used — none are approved for publication
  (positioning-statement.md: "Social proof / traction").
- Blacklist respected: no "AI-powered," "revolutionary," "game-changing,"
  "seamless," "effortless," "magic," "set it and forget it," or "10x."
- Mechanism and control point both named in each section, per messaging
  hierarchy (brand-guidelines.md §4.3).