---
type: place
place_type: city
status: visited
parent: "[[Lisboa District]]"
visited_date: 2025-05-13
rating: 4
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
---

# Lisbon

## Why visit

Hills, miradouros, and Belém day trips; energetic base for [[Lisbon and Porto 2025]].

## Practical info

- **Best time:** May–June or September
- **How to get there:** LIS metro into Baixa-Chiado
- **Cost / tickets:** Lisboa Card useful for tram days
- **Hours:** Restaurants late; attractions standard daytime

## Highlights

- Alfama lanes
- Tram 28 strategy (walk more than ride)
- LX Factory coffee morning

## Visit log

- Visited 2025-05-10 to 2025-05-14 on [[Lisbon and Porto 2025]].

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

- Parent: [[Lisboa District]]
- [[Belém Tower]]
- [[Travel]]
- [[Dashboard_Travel]]
