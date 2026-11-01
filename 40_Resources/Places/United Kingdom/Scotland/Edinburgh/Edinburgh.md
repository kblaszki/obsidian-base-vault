---
type: place
place_type: city
status: visited
parent: "[[Scotland]]"
visited_date: 2025-08-03
rating: 4
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
---

# Edinburgh

## Why visit

Strong urban start before the Highlands drive on [[Scottish Highlands 2025]].

## Practical info

- **Best time:** Avoid peak festival if you want quiet; August is lively
- **How to get there:** EDI tram
- **Cost / tickets:** Castle timed entry
- **Hours:** Long summer daylight

## Highlights

- Royal Mile
- Castle views
- New Town café streets

## Visit log

- Visited 2025-08-02 to 2025-08-04 on [[Scottish Highlands 2025]].

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

- Parent: [[Scotland]]
- [[Travel]]
- [[Dashboard_Travel]]
