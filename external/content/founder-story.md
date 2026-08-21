# The Founder's Bottleneck: The Fabrica Founder Story

Three versions of the founding narrative, built on the same arc:

1. **Struggle** — the frustration of running a business with scattered AI tools and raw terminal tabs
2. **Insight** — CLI agent orchestration, Slack-like agent channels, Knowledge Vault, approval gates
3. **Build** — how we started, what failed, the decisions we kept
4. **Vision** — where Fabrica goes and what "The Next AI Exit" means for builders and operators

Founder voice throughout: direct, grounded, technical-but-accessible, anti-hype.

---

## Version 1 — Blog Post (1500–2000 words)

# From Doing Every Task to Directing the Work: The Fabrica Story

I spent the first part of my career convinced the bottleneck was skill. Write better code. Learn more frameworks. Ship faster. If I was competent enough, the business would move. Then I started my own company and learned the truth within about six months:

The bottleneck isn't skill. It's coordination.

Founders and operators don't get to do one thing. You are product, engineering, marketing, sales, operations, support, and lately a full-time terminal wrangler. Every serious builder I know carries the same constellation of half-open conversations: Claude Code running in one terminal tab, Devin running in another, Cursor in an editor, a design brief living in a chat, an n8n webhook half-configured, and a spreadsheet where task status went to die. Output arrives without context. No one can tell you where a decision came from or whether it was reviewed. And the moment an AI result actually matters — the one that touches production code, goes to a customer, or spends real money — you realize you can't point to its source, you can't pause it mid-flight, and you can't explain to anyone else why it should be trusted.

We kept watching each other hit that wall. Eventually we had to admit we were the wall.

### The struggle: doing everything, trusting nothing

Let me be specific about what the struggle actually felt like, because it's not the polished version of the story.

It was 2 a.m. and I was moving a deliverable between a terminal window where Claude Code was running, a chat thread where the brief lived, and a spreadsheet where task status went to die. My co-founder and I had built the same feature in parallel the week before, because we each started from a different conversation and neither of us had a single place to look. We were running a company with the operational clarity of a thirty-tab browser.

The CLI agents weren't bad. That's the frustrating part. Claude Code, Codex, and Cursor CLI were genuinely powerful. But a business is not a single prompt, and these tools were built to execute isolated tasks, not to coordinate with each other or run continuous operations. None of them shared state. None of them let agents talk to each other to resolve conflicts. None of them could reference a single folder of company docs as shared truth. And none of them provided a safety net before a destructive command executed. The interface was always raw terminal tabs — you had to be the coordination layer, switching between windows, copying context, babysitting output.

So the real cost of "AI doing the work" was that we were coordinating the output of ten tools by hand. We had traded the work for more work — the coordination work. And the interface was the problem: raw terminals, not a place where a founder could direct work in plain language.

### The insight: four ideas that refused to leave us alone

The turning point wasn't a single epiphany. It was four ideas that kept showing up in every argument we had about how to fix it:

**First, manage CLI agents — don't build another LLM wrapper.** The world doesn't need another generic AI chat or another hosted model wrapper. It needs a desktop platform that manages real CLI agents — Claude Code, Codex, Cursor, Devin, Hermes, Pi — through local terminals, keeping model keys and inference direct between the user and their provider. And it needs to put those agents behind a Slack-style channel interface — not raw terminal tabs — so founders and operators can direct work in plain language without terminal fluency.

**Second, agents collaborate in channels with a Knowledge Vault and business roadmap.** Instead of running isolated agent silos, agents should communicate in Slack-like channels to debate approaches and delegate sub-tasks. And every agent should reference a shared **Knowledge Vault** — a folder of documents you drop in that serves as the single source of truth for the entire company — plus a business roadmap so agents never drift off context. Smart agents immediately know what and when each one needs to do; users don't orchestrate manually.

**Third, the UI is event-driven and adaptive.** Work should trigger on events — a task completing, a budget threshold approaching, an approval gate opening — not manual polling. And the interface should learn from user behaviors, preferences, and operational patterns over time, becoming more personalized and more useful with every run. No more babysitting terminal windows.

**Fourth, built to build AND run 24/7.** For software engineering, agents run in isolated git worktrees so parallel changes never collide. For operations, persistent daemons run 24/7 workflows — customer support triage, ecommerce bots, YouTube content pipelines, HR intake — connecting to 400+ SaaS tools through a native n8n plugin.

**Fourth, approval gates as a default — not a setting.** Consequential actions pause until a human reviews them. The plan is reviewed before the run. The diff is reviewed before the merge. The spend is capped before the job starts. The founder decides what moves and what waits — that's not a feature, it's the product.

### The build: starting as our own worst users

