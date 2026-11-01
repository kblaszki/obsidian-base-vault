---
type: place
place_type: country
status: visited
parent:
visited_date: 2025-08-09
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=United+Kingdom"
location: [55.9533, -3.1883]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/edinburgh-castle.jpg]]"
banner_position: center
---

# United Kingdom

## Why visit

Scotland Highlands road trip base via Edinburgh.

## Practical info

- **Best time:** Long daylight summer months
- **How to get there:** EDI for Scotland starts
- **Cost / tickets:** Rental car essential for Highlands
- **Hours:** Long summer daylight

## Highlights

- [[Edinburgh]]
- [[Isle of Skye]]
- [[Glencoe]]

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

- Map: [United Kingdom](https://www.google.com/maps/search/?api=1&query=United+Kingdom)
- [[Travel]]
- [[Dashboard_Travel]]
