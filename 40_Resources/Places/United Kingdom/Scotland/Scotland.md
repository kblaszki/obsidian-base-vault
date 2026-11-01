---
type: place
place_type: region
status: visited
parent: "[[United Kingdom]]"
visited_date: 2025-08-09
rating: 5
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
---

# Scotland

## Why visit

Highlands and islands corridor for [[Scottish Highlands 2025]].

## Practical info

- **Best time:** Long daylight months
- **How to get there:** EDI + rental car
- **Cost / tickets:** Parking honesty boxes common
- **Hours:** Weather dependent outdoors

## Highlights

- [[Edinburgh]] urban start
- [[Isle of Skye]] cliffs
- [[Glencoe]] valley

## Visit log

- Visited August 2025 on [[Scottish Highlands 2025]].

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

- Parent: [[United Kingdom]]
- [[Travel]]
- [[Dashboard_Travel]]
