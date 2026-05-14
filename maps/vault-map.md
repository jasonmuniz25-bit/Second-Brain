# vault-map.md — navigation manual

*Read this to understand where things live and how to create new files.*

## folder purposes

**00-inbox/** — everything lands here first. Voice note transcripts,
quick ideas, links to process. Run /process-inbox to classify and file.

**01-groundwork-ai/** — all GroundWork AI business work
- business-strategy/ — positioning, services, pricing, prospect audit, assessment SOP
- corcontracting/ — the proof-of-concept client engagement
  - ghl/ — GHL build state, workflow documentation
  - airtable/ — Airtable build status, schema docs
  - sops/ — SOP inventory, troubleshooting guides, bottleneck maps
  - marketing/ — leads, nurture copy, ad assets, contracts

**02-hvac-sales-ai/** — HVAC sales roleplay coach project
- roleplay-sessions/ — processed transcripts from Otter.ai recordings

**03-personal/** — Freedom Project: fitness, BJJ, financial context
- fitness/ — training logs, macros, programs

**AI/** — everything Claude Code writes goes here
- sessions/ — session summaries, one file per session
- weekly-reviews/ — Sunday synthesis notes
- inbox-processed/ — archive of processed inbox items

**maps/** — the navigation layer. Me.md, this file, and skills/.

## how to create notes
- Check templates/ first and use the matching template
- Default location when unsure: 00-inbox/
- Use wikilinks [[note-name]] to connect related notes
- YAML frontmatter on every note: created, tags, status, project

## note naming
- Lowercase kebab-case. No spaces.
- Session summaries: YYYY-MM-DD-topic.md
- Daily notes: YYYY-MM-DD.md