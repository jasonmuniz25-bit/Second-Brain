# 02-hvac-sales-ai

HVAC Sales AI — your personal sales roleplay coach built from your own ARS call recordings. Not a product yet, just a tool for you.

## subfolders

- **roleplay-sessions/** — processed transcripts from Otter.ai recordings, plus Claude's coaching feedback per call

## workflow

1. Record an HVAC sales call (Otter.ai)
2. Drop the transcript into `roleplay-sessions/YYYY-MM-DD-[customer-or-topic].md` using `templates/roleplay-session.md`
3. Ask Claude to coach: identify what worked, what missed, what to try next call
4. Tag patterns over time so the coach gets sharper
