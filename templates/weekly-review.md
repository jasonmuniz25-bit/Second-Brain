---
created: <% tp.date.now("YYYY-MM-DD") %>
tags: [weekly-review]
ai-generated: true
---

# Weekly Review — Week of <% tp.date.now("YYYY-MM-DD", -6) %>

## what got built / decided

## what got dropped or deferred

## patterns worth noticing

## top 3 priorities for next week
1. 
2. 
3. 

## metrics / health
- training sessions:
- macro days hit:
- HVAC closes:
- GroundWork AI hours:

## sessions this week

```dataview
list from "AI/sessions"
where file.cday >= date("<% tp.date.now("YYYY-MM-DD", -6) %>")
sort file.cday asc
```
