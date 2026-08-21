# Fabrica Brand Guidelines

> **The Next AI Exit**
>
> A practical system for anyone making Fabrica work: designers, writers,
> product teams, founders, and partners.

## 1. Brand at a glance

Fabrica is a desktop platform that manages CLI agents — Claude Code, Codex,
OpenCode, Cursor, Devin, and others — through local terminals. Founders and
operators set the brief; Fabrica spawns the right agents, routes work across
parallel sessions, gates consequential steps behind human approval, and caps
spend at a hard limit. Agents collaborate with each other in dedicated channels,
share knowledge from a central document vault, and can run operations
continuously — customer support, content pipelines, ecommerce management — not
only build software.

### Business-first UI

Fabrica transforms the raw CLI terminal experience into a Slack-style
conversation interface. Instead of juggling terminal tabs and raw command output,
founders and operators interact with agents through dedicated channels — each
channel is a workspace where agents discuss approaches, delegate sub-tasks, and
report progress in plain language. The interface is agentic and event-driven:
work happens in response to events (a task completing, a budget threshold
approaching, an approval gate opening), not through manual polling or tab
switching.

Over time, the UI adapts. It learns from user behaviors, preferences, and
operational patterns to surface the most relevant views, surface priority alerts,
and surface the controls that matter most. The more a founder uses Fabrica, the
more the interface reflects how they actually work — not a one-size-fits-all
layout, but a living system that gets more personalized and more useful with
every run.

### Brand feel

The brand should feel like a modern operating floor: precise, alive, and in
motion. Use the forge/foundry metaphor to communicate craft and momentum; use
the platform metaphor to communicate coordination at scale. Neither should
become costume or science fiction.

| We are | We are not |
| --- | --- |
| Direct and specific | Loud or breathless |
| Technical, then understandable | Jargon-first |
| Founder-led and accountable | Faceless corporate software |
| Ambitious with evidence | Promising magic |
| Warmly industrial | Rustic, steampunk, or dystopian |

### Core audience

- Technical founders and solo builders who need to ship more than one thing at once.
- Lean teams that need more capacity without losing review and accountability.
- Non-technical entrepreneurs who want to direct work in plain language and see what happens next.
- Operators and business managers who run continuous agent workflows — customer support, ecommerce, content, HR — without necessarily building new software.

### Brand promise

**Your business, automated. Your judgment, still in the loop.**

This is the operating idea behind all Fabrica communication. Do not imply that
Fabrica removes responsibility; it helps a founder direct it at a higher level.

---

## 2. Visual identity

### 2.1 Logo

Use the approved Fabrica logo artwork only. Do not redraw, typeset a replacement,
trace it, apply effects, or alter its proportions. Until the final asset package
is published, use the Fabrica wordmark as plain text only in working documents;
do not invent a logo mark.

#### Clear space

Keep clear space on every side equal to the height of the lowercase **a** in the
wordmark. No type, image edge, rule, or UI control may enter this area.

```text
      ┌──────────────────────────────────┐
      │              clear space           │
      │   [clear]  FABRICA  [clear]        │
      │              clear space           │
      └──────────────────────────────────┘
```

#### Minimum size

| Format | Wordmark | Symbol (when supplied) |
| --- | ---: | ---: |
| Screen | 96 px wide | 24 px wide |
| Print | 25 mm wide | 7 mm wide |
| Favicon/app tile | Do not use the wordmark | 16 px minimum |

If the wordmark is smaller than the stated minimum, use the approved symbol or
write the name in the accompanying text instead.

#### Color variations

| Background | Preferred logo | Use when |
| --- | --- | --- |
| Forge Dark or other dark surface | White/Steel Light | Default digital and product use |
| White or warm paper | Forge Dark | Print, documents, light pages |
| Molten Orange | Forge Dark | Short, high-energy promotional moments only |
| Photograph/texture | Solid logo on a clean overlay | The image has enough quiet contrast |

Never place the logo directly on a busy image, use an unapproved gradient fill,
outline it, add a shadow, rotate it, stretch it, or make it smaller than the
minimum. Use one logo color at a time.

### 2.2 Color palette

The palette begins in darkness and uses heat sparingly. Molten Orange is an
instruction, an emphasis, or a moment of progress—not wallpaper.

