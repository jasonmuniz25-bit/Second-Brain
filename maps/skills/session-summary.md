# skill: session-summary

**trigger:** Jay says "wrap this up," "close this out,"
"session summary," or similar end-of-session phrase.

**process:**
1. Identify today's date (YYYY-MM-DD format)
2. Identify the session topic (2-4 words, kebab-case)
3. Create file at: AI/sessions/YYYY-MM-DD-[topic].md
4. Write the summary using this exact format:

---
created: YYYY-MM-DD
tags: [session-summary, [topic-tag]]
project: [project-name]
ai-generated: true
---

# Session Summary — [Topic] — [Date]

## what we built / decided
[Concise bullets of concrete outputs and locked decisions]

## current state
[Where things stand right now]

## open items
[Unresolved questions, flags, things waiting on someone]

## next session should start with
[Exact prompt a fresh Claude instance could use to pick up immediately]

5. Confirm: "Summary written to AI/sessions/[filename].md"

**rules:**
- Never overwrite existing session files
- Make "next session should start with" specific enough
  that a cold-start Claude could continue immediately
- If Jay says "update the summary" — create [filename]-v2.md