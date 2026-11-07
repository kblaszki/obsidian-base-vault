---
type: place
place_type: region
status: visited
parent: "[[Portugal]]"
visited_date: 2025-05-13
rating: 4
map_url: "https://www.google.com/maps/search/?api=1&query=Lisbon+District+Portugal"
location: [38.7223, -9.1393]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/lisbon-view.jpg]]"
banner_position: center
---

# Lisboa District

## Why visit

Greater Lisbon area including Belém day trips.

## Practical info

- **Best time:** May–June or September
- **How to get there:** LIS metro into Baixa-Chiado
- **Cost / tickets:** Lisboa Card useful
- **Hours:** Attractions daytime

## Highlights

- [[Lisbon]]
- [[Belém Tower]]

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
- Map: [Lisbon District Portugal](https://www.google.com/maps/search/?api=1&query=Lisbon+District+Portugal)
- [[Travel]]
- [[Dashboard_Travel]]
