---
type: place
place_type: city
status: visited
parent: "[[Norte]]"
visited_date: 2025-05-17
rating: 5
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/porto-bridge.jpg]]"
banner_position: center
---

# Porto

## Why visit

Compact riverside city with strong evenings and easy Gaia tastings.

## Practical info

- **Best time:** Late spring
- **How to get there:** Alfa Pendular from Lisbon; metro to OPO
- **Cost / tickets:** One port tasting is enough
- **Hours:** Lodges keep daytime tasting slots

## Highlights

- Dom Luís I bridge upper deck
- São Bento tiles
- Sunset on the Douro

## Visit log

- Visited 2025-05-14 to 2025-05-17 on [[Lisbon and Porto 2025]].

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

- Parent: [[Norte]]
- [[Ribeira]]
- [[Travel]]
- [[Dashboard_Travel]]
