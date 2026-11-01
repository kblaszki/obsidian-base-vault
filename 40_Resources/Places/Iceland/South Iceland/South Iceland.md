---
type: place
place_type: region
status: wishlist
parent: "[[Iceland]]"
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

# South Iceland

## Why visit

Waterfalls, black sand beaches, and glacier approaches — core scenic stretch.

## Practical info

- **Best time:** Avoid peak storm windows if possible
- **How to get there:** Route 1 east from Reykjavik / Selfoss
- **Cost / tickets:** Parking and fuel dominate
- **Hours:** Outdoor; respect sneaker-wave zones

## Highlights

- [[South Coast]]
- [[Blue Lagoon]]

## Visit log

- Draft Days 04–05 on [[Iceland Ring Road]].

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
- [[Travel]]
- [[Dashboard_Travel]]
