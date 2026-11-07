---
type: area
status: active
tags:
  - area
  - topic/pkm
created_date: 2026-10-01
review_frequency: monthly
---

# Knowledge Management

Utrzymuj wiarygodny system przechwytywania, syntezy, wyszukiwania i ponownego użycia wiedzy.

## Aktywne projekty

```dataview
LIST
FROM "20_Projects"
WHERE type = "project" AND area = this.file.link AND status != "archived"
SORT target_date ASC
```

## Kluczowe zasoby

Linkuj tu trwałe zasoby PKM (książki, artykuły, kursy), gdy pojawią się w `40_Resources`.

## Standardy

- Każdy aktywny projekt ma jedno widoczne następne działanie.
- Elementy ze skrzynki są wyjaśnione, zanim zostaną przeniesione.
- Trwałe pojęcia linkują z powrotem do tego MOC.
