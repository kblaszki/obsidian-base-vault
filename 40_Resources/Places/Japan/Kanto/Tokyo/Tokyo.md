---
type: place
place_type: city
status: planned
parent: "[[Kanto]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Tokyo+Japan"
location: [35.6762, 139.6503]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/tokyo-skyline.jpg]]"
banner_position: center
---

# Tokyo

## Why visit

Dense neighborhoods and blossom parks; first base for [[Japan Spring 2026]].

## Practical info

- **Best time:** Late March to mid-April for blossoms
- **How to get there:** NRT/HND + rail into Shinjuku
- **Cost / tickets:** Suica for local transit
- **Hours:** Neighborhood dependent

## Highlights

- Shinjuku evenings
- Meiji Shrine / Harajuku
- Asakusa morning

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

- Parent: [[Kanto]]
- Map: [Tokyo Japan](https://www.google.com/maps/search/?api=1&query=Tokyo+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
