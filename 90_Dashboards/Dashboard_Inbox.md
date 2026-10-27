---
type: dashboard
tags:
  - dashboard
  - review/inbox
---

# Inbox review

```dataview
TABLE WITHOUT ID
  file.link AS Note,
  type AS Type,
  status AS Status,
  created_date AS Created,
  round((date(today) - date(created_date)).days) AS "Age (days)"
FROM "00_Inbox"
SORT created_date ASC
```

## Processing order

1. Is it actionable? Define the next action and link a project.
2. Is it useful reference? Move it to `40_Resources`.
3. Is it a continuing responsibility? Link or move it to `30_Areas`.
4. Otherwise delete it or move it to `50_Archives`.
