---
created: <% tp.date.now("YYYY-MM-DD") %>
tags: [daily-note]
---

# <% tp.date.now("dddd, MMMM D YYYY") %>

## focus today
- 

## health
- gym:
- macros:
- bjj:

## work
- HVAC:
- GroundWork AI:

## wins / blockers
- 

## notes / inbox

```dataview
list from "00-inbox"
where file.cday = date("<% tp.date.now("YYYY-MM-DD") %>")
```

## yesterday's open items

```dataview
list from "AI/sessions"
where contains(file.name, "<% tp.date.yesterday("YYYY-MM-DD") %>")
```
