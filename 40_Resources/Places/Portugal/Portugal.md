---
type: place
place_type: country
status: visited
parent:
visited_date: 2025-05-17
rating: 5
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/lisbon-view.jpg]]"
banner_position: center
---

# Portugal

## Why visit

Atlantic cities with hills, miradouros, and riverside evenings.

## Practical info

- **Best time:** May–June or September
- **How to get there:** LIS / OPO hubs
- **Cost / tickets:** Lisboa Card useful for tram days
- **Hours:** Restaurants late; attractions daytime

## Highlights

- Lisbon hills
- Porto riverside

## Visit log

- Visited May 2025 on [[Lisbon and Porto 2025]].

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

- [[Travel]]
- [[Dashboard_Travel]]
