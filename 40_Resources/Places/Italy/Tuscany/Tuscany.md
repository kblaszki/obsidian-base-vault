---
type: place
place_type: region
status: visited
parent: "[[Italy]]"
visited_date: 2024-09-15
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Tuscany+Italy"
location: [43.7711, 11.2486]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/florence-skyline.jpg]]"
banner_position: center
---

# Tuscany

## Why visit

Florence and surrounding Renaissance core.

## Practical info

- **Best time:** Shoulder seasons
- **How to get there:** Freccia from Rome; FLR airport
- **Cost / tickets:** Prebook Uffizi
- **Hours:** Many sites close earlier than Rome nightlife implies

## Highlights

- [[Florence]]
- [[Uffizi]]

## Visit log

- Visited September 2024 on [[Rome and Florence 2024]].

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

- Parent: [[Italy]]
- Map: [Tuscany Italy](https://www.google.com/maps/search/?api=1&query=Tuscany+Italy)
- [[Travel]]
- [[Dashboard_Travel]]