We built Fabrica the way founders build most things that work: we started by fixing our own workflow.

The first version was a chat wrapper. It failed — no state, no visibility, no way to stop it when it went sideways.
The second version was a sequential pipeline. It failed — because orderliness on a single track just means everything moves at the speed of the slowest step.
The third version is the one we kept: a desktop platform managing parallel CLI agents, a Slack-style channel interface instead of raw terminal tabs, agent collaboration channels, a shared knowledge vault, isolated worktrees, and visual approval gates. The UI is event-driven — work triggers on completions, budgets, and gates, not manual polling. And it adapts to how you work over time.

And we made a name decision that took longer than it should have. The project started under a codename: Orca. It stuck for months, until we said it out loud and heard what it meant — a hunter, a solitary predator moving alone through dark water. That is not what we were building. We renamed it Fabrica, from the Latin for workshop, the foundry, the place where raw material becomes something finished through craft and coordination.

### The vision: the next AI exit

"The Next AI Exit" is our name for that transition — the move from doing every task to directing and operating the work. It's the exit from the bottleneck.

Judgment is the point of being a founder; it's the last thing you should automate. What you can and should automate is the coordination — the routing, the state, the handoffs, the 24/7 execution. Fabrica's bet is that the founders and operators who win the next generation aren't the ones with the best prompts. They're the ones who build the operating layer: a clear brief for every job, visible work, an approval gate where it counts, a budget that holds.

Your business, automated. Your judgment, still in the loop.

---

## Version 2 — LinkedIn (800–1200 words)

# We Built Fabrica Because We Were the Bottleneck

We kept failing at our own startup in a way nobody warns you about. Not the product. Not the market. Coordination.

My co-founder and I were juggling terminal windows with Claude Code, Cursor CLI, and Devin alongside product, marketing, sales, and ops. Each tool was smart in isolation and useless together. A plan in one chat. Status in a spreadsheet no one could keep updated. Output from an agent that had "handled" something we still couldn't verify.

So we built the thing we couldn't find anywhere: a desktop platform to manage our CLI agents and run our operations with total control — with a Slack-style channel interface instead of raw terminal tabs.

Four ideas shaped it:
1. **Manage CLI agents directly:** Run Claude Code, Cursor, Devin, Hermes, and Pi in local terminals with your own keys — zero LLM markup. The interface is a Slack-style channel, not raw terminal tabs.
2. **Agent collaboration channels & Knowledge Vault:** Agents debate in dedicated channels and reference a shared document vault and business roadmap as their source of truth. Smart agents know what to do and when — no manual orchestration needed.
3. **Event-driven & adaptive UI:** Work triggers on events (task completions, budget thresholds, approval gates), not manual polling. The interface learns from your behaviors and adapts over time.
4. **Build software & run 24/7 operations:** Isolated git worktrees for engineers, plus 24/7 continuous operations (customer support, ecommerce, content) with 400+ SaaS automations via n8n.
5. **Approval gates as a default:** Diff reviews, hard budget caps, and visual sign-offs before any consequential action runs.

We call this **The Next AI Exit** — the moment a founder or operator moves from doing every task by hand to directing and operating agent crews.

Early access is open. Come tell us where it breaks.

---

## Version 3 — Twitter/X Thread (10 tweets)

1. We built Fabrica because we kept failing at our own startup in a way nobody warns you about. Not the product. Not the market. Coordination. Thread on the whole story. 🧵

2. We were juggling raw terminal tabs with Claude Code, Cursor, and Devin — while running product, marketing, and ops. Each tool was powerful in isolation, but they had no shared context and couldn't collaborate.

3. The tools weren't bad. But a business isn't a single prompt. It's a crew of jobs that need to move in parallel, share context, and respect the judgment of the person who owns the outcome.

4. So we built the desktop platform we wished existed. Four ideas shaped it:

5. One: Manage CLI agents via local terminals. Run Claude Code, Cursor, Devin, and others with your own direct keys. We never touch or mark up inference.

6. Two: Agent collaboration channels & Knowledge Vault. Agents talk to each other in Slack-like channels and reference your dropped documents as shared truth.

7. Three: Build code & run 24/7 operations. Isolated git worktrees for developers, plus 24/7 customer support, ecommerce, and content pipelines via our native n8n plugin.

8. Four: Approval gates as defaults. Consequential actions pause for visual diff review and budget sign-off. Autonomy for execution; authority stays with you.

9. We renamed it from Orca to Fabrica (Latin for foundry/workshop) because it's not about a solitary predator — it's about a well-run operating floor where you keep the call.

10. That's our whole bet: The Next AI Exit. From doing every task yourself to directing the crew. Early access is open — come break it: https://fabrica-ai.vercel.app