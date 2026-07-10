# Your first 30 minutes

One rule for this whole kit: **you never type a file — you talk, the AI writes.** Works with ChatGPT, Claude, or Gemini, whichever you already pay for.

## Minute 0–5 — rescue what your AI already knows
Your current chat tool has been quietly building memory about you. Run **Prompt A** (or business-only **Prompt B**) from `templates/export-your-memories.md` and keep the output in the conversation.

## Minute 5–20 — dictate the interview
Open `templates/interview-and-generate.md`. Answer its 10 questions **out loud** — voice mode, phone-keyboard mic, or a dictation app; ramble, detail is the point. (Typing works; you'll just say less.)

## Minute 20–25 — let it write your files
Paste the generator prompt from the same file. It turns your dictation + memory export into `CONTEXT.md` and `MEMORY.md` — your words, organized, gaps flagged as TODOs.

## Minute 25–30 — install the operating system
Install two things into your project / custom instructions:
1. The generated **CONTEXT.md** (what it knows about you), and
2. **`templates/CLAUDE-starter.md`** (how it MAINTAINS what it knows — the rules that make it propose its own memory updates every time you correct it).

That second file is the difference between a note and a system. From now on, every conversation starts already knowing you — and gets a little smarter when you correct it, without you maintaining anything by hand.

**Tomorrow:** `02-crawl-week-one.md`.
