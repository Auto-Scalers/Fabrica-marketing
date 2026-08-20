# The Founder's Bottleneck: The Fabrica Founder Story

Three versions of the founding narrative, built on the same arc:

1. **Struggle** — the frustration of running a business with scattered AI tools
2. **Insight** — parallel agents, approval gates, builders command instead of code
3. **Build** — how we started, what failed, the decisions we kept
4. **Vision** — where Fabrica goes and what "The Next AI Exit" means

Founder voice throughout: direct, grounded, technical-but-accessible, anti-hype.

---

## Version 1 — Blog Post (1500–2000 words)

# From Doing Every Task to Directing the Work: The Fabrica Story

I spent the first part of my career convinced the bottleneck was skill. Write better code. Learn more frameworks. Ship faster. If I was competent enough, the business would move. Then I started my own company and learned the truth within about six months:

The bottleneck isn't skill. It's coordination.

Founders don't get to do one thing. You are product, marketing, sales, operations, support, and lately a full-time AI wrangler. Every serious founder I know carries the same constellation of half-open conversations: a design brief living in one chat, a market analysis in another, a code change in a copilot, a browser agent that supposedly "handled" something on Tuesday that nobody can confirm actually happened. Output arrives without context. No one can tell you where a decision came from or whether it was reviewed. And the moment an AI result actually matters — the one that goes to a customer, or the one that moves money — you realize you can't point to its source, you can't pause it mid-flight, and you can't explain to anyone else why it should be trusted.

We kept watching each other hit that wall. Eventually we had to admit we were the wall.

### The struggle: doing everything, trusting nothing

Let me be specific about what the struggle actually felt like, because it's not the polished version of the story.

It was 2 a.m. and I was moving a deliverable between a chat thread where the plan lived, a spreadsheet where the task status went to die, and a tool that had produced output I could not trace back to any input I remembered giving it. My co-founder and I had built the same feature in parallel the week before, because we each started from a different conversation and neither of us had a single place to look. We were running a three-person company with the operational clarity of a thirty-tab browser.

The tools weren't bad. That's the frustrating part. Each one was good at its own narrow job. The copilot was genuinely helpful. The chat models were genuinely smart. The browser agents were genuinely ambitious. But a business is not a task, and these tools were built to complete tasks, not to run work. None of them shared state. None of them let us see what was moving, what was waiting, and what needed a human decision. None of them could tell us what a run had cost before it had already spent it.

So the real cost of "AI doing the work" was that we were coordinating the output of ten tools by hand. We had traded the work for more work — the coordination work. We were the ones holding the invisible seams together, and nothing told us when a seam was about to tear.

### The insight: three ideas that refused to leave us alone

The turning point wasn't a single epiphany. It was three ideas that kept showing up in every argument we had about how to fix it, until we finally admitted they were the answer.

**First, parallel agents — not parallel chats.** A copilot helps one person write code. A chat model answers one person's questions. But a founder needs a crew of jobs moving at once: research, build, market, sell, support. Each job deserves a clear brief and its own isolated workspace, so parallel work doesn't collide the way our two versions of the same feature collided. Distributed teams solved this problem decades ago — you keep parallel changes in separate branches, in separate worktrees, and merge deliberately. We decided agent work deserved the same discipline. Give each specialist its own workspace. Let them run in parallel. Merge what's ready and review what's not.

**Second, approval gates as a default — not a setting.** The reason founders don't trust agents isn't that agents are dumb. It's that when the stakes get real, nobody wants to discover what a model decided to do on its own. The answer isn't more trust; it's better structure. So we made control structural: a consequential step pauses until a human reviews it. The plan is reviewed before the run. The diff is reviewed before the merge. The spend is bounded before the job starts. The founder decides what moves and what waits — that's not a feature, it's the product. We never wanted to be the tool that says "we'll handle everything." We wanted to be the tool that makes it genuinely easy to say "here's what you handle, and here's where I decide."

**Third, builders command — they don't script.** The phrase "no-code" always felt patronizing to us, because it assumed non-technical people are too fragile for a command line. What founders actually need is to direct work in plain language and still have technical detail available when they want it. Write a brief like you'd brief a contractor: here's the job, here's the context, here's the standard for done. Review the plan. Approve the run. The technical layer — diffs, commands, worktrees, isolated environments — stays one level down, visible to the people who want to verify it and invisible to the people who just want it to move. And because you bring your own model keys, Fabrica is the workshop and your providers are the fuel: no opaque credit meters, no bundled tokens you can't audit, no billing maze between you and what a run actually costs.

These three ideas became the operating shape of the product. Brief the crew. Review the plan. Approve the run. Ship the output.

### The build: starting as our own worst users

We built Fabrica the way founders build most things that work: we started by fixing our own workflow, and we were our own first users, which meant our own first victims.

