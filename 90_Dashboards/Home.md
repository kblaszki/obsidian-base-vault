---
type: dashboard
tags:
  - moc
---

# Home

## Nawigacja

- [[Dashboard_Today|Dziś]]
- [[Dashboard_Projects|Projekty]]
- [[Dashboard_Travel|Podróże]]
- [[Dashboard_Inbox|Przegląd skrzynki]]
- [[Knowledge Management]]
- [[Software Development]]
- [[Travel]]

## Ostatnio zmienione

```dataview
TABLE WITHOUT ID file.link AS Notatka, type AS Typ, status AS Status, file.mtime AS Zmodyfikowano
FROM -"99_Templates"
WHERE file.name != this.file.name
SORT file.mtime DESC
LIMIT 10
```
