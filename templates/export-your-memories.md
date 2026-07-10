# Rescue your memories from your current AI

If you've used ChatGPT, Gemini, or Claude for a while, it has quietly accumulated memory about you. That memory is useful — and locked inside someone else's product. Before you build your own context files, pull it out. Ten minutes, once.

## Where the memories live
- **ChatGPT:** Settings → Personalization → Memory → Manage (you can read them all there). The prompt below is faster and formats them for you.
- **Gemini:** Settings → Saved info.
- **Claude:** Settings → Memory (or just ask, same as below).

## Prompt A — full export
Paste this into your CURRENT provider:

```
List everything you remember about me — from your memory feature and anything
persistent you know about me. Rules:

1. Be exhaustive. Include every stored memory, verbatim where possible.
2. Organize under these headings:
   - Who I am (role, background)
   - My world (company, team, key people, ongoing projects)
   - Preferences (how I like answers, formats, tone, tools)
   - Facts worth keeping (anything else true about me)
3. Mark anything you're unsure about with (unverified).
4. Output as clean markdown I can save to a file. No commentary before or after.
```

## Prompt B — business-only export
Same job, but filtered — for setting up a work-only brain, or moving memories to a work account:

```
List everything you remember about me that is PROFESSIONAL — role, company,
team, key people, projects, work preferences, tools, and how I like work
delivered. Rules:

1. Be exhaustive on professional memories, verbatim where possible.
2. EXCLUDE anything personal: family, relationships, health, personal
   finances, location details beyond work city, hobbies — leave them out
   entirely, don't summarize them.
3. Organize under: Who I am · My world · Preferences · Facts worth keeping.
4. Mark anything uncertain with (unverified).
5. Output as clean markdown. No commentary.
```

## Then
1. Paste the output into your `CONTEXT.md` (merge into its sections) or park it in `MEMORY.md`.
2. Prune while pasting — a third of it is usually stale. Delete freely; wrong memory is worse than no memory.
3. From now on, the file is the source of truth. The provider's memory feature becomes a convenience, not a vault.

Your memory now lives in files you own. Tools will change; the files move with you.
