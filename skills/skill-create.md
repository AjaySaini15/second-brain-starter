# SKILL — Skill-create (meta-skill 3 of 3)
<!-- How new skills get born: from doing, never from a blank page. The user
never hand-writes a skill; you draft it from observed work. -->

You turn a task the user just did with you into a reusable skill file.

## Trigger
The second time the user does a similar task with you — or whenever they say "write this up as a skill" — offer:
> "We've done this twice. Want me to write it up as a skill so next time it's one command?"

## Steps
1. **Interview — exactly 3 questions** (dictated answers are fine):
   a. When should this run — what would you SAY to invoke it, and does it recur on a schedule?
   b. What inputs does it need (pasted text, a file, a folder, nothing)?
   c. Show me the output you'd call perfect — or point at the one we just made and tell me what to change.
2. **Draft the skill file** with this exact skeleton:
   ```
   # SKILL — <name>
   <!-- one line: what this does and when to reach for it -->
   ## When to use        (trigger phrases + schedule if any)
   ## Inputs
   ## Steps              (numbered, specific, no step you couldn't follow yourself)
   ## Output format      (a literal template block)
   ## Rules              (the sharp edges: never do X, always check Y)
   - v1.0 (<date>): created from <the task we just did>
   ```
3. **Dry-run it** against the input from the task you just did together. Show output next to the original. Fix gaps before saving — a skill that hasn't run once isn't a skill, it's a guess.
4. **Save it where this tool keeps skills** (see README "Where files live") and add one line to MEMORY.md → Working agreements: `- <name> skill: runs when …`

## Rules
- Steps must be executable without the user in the room. "Use judgment" is not a step.
- Rules section captures corrections-so-far; from now on, skill-improve maintains it.
- Name skills by what they produce, not by tool ("weekly-review", not "claude-summary-helper").
