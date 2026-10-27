---
type: dashboard
tags:
  - dashboard
  - review/weekly
---

# Projects

## Open projects by status

```dataview
TABLE WITHOUT ID
  key AS Status,
  rows.file.link AS Projects,
  rows.area AS Areas,
  rows.target_date AS Targets
FROM "20_Projects"
WHERE type = "project" AND status != "done" AND status != "archived"
GROUP BY status
SORT key ASC
```

## Needs review

```dataview
TABLE area AS Area, status AS Status, review_date AS "Review due"
FROM "20_Projects"
WHERE type = "project"
  AND status != "done"
  AND status != "archived"
  AND review_date
  AND date(review_date) <= date(today)
SORT review_date ASC
```

## Incomplete project tasks

```dataview
TASK
FROM "20_Projects"
WHERE !completed
GROUP BY file.link
```