| Token | Value | Role | Typical use |
| --- | --- | --- | --- |
| **Forge Dark** | `#16171A` | Primary | Primary canvas, wordmark on light, dark type |
| Forge Surface | `#22242A` | Supporting dark | Panels, cards, deep image overlays |
| Forge Edge | `#343842` | Boundary | Dividers, restrained borders, inactive UI |
| **Molten Orange** | `#E8590C` | Accent | Primary actions, key emphasis, progress |
| Molten Light | `#FF8A3D` | Highlight | Gradient start, hover/highlight, data emphasis |
| Molten Ember | `#B94308` | Deep accent | Active/pressed states, print emphasis |
| **Steel Gray** | `#8F939E` | Secondary | Supporting labels, diagrams, secondary type on dark |
| Steel Light | `#C2C6CC` | Light neutral | Subheads, borders on dark, quiet type |
| Steel Deep | `#5E636D` | Dark neutral | Secondary UI and structure |
| Paper | `#FAF7F0` | Light canvas | Documents, light-mode campaigns |
| Ink | `#292725` | Light-mode type | Text on Paper |

The product web implementation uses `#E8590C` as its primary molten copper/amber
token and `#FF8A3D → #E8590C` for its molten gradient. Treat those values as
canonical for digital assets.

#### Color rules

- Use Forge Dark as the dominant field on dark work (about 70–80% of the frame).
- Use Steel Gray to organize, label, and recede; it should not compete with a CTA.
- Use Molten Orange once per decision point. A page with five orange actions has no primary action.
- On dark surfaces, use white or Steel Light for long-form text—never Molten Orange.
- On Paper, use Forge Dark or Ink for body text and reserve orange for links, actions, and highlights.
- Meet WCAG AA contrast at minimum; do not place small orange text on Forge Dark without testing contrast.

**Correct:** a Forge Dark launch visual with one orange CTA and steel-gray metadata.

**Incorrect:** orange body copy, orange borders, orange icons, and orange buttons in the same view.

### 2.3 Typography

Fabrica typography is clear before it is distinctive. The current web product
uses **Geist** and **Geist Mono**; use them whenever available.

| Job | Primary family | Weight/style | Rules |
| --- | --- | --- | --- |
| Display/headlines | Geist | 700–800 | Compact, declarative, sentence case by default |
| Subheads | Geist | 600–700 | Explain the promise; avoid stacked abstractions |
| Body | Geist | 400–500 | 16–18 px screen equivalent; generous line height |
| Navigation/meta | Geist | 500–600 | Small labels may be uppercase with tracking |
| Commands, paths, technical proof | Geist Mono | 400–500 | Use only for literal strings or system evidence |

Fallback stack: `Arial, Helvetica, sans-serif` for Geist; `Consolas, monospace`
for Geist Mono. Do not substitute display serif faces, condensed novelty faces,
or generic "tech" fonts.

#### Type in action

```text
BUILD THE WORK. KEEP THE CONTROL.     Geist 800
Direct a crew. Review every move.     Geist 600
Fabrica gives founders a visible...   Geist 400
$ fabrica run growth-audit            Geist Mono 400
```

Use short, forceful headlines. Never set entire paragraphs in all caps. Keep
line lengths readable (roughly 45–75 characters for body copy).

### 2.4 Imagery, illustration, and motion

The visual world is a **digital foundry**, not a literal one. Favor interfaces,
work in progress, systems diagrams, material texture, and controlled warmth.

**Use:**

- Dark command-center screens, with honest product UI and visible task states.
- Close crops of purposeful work: notes, diagrams, code, review queues, and founder decisions.
- Subtle grain, metal, graphite, blueprint, or heat-light texture at low opacity.
- One warm source of light or orange signal against a mostly dark composition.
- Motion that indicates progress: routing lines, status changes, task completion, and review gates.

**Avoid:**

- Generic robots, brains, glowing humanoids, or stock people looking at laptops.
- Literal flames, anvils, sparks, or medieval/steampunk machinery.
- Neon rainbow gradients, glossy 3D blobs, and fake terminal output.
- Screenshots with unreadable microtext or fabricated metrics/testimonials.

For social images, start with Forge Dark, a concise claim, a product/workflow
visual, and one Molten Orange focal point. Keep the lower-right corner clear
when a platform may add UI overlays.

#### Signature visual element: Forge Pulse

Every major Fabrica touchpoint — product UI, marketing, and social — must
include the **Forge Pulse**: a subtle animated ring or heat-ripple in Molten
Orange (`#E8590C`) that appears on any active or running agent card. It
communicates that something is working — alive and in motion. This is the one
visual detail a person who uses Fabrica once should always remember. Apply it
consistently to active-agent states only; never use it on idle, paused, or
completed cards. Do not over-animate; the pulse should be calm and purposeful,
not distracting.

---

## 3. Voice and tone

### 3.1 Voice: constant characteristics

Fabrica speaks as a capable builder beside another builder. The voice stays:

