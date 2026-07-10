# Day 1 — the interview you dictate, and the prompt that writes your files

You do not type your context files. You talk; the AI writes them. Two steps.

## Step 1 — dictate the interview
Open your chat tool. Use voice if it has it (or your phone keyboard's mic, or a dictation app like Wispr Flow). Typing works too — it's just slower and you'll say less, and detail is the whole point.

Answer these out loud, in full flow, rambling encouraged — one long message or several:

1. Who are you? Role, company, what the business does, what you actually do all day.
2. Walk me through yesterday, hour by hour.
3. Who are the people around you? Team, boss, peers — names, what they own, how they operate.
4. What are you trying to move in the next 3 months? What does your boss want from you?
5. What decisions do you make repeatedly? How do you decide — what do you optimize for?
6. What work annoys you most every week? Where does your time leak?
7. What meetings/rhythms recur? (weekly reviews, monthly closes, 1:1s…)
8. How do you like answers delivered — direct or diplomatic, short or thorough? What should it never do?
9. What must never be stored or repeated? What should it always ask before doing?
10. Anything an ideal chief of staff would know about you that nobody ever asks?

## Step 2 — paste this generator prompt

```
From everything I just dictated (plus my memory export, pasted below if I have
one), create two markdown files.

FILE 1 — CONTEXT.md with sections: Who I am · My world (company, team, key
people) · My priorities right now · How I decide · How to talk to me ·
Boundaries.

FILE 2 — MEMORY.md with sections: Decisions · People · Projects · Lessons ·
Working agreements — seeded with whatever I gave you that fits, one line per
item.

Rules:
1. My words, tightened — don't invent, don't embellish.
2. Bullets, not prose. Specific beats complete.
3. Where something important seems missing, add a line "TODO: <the question
   to answer>" rather than guessing.
4. Ask me at most 3 sharp follow-up questions first if anything critical is
   unclear — then produce both files, each in its own code block so I can
   save or install them directly.
```

## Step 3 — bootstrap from your existing tool (do this too — it's free)
Your current chat tool already knows things about you. Run the export prompt from `export-your-memories.md` (full or business-only version) and paste its output into the same conversation before Step 2 — the generator folds it in.

## Step 4 — install
- **Chat tools:** paste CONTEXT.md + the operating rules from `CLAUDE-starter.md` into project instructions / custom instructions. Keep MEMORY.md in the project too.
- **Cowork / Claude Desktop / CLI:** save all three files into your brain folder — from here on, the AI maintains them itself (see `03-walk-first-month.md`).

Total time: ~25 minutes, of which ~15 is you talking. That's the whole setup.
