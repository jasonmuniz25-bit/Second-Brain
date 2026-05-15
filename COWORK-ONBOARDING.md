# Claude Cowork onboarding — read this once

This vault is wired so any Claude (Claude Code, Claude Cowork, Claude.ai with a connector) can pick it up. Below is the **specific Cowork setup** so you don't have to figure it out cold.

---

## one-time setup

### 1. Connect this GitHub repo to Cowork

In Claude Cowork:
- Settings → **Connectors** → **GitHub**
- Authorize, then choose the repo: `jasonmuniz25-bit/Second-Brain`
- Branch: `main`

That gives Cowork read access to the vault. Every time you push a new commit from Obsidian, Cowork sees the latest version on next session.

### 2. Push from Obsidian automatically

Install the **Obsidian Git** community plugin:
- Obsidian → Settings → Community plugins → Browse → search "Obsidian Git" → Install + Enable
- In its settings: enable **Auto Backup** every 10 minutes (or whatever cadence feels right)
- Set commit message to something simple like `vault sync`

Now writing a note in Obsidian → push to GitHub → visible to Cowork. No copy-paste.

### 3. Create a Cowork Project for the vault

In Cowork, create a new **Project** called "Second Brain" and pin the GitHub connector to it. Anything you do inside that project has the vault as context automatically.

---

## starting a session in Cowork

Open the Second Brain project. Send this exact first message:

> Read `CLAUDE.md`, then `maps/me.md`, then the most recent file in `AI/sessions/`. State in one sentence what context you found, then ask me what we're working on.

That's the cold-start prompt. Pin it as a saved prompt in Cowork so you don't retype it.

## ending a session in Cowork

Type: **"wrap this up"** or **"close this out"** or **"session summary."**

Cowork will read `maps/skills/session-summary.md`, follow the format, and give you the markdown for a new file at `AI/sessions/YYYY-MM-DD-topic.md`. **Cowork can't write to GitHub through the connector**, so:

1. Cowork outputs the file content in chat.
2. You create the file in Obsidian (paste content), save, and Obsidian Git pushes it.

If you're using the **Cowork Computer Use / Claude Desktop with file access** instead, it can write the file directly.

## processing the inbox

Type: **"process the inbox"**

Cowork reads `00-inbox/`, classifies each note, and tells you where each one should go. You move the files in Obsidian. Original files get archived to `AI/inbox-processed/` (you do the move, Cowork tells you the destination).

## weekly review

Sundays, type: **"weekly review"**

Cowork reads the week's session summaries + daily notes and writes the week's `AI/weekly-reviews/YYYY-Www.md` file content. Same as session summary — paste, save, push.

---

## what Cowork *can't* do that Claude Code could

- Write files directly to your filesystem (without Computer Use)
- Run terminal commands
- Auto-trigger on file save

That's why the workflow above is "Cowork outputs → you paste into Obsidian → Obsidian Git pushes." The vault structure makes it fast.

---

## if something feels broken

- **Cowork doesn't see your latest note** → check Obsidian Git pushed (Source Control panel) and that the GitHub connector is still authorized.
- **Cowork forgets your tone / preferences mid-session** → it skipped reading `maps/me.md`. Tell it to read the file again.
- **Cowork wants to overwrite `maps/me.md`** → don't let it. The file's hard rule says it only edits with your explicit "yes, change me.md."
