# SKILL — Session log & handover (meta-skill 1 of 3)
<!-- The memory loop's engine. Run at the end of any work session, and ALWAYS
before clearing/abandoning a long thread. In Cowork/CLI, the AI writes the
files itself; in a chat tool, it outputs blocks for you to keep. -->

You are closing out a working session. Your job: make sure nothing this session produced evaporates, and leave a clean starting point for the next session.

## Steps
1. **Summarize the session** — 5–10 bullets, written for a future session that has zero memory of this one: what was produced (files, drafts, decisions), what was corrected and why, what's open or deferred. Facts, not narrative.
2. **Append it** to `logs/YYYY-MM-DD.md` in the brain folder (create if missing). Chat tools: output the block for the user to keep in the project.
3. **Propose memory updates** — scan the session for durable facts (a decision, a person detail, a lesson, a new working agreement) and propose one-line MEMORY.md entries under the right sections. Apply what the user approves.
4. **Propose skill updates** — if any correction this session was a *skill* failure (see skill-improve's test), flag it: "worth folding into <skill>? " Don't fold silently.
5. **If the thread is ending** (user is about to clear or start fresh): write a HANDOVER block — current state, next 3 steps, open questions — so the next thread starts warm instead of cold. This is what makes thread hygiene free.

## Rules
- Never skip step 3. The log without memory-proposals is a diary; with them, it's a compounding system.
- Bullets a future session can act on ("draft saved at X, awaiting review") beat prose ("we had a productive discussion").
- If the session produced nothing durable, say so in one line — a truthful empty log beats a padded one.
