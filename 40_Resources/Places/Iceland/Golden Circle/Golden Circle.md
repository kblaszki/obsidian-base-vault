---
type: place
place_type: region
status: planned
parent: "[[Iceland]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Gullfoss+Golden+Circle+Iceland"
location: [64.3271, -20.1211]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/gullfoss.jpg]]"
banner_position: center
---

# Golden Circle

## Why visit

Highest-yield day loop from Reykjavik: rift valley, geysers, and waterfall.

## Practical info

- **Best time:** Start early to beat buses
- **How to get there:** Rental car day loop
- **Cost / tickets:** Mostly free viewpoints; parking fees vary
- **Hours:** Daylight dependent

## Highlights

- Þingvellir
- Geysir area
- Gullfoss

## Visit log

- Draft Day 03 on [[Iceland Ring Road]].

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

- Parent: [[Iceland]]
- [[Reykjavik]]
- Map: [Gullfoss Golden Circle Iceland](https://www.google.com/maps/search/?api=1&query=Gullfoss+Golden+Circle+Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
