---
type: place
place_type: city
status: visited
parent: "[[Tuscany]]"
visited_date: 2024-09-15
rating: 5
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
---

# Florence

## Why visit

Renaissance core with walkable evenings and [[Uffizi]] as the museum anchor.

## Practical info

- **Best time:** Shoulder seasons
- **How to get there:** Freccia from Rome; FLR airport on departure
- **Cost / tickets:** Prebook Uffizi
- **Hours:** Many sites close earlier than Rome nightlife implies

## Highlights

- Oltrarno
- Piazzale Michelangelo sunset
- Ponte Vecchio (expect crowds)

## Visit log

- Visited 2024-09-12 to 2024-09-15 on [[Rome and Florence 2024]].

## Child places

```dataview
TABLE WITHOUT ID file.link AS Place, place_type AS Kind, status AS Status
FROM "40_Resources/Places"
WHERE parent = this.file.link
SORT place_type ASC, file.name ASC
```

## Trips

```dataview
LIST
FROM "20_Projects/Trips"
WHERE type = "trip" AND contains(file.outlinks, this.file.link)
SORT start_date DESC
```

## Related

- Parent: [[Tuscany]]
- [[Uffizi]]
- [[Travel]]
- [[Dashboard_Travel]]
