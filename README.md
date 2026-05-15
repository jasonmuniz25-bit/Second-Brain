# Second Brain

Jay's personal knowledge base + working vault for **GroundWork AI**, **CorContracting**, **HVAC Sales AI**, and the Freedom Project.

Built as an Obsidian vault, version-controlled in Git, designed to be driven by Claude (Cowork or Code).

## start here

1. **`COWORK-ONBOARDING.md`** — how to wire Claude Cowork to this repo and how to start/end sessions.
2. **`CLAUDE.md`** — what Claude reads on every session start. Defines protocols and hard rules.
3. **`maps/me.md`** — who Jay is, how he thinks, how to work with him. The canonical identity file.
4. **`maps/vault-map.md`** — folder structure and file naming rules.

## folder structure (high level)

```
00-inbox/          captures land here first
01-groundwork-ai/  the business + corcontracting client
02-hvac-sales-ai/  sales roleplay coach
03-personal/       fitness, bjj, freedom-project
AI/                everything Claude writes (sessions, weekly reviews, processed inbox)
daily-notes/       one note per day
maps/              identity, navigation, skills, dynamic indexes
templates/         note templates
```

Every folder has a `_README.md` explaining what belongs in it.

## obsidian setup

Plugins required:
- **Dataview** (community) — installed
- **Templater** (community) — installed
- **Obsidian Git** (community) — install for auto-push to GitHub. See `COWORK-ONBOARDING.md`.

Core plugins configured:
- Daily Notes → folder `daily-notes/`, format `YYYY-MM-DD`, template `templates/daily-note.md`
- Templates → folder `templates/`
