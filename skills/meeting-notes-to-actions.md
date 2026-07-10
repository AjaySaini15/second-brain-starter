# SKILL — Meeting notes → actions
<!-- Paste this whole file into your AI along with your raw notes/transcript.
Or, if your tool supports skills/instructions, install it once and just say
"run meeting-notes on this". Works at every level from chat to CLI. -->

You are processing my raw meeting notes or transcript into structured, actionable output. Use my CONTEXT file to resolve names, priorities, and ownership.

## Steps
1. Read the full input before extracting anything.
2. Extract ACTION ITEMS — things someone committed to do or clearly must do:
   - owner (a person, from context; if unclear, mark "OWNER?")
   - the action, phrased as a verb-first instruction
   - due date if stated; otherwise suggest one based on urgency
   - urgency: high / normal
3. Extract DECISIONS — anything that was settled, with a one-line rationale.
4. Extract OPEN QUESTIONS — raised but not resolved.
5. Note SIGNALS — one or two lines max: anything a good chief of staff would flag (a risk mentioned in passing, a commitment that contradicts an earlier one, a person who pushed back).

## Output format
```
MEETING: <inferred title> · <date>
ACTIONS
1. [owner] action — due <date> (urgency)
DECISIONS
- decision — rationale
OPEN
- question
SIGNALS
- observation
```

## Rules
- Never invent actions that weren't discussed. If the meeting produced nothing actionable, say so.
- Keep my team's names exactly as they appear in my CONTEXT file.
- If the notes are partial or garbled, extract what's solid and list what seems missing — don't fill gaps with guesses.
