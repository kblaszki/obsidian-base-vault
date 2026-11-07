---
type: place
place_type: city
status: wishlist
parent: "[[Capital Region]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Reykjavik+Iceland"
location: [64.1466, -21.9426]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/reykjavik.jpg]]"
banner_position: center
---

# Reykjavik

## Why visit

Compact capital base for gear checks and rest before South Coast drives on [[Iceland Ring Road]].

## Practical info

- **Best time:** Late spring to early autumn for easier driving
- **How to get there:** KEF + Flybus or rental car
- **Cost / tickets:** City food is expensive; grocery breakfasts help
- **Hours:** Extreme daylight seasonality

## Highlights

- Harbor and Harpa
- Laugavegur gear shops
- Easy first/last nights

## Visit log

- Wishlist base for [[Iceland Ring Road]] (dates TBD).

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

- Parent: [[Capital Region]]
- Map: [Reykjavik Iceland](https://www.google.com/maps/search/?api=1&query=Reykjavik+Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