- **Direct:** lead with what changes, not a scene-setting claim.
- **Commanding:** use active verbs and make the next step obvious.
- **Builder-first:** respect technical detail and real constraints.
- **Accessible:** translate the system into plain language before adding terms of art.
- **Grounded:** state limits, prerequisites, and evidence plainly.

Prefer active construction: “Review the plan before it runs,” not “The plan can
be reviewed prior to execution.” Be concise, but not cold.

### 3.2 Tone by context

| Context | Tone | What it sounds like |
| --- | --- | --- |
| Marketing | Confident, vivid, outcome-led | “Direct the crew. Keep the call.” |
| Product/UI | Brief, calm, decisive | “3 tasks need review.” |
| Support | Patient, specific, accountable | “That job paused at the approval gate. Here’s how to resume it.” |
| Technical docs | Exact, neutral, transparent | “Each agent runs in an isolated worktree.” |
| Founder/community | Candid, human, learning in public | “We changed this after watching founders lose context between tools.” |
| Incident/update | Plain and timely | “Runs created between 14:10–14:32 UTC may not have started. We’re replaying them.” |

### 3.3 Do and don’t

| Do | Don’t |
| --- | --- |
| Name the job and the control point. “Assign research, review the plan, then approve the run.” | Hide the mechanism. “Let the platform handle everything.” |
| Make a claim that can be demonstrated. “Run specialized tasks in parallel, each in its own worktree.” | Use vague superlatives. “The ultimate future of work.” |
| Speak founder-to-founder. “You decide what moves and what waits.” | Patronize. “Even non-technical users can finally understand AI.” |
| Describe agents as tools with scope. “Give the marketing agent a brief and an approval gate.” | Give agents mystical agency. “Your autonomous workforce thinks for you.” |
| Be candid about unfinished work. “Early access; integrations are still expanding.” | Manufacture certainty. “Flawless automation from day one.” |

### 3.4 Word bank

Use these words when they accurately describe the product:

**Direct, platform, crew, build, ship, run, operate, review, approve, route,
visible work, workflow, worktree, channel, knowledge vault, guardrail, budget,
checkpoint, brief, output, momentum, capacity, founder, builder, operator,
control.**

Use “agent” as a clear functional noun, not as a synonym for magic. Define any
specialized technical term on first use for non-technical audiences.

### 3.5 Blacklist and cautions

Never use these terms in Fabrica copy:

- “AI-powered”
- “revolutionary”
- “game-changing”

Also avoid “seamless,” “effortless,” “magic,” “set it and forget it,” “10x,” and
"replace your team" unless a carefully qualified, evidence-based context makes
their use unavoidable. Do not call Fabrica an IDE unless the audience and claim
are specifically about its coding environment; broadly, it is a desktop platform with Slack-style channels
for directed agent work.

---

## 4. Messaging framework

### 4.1 Tagline

**The Next AI Exit**

Use it as a perspective, not an unexplained slogan. In first-touch marketing,
pair it with a clarifier such as: “From doing every task to directing the work.”

### 4.2 Elevator pitches

| Length | Copy |
| --- | --- |
| 10 words | **Fabrica runs your AI agents. You keep the control.** |
| 30 words | **Fabrica is a desktop platform that manages Claude Code, Codex, OpenCode, Cursor, Devin, and other CLI agents across business and coding work — with visible approval gates, budget limits, and 24/7 operations.** |
| 60 words | **Fabrica gives founders and operators one place to manage specialist CLI agents across any business task — research, building, marketing, customer support, or operations. Set a brief, let agents collaborate in dedicated channels and reference a shared knowledge vault, review the work, approve what matters, and keep hard budget limits in place. Agents run in your terminals, on your machine, with your provider keys — never through Fabrica.** |

### 4.3 Messaging hierarchy

1. **Primary:** Direct the work; keep the control.
2. **Outcome:** Build more, run more, and grow more — without becoming the coordination bottleneck.
3. **Mechanism:** Fabrica manages CLI agents (Claude Code, Codex, Cursor, Devin, and others) through local terminals. Agents collaborate in dedicated channels and reference a shared knowledge vault and business roadmap — your document source of truth for the entire operation. Smart agents immediately know what and when each one needs to do; users don't orchestrate manually.
4. **Guardrails:** Approval gates, hard budget caps, and spend tracking (where the CLI agent exposes it) keep the founder in charge of every consequential action. Agents propose; you approve. Nothing moves past a gate without you.
5. **Audience:** Built for founders building products and operators running businesses — solo builders, lean teams, project managers, and agencies.

### 4.4 Value propositions