The first version was a chat wrapper. We gave a model a long prompt with instructions and crossed our fingers. It failed exactly the way everything we were running from failed — no state, no visibility, no way to stop it when it went sideways. A wrapper around the problem is not a solution to the problem; it's the problem with a new coat of paint. We threw it away.

The second version was a sequential pipeline. Every job waited for the one before it. It was orderly, legible, and useless — because orderliness on a single track just means everything moves at the speed of the slowest step. A founder who can only run one job at a time is still a founder who is the bottleneck, and we were trying to stop being the bottleneck.

The third version is the one we kept, and it started with the failures. We kept the discipline we'd learned the hard way and rebuilt around three rules:

- **If the work can't be seen, it can't be trusted.** Every run has a visible state — running, waiting, ready for review. Work is organized as tasks and outputs, not buried in scattered conversations.
- **If control is optional, it won't be used.** Approval gates and budget limits are defaults, not toggles you have to discover. The safe default is that consequential work waits for a human.
- **If you can't audit cost, you can't budget.** Bring your own keys. Pay your providers directly for inference. See what a run costs before it runs, and set a hard stop for when it must not run past.

And we made a name decision that took longer than it should have. The project started under a codename: Orca. It stuck for months, until we said it out loud and heard what it meant — a hunter, a solitary apex predator, moving alone through dark water. That is not the product we were building. We renamed it Fabrica, from the Latin for workshop, the foundry, the place where raw material becomes something finished through heat and craft and hands that know what they're doing. The forge language matched the product better than any predator ever could. Fabrica is warm, industrial, and in motion — a place where work is built, and where the person running the forge keeps the call.

We're still early. Early access means integrations are still expanding, and we'll say so plainly as we go. We have not shipped a finished product; we have shipped a direction we believe in and a set of defaults we're willing to defend. Every feature has been built because we saw a founder — usually ourselves — lose context, or lose control, or lose money on a run that had no guardrail. Those are the failures we're still building against, and we expect there are more of them we haven't met yet.

### The vision: the next AI exit

Here's where we think this goes, and why we put "The Next AI Exit" on the box.

There are two exits in a founder's life. The one everyone talks about is the liquidity event — the sale, the acquisition, the IPO, the moment the years of work convert into something you can hold. The one nobody frames as an exit is smaller and, for most of us, arrives much earlier: the moment you stop being the person who does every task yourself.

That second exit is the one AI is finally making real, and it's the one we care about.

"The Next AI Exit" is our name for that transition — the move from doing every task to directing the work. It's the exit from the bottleneck. The exit from the thirty-tab browser and the spreadsheet where status goes to die and the output you can't trace. It's the exit from being the constraint that keeps your own business from moving faster than you can personally type, write, and decide.

We're not talking about a black box that runs your company while you sleep. We don't think that's real, and we don't think it's healthy even in the version where it's real. Judgment is the point of being a founder; it's the last thing you should automate. What you can and should automate is the coordination — the routing, the state, the handoffs, the busywork of moving work from one tool to another and one person to another. Fabrica's bet is that the founders who win the next generation aren't the ones with the best prompts. They're the ones who build the operating layer: a clear brief for every job, visible work, an approval gate where it counts, a budget that holds. A company that can outrun its founder, because it finally has more than one set of hands and a single place to direct them.

That's where Fabrica goes. Not toward more autonomy for its own sake, but toward a more capable version of what a founder-run company already is: a crew with a route and a review point for every consequential move. Your business, automated. Your judgment, still in the loop.

We built this because we were the bottleneck, and we wanted out. If you've ever been the bottleneck, you know exactly what we mean — and we built the door for you too.

---

## Version 2 — LinkedIn (800–1200 words)

# We Built Fabrica Because We Were the Bottleneck

We kept failing at our own startup in a way nobody warns you about. Not the product. Not the market. Coordination.

My co-founder and I were running product, marketing, sales, ops, and support — and increasingly, a pile of AI tools that were each smart in isolation and useless together. A plan in one chat. Status in a spreadsheet that no one could keep updated. Output from a browser agent that had "handled" something we still couldn't verify. We built the same feature twice in parallel one week, because each of us started from a different conversation and neither of us had one place to look.

The tools weren't bad. That was the frustrating part. They were good at tasks. But a business isn't a task — it's a crew of jobs that need to move in parallel, stay visible, and respect the judgment of the person who owns the outcome. We were spending more time holding the seams between tools together than actually doing the work. We had automated the tasks and kept the coordination.

So we built the thing we couldn't find anywhere: a command center for directed agent work.

Three ideas shaped it, and I'll keep them short.

**Parallel agents, not parallel chats.** A copilot helps one person code. A chat model answers one person. A founder needs research, build, market, sell, and support moving at once. Each job gets a clear brief and its own isolated workspace — the same discipline distributed teams use for parallel code changes, applied to all the work. Specialists run in parallel. They don't collide. We merge what's ready and review what's not.

