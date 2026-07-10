# Second Brain Starter

A minimal, tool-agnostic starting point for building your own AI second brain — the kind I walked through in my session "Make AI Work For You" (July 2026). No exotic tools required, nothing to install for the first month, and everything you create stays in plain files **you own**.

## The mental model

AI already has a **brain** — you rent it for ~$20/month, same one as everyone else. That's exactly why the brain alone is not an edge. What you build is the rest of the body:

- **Eyes** — feed it what's actually going on: your notes, meetings, mail, documents.
- **Understanding** — organized memory (plain markdown files) + **skills** (your repeatable procedures, written once in plain English).
- **Hands** — let it produce: drafts, briefs, plans, reviews — with you as the approval gate.

The brain is rented. The body is yours. The body is the edge.

## Fastest start — let the kit install itself
Don't read all of this. Give it to your AI and let IT do the setup:

- **Claude Code (CLI):** `git clone https://github.com/AjaySaini15/second-brain-starter && cd second-brain-starter && claude` — then paste the prompt below.
- **Claude Cowork / Desktop:** download this repo (green button → Download ZIP), add the folder to Cowork, paste the prompt below.
- **Chat only (ChatGPT/Claude/Gemini):** paste this README plus `templates/interview-and-generate.md` and `templates/CLAUDE-starter.md` into a new conversation, then the prompt below.

> Read this starter kit end to end. Then set me up: run the Day-1 interview from templates/interview-and-generate.md conversationally — I'll answer by voice — and first have me run the memory-export prompt in my old AI tool so you can fold that in. Generate my CONTEXT.md and MEMORY.md, adopt CLAUDE-starter.md as your operating rules, install the six skills, and place every file where it belongs for THIS tool (the "Where files live" table below). Then tell me exactly what you set up, and what my first week looks like.

Twenty-five minutes, mostly you talking. That's the install.

## Where files live, by tool
| | Context + operating rules | Skills | Who maintains the files |
|---|---|---|---|
| **Chat tools** (ChatGPT / Claude / Gemini) | Project or custom instructions: paste CONTEXT.md + CLAUDE-starter.md text | Paste the skill file into the chat when you need it (or make one Project/Gem per heavy skill) | It proposes lines; you re-paste weekly (2 min) |
| **Claude Cowork / Desktop** | `my-brain/CLAUDE.md` (= CLAUDE-starter.md renamed) + CONTEXT.md + MEMORY.md in the folder you grant it | `my-brain/skills/*.md` | The AI edits files directly — zero manual upkeep |
| **Claude Code (CLI)** | `CLAUDE.md` at the root of the folder where you launch `claude` (or `~/.claude/CLAUDE.md` to apply everywhere) | `.claude/skills/<name>/SKILL.md` in the project — or `~/.claude/skills/` globally. With a name+description header they auto-trigger as /commands. Ask the AI to do this migration itself. | The AI edits files directly |

## What's inside

```
START-HERE/
  01-first-30-minutes.md    ← do this today. You talk for 15 min; it writes your files.
  02-crawl-week-one.md      ← week one: any chat tool — it maintains its own memory
  03-walk-first-month.md    ← month one: give it a folder (Cowork/Desktop) — it gets hands
  04-run-first-quarter.md   ← quarter one: schedules, staging gates, self-improving loops
templates/
  interview-and-generate.md ← the 10 questions you DICTATE + the prompt that writes your files
  CLAUDE-starter.md         ← the operating file — the rules that make memory maintain ITSELF
  CONTEXT.md                ← what the generator produces (spec — you never type this by hand)
  MEMORY.md                 ← the memory index it keeps for you
  export-your-memories.md   ← rescue what ChatGPT/Gemini/Claude already know about you
skills/
  meeting-notes-to-actions.md   ← the three starters: run these on real work
  weekly-review.md
  daily-brief.md
  log.md                        ← the scaffolding: session log & handover (the memory loop)
  skill-improve.md              ← corrections become permanent skill upgrades (the skills loop)
  skill-create.md               ← new skills get born from doing, never from a blank page
FAQ.md                      ← cost, privacy, which model, portability, "I can't code"
```

## Feed it — the organ most people forget
A second brain with no input stream is a filing cabinet. Get signal flowing in from day one:

- **Meetings — the richest input there is.** Use whatever transcription you already have: Google Meet / Teams / Zoom native transcripts, your phone's recorder + any transcriber app for physical meetings, or a dedicated tool. Drop every transcript into `notes/` (or paste it in, at chat level) and run the meeting-notes skill on it. My entire system started as exactly this and nothing more.
- **Your voice, daily.** One dictated end-of-day note — what happened, what's worrying you, what's next. Ugly is fine; volume beats form.
- **Documents you already produce** — reports, plans, reviews. Drop copies in `notes/` as you make them.
- Later (Run stage): calendar, mail, and sheets flow in through bridges — no pasting at all.

The rule: if it carries signal and you touched it today, the brain should see it.

## What this kit is — and isn't
This is my system at week-zero scale: the same anatomy (brain, eyes, memory, hands), the same two compounding loops (memory + skills), the same operating rules, the same meta-skills — minus 18 months of accumulated context and a fleet of automations. The architecture is fully shareable, and it's all here. The accumulated context is not shareable — nobody's is. You build that part by feeding yours, starting today. Twelve weeks of this kit ≈ where I was at month three; the rest is the same loops, run longer.

## The four rules that matter more than any tool

1. **You talk; it types.** You never hand-write a context file, a memory entry, or a skill — you dictate, it drafts, you approve. If the kit ever feels like homework, you're doing it the wrong way.
2. **Context beats prompts.** A clever prompt is a one-off; maintained context compounds. Every correction becomes a file update — proposed by the AI itself (that's what `CLAUDE-starter.md` is for).
3. **Own your memory.** Plain files on your machine — not locked inside any product's memory feature. Files move with you when tools change. Tools will change.
4. **It's a workout, not a vending machine.** Weeks 1–2 feel like more effort, not less. Results show around month two — if you keep feeding it. Most people quit before the compounding starts. Don't.

## Where this comes from

I run a 300+ person business on a much bigger version of this — the architecture is written up here:
- [I Built a Second Brain to Run a 300-Person Business](https://ajaysaini.io/second-brain/)
- [The ₹2,000 AI Sales Engine](https://ajaysaini.io/kaizen/)

The architecture is shareable. The accumulated context is not — that part you build yourself, starting with the next 30 minutes.

— Ajay Saini
