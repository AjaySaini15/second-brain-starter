# SKILL — Schedule a skill (the automation layer)
<!-- Run-stage, for Claude Code / CLI. Takes ONE skill you already trust and
puts it on a timer — with the three survival features every automation needs:
a staging gate, a run log, and a dead-man check. Your AI writes all of it. -->

You are putting one of my existing skills on a schedule. You write the runner and the schedule; I approve each step.

## Preconditions — refuse politely if not met
- The skill has been run manually at least 5 times with good output. We don't automate guesses.
- Its inputs are available without me (a folder, a feed, a bridge output) — a skill that needs me mid-run can't be scheduled.

## Steps
1. **Scope:** which skill, what cadence (daily 7am? Friday 6pm?), and what exact inputs it reads.
2. **Write the runner** — a small script that: runs the skill headlessly → writes the output to `staging/<skill>-<date>.md` (NEVER to its live destination) → appends one line to `logs/runs.log`: `<timestamp> <skill> OK|FAIL <one-line detail>`. On any failure: still write the runs.log line and a visible notification if the OS supports it. Show me the script before first run.
3. **The staging gate stays, permanently:** I review staging files and approve; only an explicit second step (manual at first) moves output to its real destination — sends the email, updates the file, posts the message. Automation without a gate is how you stop trusting your own system.
4. **Schedule it** — macOS: `launchd` plist; Linux: `cron`. Show me the entry, install on my yes.
5. **Install the dead-man check:** add one line to my CLAUDE.md session-open ritual — "check `logs/runs.log`: if any scheduled skill has no OK line within its expected cadence, tell me FIRST, before anything else." A dead job looks exactly like a quiet day; this is the only thing that makes silence visible.
6. **Probation week:** for the first week, mention every run's staging output at session open so I build the review habit. After a clean week, it's part of the furniture.

## Rules
- One scheduled skill at a time; the next one waits until this one has survived two weeks.
- Anything that writes OUTWARD (email, messages, shared docs) keeps the human gate forever — no exceptions, including for me on a confident day.
- If I stop reviewing the staging folder for a week, say so plainly — an unreviewed gate is theater, and we should either recommit or unschedule.
