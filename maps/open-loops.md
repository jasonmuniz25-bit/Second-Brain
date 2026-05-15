# open loops

*Anything in the vault with `status: open` or `status: blocked`. If something matters and isn't here, the frontmatter is missing or wrong.*

## open

```dataview
table file.folder as "where", project, created
from ""
where status = "open"
sort created asc
```

## blocked

```dataview
table file.folder as "where", project, created, blocked-on
from ""
where status = "blocked"
sort created asc
```

## stale (open >14 days)

```dataview
table file.folder as "where", project, created, (date(today) - created).days as "days open"
from ""
where status = "open" and (date(today) - created).days > 14
sort created asc
```
