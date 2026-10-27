---
type: dashboard
tags:
  - moc
---

# Home

## Navigate

- [[Dashboard_Today|Today]]
- [[Dashboard_Projects|Projects]]
- [[Dashboard_Inbox|Inbox review]]
- [[Knowledge Management]]
- [[Software Development]]

## Recently changed

```dataview
TABLE WITHOUT ID file.link AS Note, type AS Type, status AS Status, file.mtime AS Modified
FROM -"99_Templates"
WHERE file.name != this.file.name
SORT file.mtime DESC
LIMIT 10
```
