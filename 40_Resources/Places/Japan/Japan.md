---
type: place
place_type: country
status: planned
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
banner: "[[./assets/tokyo-skyline.jpg]]"
banner_position: center
---

# Japan

## Why visit

Island nation with dense cities, temple circuits, and spring blossom travel.

## Practical info

- **Best time:** Late March to mid-April for blossoms
- **How to get there:** NRT/HND or KIX
- **Cost / tickets:** Rail Pass or IC + shinkansen tickets
- **Hours:** Temples often close late afternoon

## Highlights

- Tokyo base
- Kansai temple days
- Food and transit etiquette

## Visit log

- Planned April 2026 via [[Japan Spring 2026]].

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
