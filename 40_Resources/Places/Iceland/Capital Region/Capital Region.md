---
type: place
place_type: region
status: wishlist
parent: "[[Iceland]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Reykjavik+Capital+Region+Iceland"
location: [64.1466, -21.9426]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/reykjavik.jpg]]"
banner_position: center
---

# Capital Region

## Why visit

Reykjavik and airport logistics for ring-road starts and ends.

## Practical info

- **Best time:** Late spring to early autumn
- **How to get there:** KEF + Flybus or rental car
- **Cost / tickets:** City food is expensive
- **Hours:** Extreme daylight seasonality

## Highlights

- [[Reykjavik]]

## Visit log

- Wishlist base for [[Iceland Ring Road]].

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
- Map: [Reykjavik Capital Region Iceland](https://www.google.com/maps/search/?api=1&query=Reykjavik+Capital+Region+Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
