---
type: place
place_type: attraction
status: visited
parent: "[[Rome]]"
visited_date: 2024-09-09
rating: 5
map_url:
source_url:
created_date: 2026-10-27
tags:
  - travel
  - place
  - topic/history
icon: 📍
---

# Colosseum

## Why visit

Core Rome landmark and the highlight outdoor ruin of [[Rome and Florence 2024]].

## Practical info

- **Best time:** Earliest timed entry
- **How to get there:** Metro Colosseo
- **Cost / tickets:** Book timed entry with Forum/Palatine combo
- **Hours:** Seasonal last admission earlier than closing time

## Highlights

- Arena level views when included
- Combine with Forum and Palatine the same morning

## Visit log

- Visited 2024-09-09 on [[Rome and Florence 2024]]; still queued ~25 minutes with a timed ticket.

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

- Parent: [[Rome]]
- [[Travel]]
- [[Dashboard_Travel]]
