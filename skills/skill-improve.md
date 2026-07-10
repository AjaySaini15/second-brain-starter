# SKILL — Skill-improve (meta-skill 2 of 3)
<!-- The skills loop's engine: corrections become permanent skill upgrades.
This is the difference between 20 versions of a skill and 20 repetitions of
the same mistake. -->

You watch for corrections to skill output and fold them back into the skill file — permanently.

## Auto-trigger — offer, don't wait to be asked
After any skill runs, watch for correction patterns: "no, that should…", "actually…", "that's wrong…", a fixed attribution/format/omission. When you see one, offer:
> "I got [specific thing] wrong in [skill]. Save this as a permanent improvement so it never recurs?"

## The test — skill failure vs data error (apply BEFORE proposing)
Ask: **would the same input, run again, produce the same wrong output?**
- YES → skill failure. Proceed.
- NO (the input itself was wrong/unusual, or the user said "just this once") → data error or one-off. Do NOT touch the skill.
Never fold corrections to *content values* (a wrong number in the source) into skill rules.

## Steps (on user's yes)
1. State the failure in one line: what the skill did vs what it should have done.
2. Propose the **surgical diff** — the exact line(s) to add or change in the skill file. Smallest change that prevents recurrence; no rewrites.
3. Apply it (Cowork/CLI: edit the file; chat: output the updated skill text to re-paste).
4. Bump the version line and append to the change log at the bottom of the skill:
   `- v1.3 (2026-07-12): never assign actions to attendees who only observed — [trigger: X correction]`

## Rules
- One correction = one focused edit. If a skill needs its third patch in a week, propose a rethink of the skill instead of a fourth patch.
- The change log is not optional — it's how you (and the user) audit why the skill behaves as it does.
- If the same correction keeps arriving despite the rule, say so plainly: the rule isn't working, don't just re-add it.
