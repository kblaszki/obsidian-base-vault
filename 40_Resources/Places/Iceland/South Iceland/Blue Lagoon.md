---
type: place
place_type: attraction
status: wishlist
parent: "[[South Iceland]]"
visited_date:
rating:
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/blue-lagoon.jpg]]"
banner_position: center
---

# Blue Lagoon

## Why visit

Optional spa buffer day near KEF; book ahead or consider Sky Lagoon instead.

## Practical info

- **Best time:** Flex day before departure
- **How to get there:** Bus packages or rental car near KEF
- **Cost / tickets:** Expensive; prebook
- **Hours:** Session slots

## Highlights

- Geothermal soak
- Convenient with airport logistics

## Visit log

- Optional Day 06 on [[Iceland Ring Road]].

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

- Parent: [[South Iceland]]
- [[Reykjavik]]
- [[Travel]]
- [[Dashboard_Travel]]
