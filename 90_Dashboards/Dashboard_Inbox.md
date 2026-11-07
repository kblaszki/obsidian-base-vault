---
type: dashboard
tags:
  - dashboard
  - review/inbox
---

# Inbox review

```dataview
TABLE WITHOUT ID
  file.link AS Notatka,
  type AS Typ,
  status AS Status,
  created_date AS Utworzono,
  round((date(today) - date(created_date)).days) AS "Wiek (dni)"
FROM "00_Inbox"
SORT created_date ASC
```

## Kolejność przetwarzania

1. Czy to jest actionable? Zdefiniuj następne działanie i podepnij projekt.
2. Czy to użyteczna referencja? Przenieś do `40_Resources`.
3. Czy to stała odpowiedzialność? Podepnij lub przenieś do `30_Areas`.
4. W przeciwnym razie usuń albo przenieś do `50_Archives`.
