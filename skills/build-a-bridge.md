# SKILL — Build a bridge (build your eyes, part 2 of 2)
<!-- Run-stage skill, for Claude Code / CLI (Cowork can do the design steps).
Takes ONE surface from your eyes-roadmap and connects it — by having your AI
write the thin script itself. No shipped code in this kit: your AI writes a
bridge for YOUR stack, which is the whole point. -->

You are building me one input bridge: from the surface I name to my brain folder. You write the code; I approve each step.

## Steps
1. **Scope it** — confirm from my eyes-roadmap: which surface, what exact signal (e.g., "calendar events + attendees", not "my calendar"), how often it should flow (daily? on-demand?).
2. **Pick the least-privilege path, in this order:** native export/subscription (ICS feed, forward-to-email, scheduled CSV) → official API with READ-ONLY scope → last resort, ask me before anything clever. Explain the choice in two lines.
3. **Preflight:** check what auth it needs and have me create my own credentials (my account, my tokens, stored OUTSIDE the brain folder — never in a file that could get shared or committed). If this is a work surface: confirm my company permits it; if unsure, STOP and downgrade to a manual export routine.
4. **Write the thin script** — smallest possible: fetch → normalize to plain text/markdown → write to `notes/inbox/<surface>-<date>.md`. No frameworks, no heavy connectors; loops and batching welcome. Show me the code before first run.
5. **Test read-only on a small sample** (one day's data). I eyeball the output for anything that shouldn't be stored. Only then widen.
6. **Add the organizing step — eyes are useless without understanding:** extend the run so that after fetching, you (the AI) process `notes/inbox/` — route each item per the CLAUDE.md rules: durable facts → propose MEMORY lines · action items → wherever my tasks live · raw material stays in notes/ under a dated file. Inbox should be EMPTY after each run; that's the definition of organized.
7. **Run it manually for a week.** Only after a clean week, schedule it (launchd/cron) — and remember the staging-gate rule from `04-run-first-quarter.md` for anything that WRITES outward.

## Rules
- One bridge at a time, reliable before the next. A flaky eye is worse than no eye — you stop trusting the whole system.
- Read-only until there's a proven reason to write. Writing goes behind a staging gate, always.
- Log every run (one line: when, items fetched, items routed) — silent failure is the default failure mode; a dead bridge looks like a quiet day.
