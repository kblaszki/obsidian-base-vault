---
type: dashboard
tags:
  - dashboard
  - review/weekly
---

# Projects

## Otwarte projekty według statusu

```dataview
TABLE WITHOUT ID
  key AS Status,
  rows.file.link AS Projekty,
  rows.area AS Obszary,
  rows.target_date AS Terminy
FROM "20_Projects"
WHERE type = "project" AND status != "done" AND status != "archived"
GROUP BY status
SORT key ASC
```

## Wymagają przeglądu

```dataview
TABLE area AS Obszar, status AS Status, review_date AS "Termin przeglądu"
FROM "20_Projects"
WHERE type = "project"
  AND status != "done"
  AND status != "archived"
  AND review_date
  AND date(review_date) <= date(today)
SORT review_date ASC
```

## Nieukończone zadania projektów

```dataview
TASK
FROM "20_Projects"
WHERE !completed
GROUP BY file.link
```
