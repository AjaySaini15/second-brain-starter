# Run — the first quarter (the builder stage)

**Goal:** the system stops waiting for you. It acts on schedule, touches your real surfaces, and you become the approval gate instead of the operator. Claude Code / the CLI is the natural home (same thing as Cowork's engine, different clothes — the terminal just runs many threads at once).

## The five patterns that make it real
Build them in this order — each one is a week or two of evenings, and the AI writes most of the code itself.

**1. The scheduled skill.** Take the skill you run most (daily brief, weekly review) and put it on a timer so the output exists before you ask. macOS: `launchd`; Linux: `cron`; anywhere: a calendar-triggered script. The test of this level: something useful was waiting for you when you woke up.

**2. The staging gate (maker-checker).** Never let an automation act directly on the world. It writes its output to a `staging/` folder as a reviewable file; you tick what you approve; a second step executes only the ticks. One folder = one inbox of everything pending your yes. This single pattern is what keeps trust in your own system as it scales.

**3. The bridge.** Connect one real surface you use daily — calendar, mail, sheets. When access is blocked, don't stop: describe the block to the AI and let it write a thin script around it (an API bridge is an afternoon, not a project). Own thin scripts beat heavy connectors: less token overhead, loops and batching, and you control what goes back and forth.

**4. The self-improving loop.** Create two meta-skills: a `log` skill (end of each working session: append what was done, what was corrected, what's open) and a `skill-improve` skill (fold a correction back into the skill file that caused it, permanently). This is the difference between 20 versions of a skill and 20 repetitions of a mistake.

**5. The health check.** Once you have 3+ scheduled jobs, add a script that answers one question: *did everything run when it should have?* Silent failure is the default failure mode of automation — a dead job looks exactly like a quiet day. A read-only checker that lists each job's last successful run turns "silent" into "caught."

## The reference implementation
My full setup — the architecture, the staging inboxes, the health board, the memory graph — is documented at [ajaysaini.io/second-brain](https://ajaysaini.io/second-brain/), and the business-process version at [ajaysaini.io/kaizen](https://ajaysaini.io/kaizen/). Steal the shapes, not the specifics.

## Two warnings from my own scars
- **Don't over-build.** Past a point, more rules make it brittle — if you're adding corrections faster than you're using outputs, stop and simplify. I've had to learn when to stop tuning.
- **Thread hygiene.** Long chat threads compound their own context cost. End a work thread with a handover note (the log skill), clear, start fresh. Separate threads per topic.

## Staying current (my actual inputs)
Nate B Jones · Product Hunt newsletter · podcasts on commutes. Build in public and compare notes — the architecture is shareable; the accumulated context is yours alone.