| Pillar | Claim | Supporting explanation |
| --- | --- | --- |
| More capacity | Run multiple CLI agents in parallel — building and operating at once. | Fabrica manages Claude Code, Codex, Cursor, Devin, and others simultaneously across coding, research, marketing, and ops sessions. |
| Visible control | See what every agent is doing, waiting on, or ready to hand off. | Work is organized as tasks and agent sessions — not buried in terminal windows or scattered chat logs. |
| Safer delegation | Set approval gates, budget ceilings, and risk tiers on every consequential action. | Agents propose; you approve. Hard budget stops at your defined limit. No black-box autonomy. |
| Better handoffs | Context, documents, and briefs travel with the work. | A shared knowledge vault and business roadmap give every agent the same source of truth — no re-explanation between sessions or agents. |
| Built for builders and operators | Keep deep technical power available while enabling non-technical operators to run continuous workflows. | Fabrica supports isolated coding worktrees for builders and 24/7 runtime operations — customer support, content pipelines, ecommerce management — for operators. |


### 4.5 Message patterns

Use these as starting points, then replace bracketed terms with a real workflow:

- **Problem → turn:** "You are still the bottleneck between [brief] and [result]. Fabrica gives that work a crew, a route, and a review point."
- **Control:** "Let [agent/task] move. Keep [approval/budget/decision] with you."
- **Workflow:** "Brief [specialist]. Review the plan. Approve the run. Ship the output."
- **Proof-led:** "In [workflow], Fabrica shows [observable event] and requires [specific control] before [consequential action]."
- **Runtime:** "[Agent] is running [workflow] continuously. [Metric or event] will trigger your next approval."
- **Platform scope:** "Fabrica manages [Claude Code / Cursor / Devin]. Your provider keys go to [provider] directly — never through Fabrica."

---

## 5. Proof and social proof

### 5.1 Evidence standard

Every material product claim needs one of these behind it: a demonstrable workflow,
a product screenshot/video, an instrumented metric, a customer quote approved for
use, or a clearly labeled founder perspective. Never invent user counts, time
savings, customer logos, benchmark results, or quotes.

| Claim type | Acceptable proof | Avoid |
| --- | --- | --- |
| Product capability | Screenshot, demo, documentation | “Works while you sleep” without showing scope/controls |
| Time/capacity | Measured before/after and method | Unqualified “10x faster” |
| Customer outcome | Named/approved quote with context | Anonymous praise presented as a case study |
| Reliability/control | Clear behavior and limit | “Fully autonomous” |

### 5.2 Social-proof templates

**Customer quote**

> “Before Fabrica, [specific bottleneck]. Now we [specific workflow], and I
> still [control or result].”
>
> — [Full name], [role] at [company], used with permission

**Workflow proof card**

```text
[Workflow name]
Brief: [what was assigned]
Control: [approval gate, budget, or review]
Output: [what was delivered]
Evidence: [link to demo, screenshot, or case study]
```

**Founder proof post**

> We built [feature] because [specific observed problem]. In the first version,
> it [observable behavior]. Next, we are measuring [metric/learning].

**Early-access metric**

> “[Number] founders joined early access to test [specific workflow] as of
> [date].”

Only publish the metric after it is verified, dated, and owned by the team.

---

## 6. Ready-to-use examples

### Landing-page hero

**Headline:** Direct the crew. Keep the call.

**Body:** Fabrica helps founders put focused business and coding work in motion,
then review the decisions that matter.

**CTA:** See the Slack-style interface

### Product status message

**Correct:** “Growth audit is ready for review. Approve the plan to start the run.”

**Incorrect:** “Your AI workflow has intelligently completed its autonomous cycle.”

### Support reply

**Correct:** “The task is waiting at its approval gate. Open the run, review the
proposed plan, then select Approve to continue. If the plan is wrong, edit the
brief and rerun it.”

**Incorrect:** “Don’t worry—our intelligent system will take care of it.”

### Technical-documentation introduction

**Correct:** “Fabrica can run coding tasks in isolated worktrees so parallel
changes do not share the same working directory. Review each output before merge.”

**Incorrect:** “Fabrica’s revolutionary multi-agent architecture transforms
development forever.”

---

## 7. Pre-publish checklist

Before publishing any Fabrica asset, confirm:

- The main message tells the audience what changes for them.
- The product mechanism and the founder’s control are both clear.
- Claims have evidence or are labeled as a vision/early-access statement.
- The asset uses Forge Dark, Molten Orange, and Steel Gray according to their roles.
- Orange appears only where attention or action is genuinely needed.
- Typography uses Geist/Geist Mono (or the approved fallbacks) and remains readable.
- The logo has clear space, sufficient contrast, and an approved treatment.
- Copy avoids the blacklist and uses direct, builder-first language.
- Screens, quotes, metrics, and testimonials are real, current, and approved.

When in doubt, make it clearer, more specific, and easier to verify.
