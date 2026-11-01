---
type: place
place_type: country
status: wishlist
parent:
visited_date:
rating:
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
---

# Iceland

## Why visit

Ring-road landscapes: coasts, geothermal, and waterfall day loops.

## Practical info

- **Best time:** Late spring to early autumn for easier driving
- **How to get there:** KEF hub
- **Cost / tickets:** Rental car and fuel dominate
- **Hours:** Extreme daylight seasonality

## Highlights

- [[Reykjavik]] base
- [[South Coast]]
- [[Golden Circle]]

## Visit log

- Draft itinerary on [[Iceland Ring Road]] (dates TBD).

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