**Approval gates as a default, not a setting.** Founders don't distrust agents because agents are dumb. They distrust the moment they realize no human signed off on something consequential. So control is structural here: a plan is reviewed before a run, a diff before a merge, a spend capped before it starts. The founder decides what moves and what waits. That's not a feature — it's the product.

**Builders command; they don't script.** Write a brief in plain language, like you'd brief a contractor: the job, the context, the standard for done. Review the plan. Approve the run. Technical detail — diffs, commands, worktrees — stays one level down for the people who want to verify it. And you bring your own model keys. Fabrica is the workshop; your providers are the fuel. No opaque credit meters, no bundled tokens you can't audit.

The build story is mostly failure, which I think is the honest part. The first version was a chat wrapper — a smarter prompt around the same broken workflow, and it failed the same way. The second was a sequential pipeline — orderly, legible, and useless, because a single track just means everything moves at the speed of the slowest step. We were trying to stop being the bottleneck, and both versions quietly kept us in the middle of it.

The third version is the one we kept, and it's built on rules we earned the hard way: if the work can't be seen, it can't be trusted. If control is optional, it won't be used. If you can't audit cost, you can't budget.

One more decision worth naming: the name. The project started as Orca. We kept it until we heard what it meant — a solitary hunter moving alone through dark water. That's not the thing we were building. We renamed it Fabrica, from the Latin for workshop, the foundry, where raw material becomes something finished through heat, craft, and hands that know what they're doing. The person running the forge keeps the call. That's the whole philosophy in a name.

We're still early. Early access means integrations are still expanding, and we'll say so plainly. This isn't a finished product; it's a direction we believe in and a set of defaults we're willing to defend.

Which brings me to the tagline you'll see on us: **The Next AI Exit.**

There are two exits in a founder's life. The one everyone talks about is the liquidity event. The one nobody frames as an exit is the moment you stop being the person who does every task yourself. That's the exit AI is finally making real, and it's the one we care about.

We don't mean a black box running your company while you sleep. We don't think that's real, and it's not healthy in the version where it is. Judgment is the point of being a founder — it's the last thing you should automate. What you should automate is the coordination: the routing, the state, the handoffs, the busywork of moving work between tools and people. The founders who win the next generation aren't the ones with the best prompts. They're the ones who build the operating layer — a clear brief for every job, visible work, an approval gate where it counts, a budget that holds.

That's where Fabrica goes: not toward more autonomy for its own sake, but toward a more capable version of what a founder-run company already is. A crew with a route and a review point for every consequential move. Your business, automated. Your judgment, still in the loop.

We built this because we were the bottleneck and we wanted out. If you've ever been the bottleneck — and if you're a founder, you have — we built the door for you too.

Early access is open. We'll be candid about what works, what doesn't, and where we're breaking it next. Come find us, or tell us where it should break first.

---

## Version 3 — Twitter/X Thread (10 tweets)

1. We built Fabrica because we kept failing at our own startup in a way nobody warns you about. Not the product. Not the market. Coordination. Thread on the whole story. 🧵

2. We were running product, marketing, sales, ops — and a pile of AI tools that were each smart in isolation and useless together. A plan in one chat. Status in a spreadsheet no one could keep up. Output we couldn't trace back to any input we gave it.

3. The tools weren't bad. That's the frustrating part. They were great at tasks. But a business isn't a task. It's a crew of jobs that need to move in parallel, stay visible, and respect the judgment of the person who owns the outcome.

4. So we built the thing we couldn't find anywhere: a command center for directed agent work. Three ideas shaped it.

5. One: parallel agents, not parallel chats. A copilot helps one person code. A founder needs research, build, market, and support moving at once. Each job gets a clear brief and its own isolated workspace. They run parallel. They don't collide.

6. Two: approval gates as a default, not a setting. Founders don't distrust agents because agents are dumb. They distrust the moment nobody signed off on something that mattered. So control is structural: review the plan before the run. Review the diff before the merge. Cap the spend before it starts.

7. Three: builders command, they don't script. Brief the crew in plain language. Technical detail stays one level down for whoever wants to verify it. And you bring your own model keys — the workshop is Fabrica, the fuel is your providers. No opaque credit meters.

8. The build story is mostly failure. V1 was a chat wrapper — a smarter prompt around the same broken workflow. V2 was a sequential pipeline — orderly, legible, useless. Both kept us in the middle of the bottleneck we were trying to escape. V3 is the one we kept.

9. We started calling it Orca, then heard what that meant: a solitary hunter moving through dark water. Not what we're building. We renamed it Fabrica — from the Latin for workshop, the foundry, where raw material becomes something finished through craft. The person running the forge keeps the call.

10. That's our whole bet, and it's on the box: The Next AI Exit. Not the liquidity kind — the exit from being the person who does every task yourself. Judgment stays with the founder. The coordination gets automated. Brief the crew. Review the plan. Approve the run. Ship the output. Early access is open — come break it.