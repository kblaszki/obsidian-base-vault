---
type: place
place_type: region
status: visited
parent: "[[Portugal]]"
visited_date: 2025-05-17
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Norte+Portugal"
location: [41.1579, -8.6291]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/porto-bridge.jpg]]"
banner_position: center
---

# Norte

## Why visit

Northern Portugal with Porto as the riverside hub.

## Practical info

- **Best time:** Late spring
- **How to get there:** Alfa Pendular from Lisbon; metro to OPO
- **Cost / tickets:** Port tasting slots
- **Hours:** Lodges keep daytime tasting slots

## Highlights

- [[Porto]]
- [[Ribeira]]

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

- Parent: [[Portugal]]
- Map: [Norte Portugal](https://www.google.com/maps/search/?api=1&query=Norte+Portugal)
- [[Travel]]
- [[Dashboard_Travel]]
