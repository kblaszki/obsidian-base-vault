---
type: place
place_type: attraction
status: visited
parent: "[[Scotland]]"
visited_date: 2025-08-08
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Glencoe+Scotland"
location: [56.682, -5.102]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/glencoe.jpg]]"
banner_position: center
---

# Glencoe

## Why visit

Highland valley drama and easy roadside viewpoints.

## Practical info

- **Best time:** Clear spells between rain bands
- **How to get there:** A82 corridor by car
- **Cost / tickets:** Parking fees at popular lots
- **Hours:** Daylight hiking only unless equipped

## Highlights

- Three Sisters viewpoints
- Buachaille Etive Mòr approaches
- Kingshouse area light

## Visit log

- Overnight and walks 2025-08-07 to 2025-08-09 on [[Scottish Highlands 2025]].

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

- Parent: [[Scotland]]
- Map: [Glencoe Scotland](https://www.google.com/maps/search/?api=1&query=Glencoe+Scotland)
- [[Travel]]
- [[Dashboard_Travel]]
