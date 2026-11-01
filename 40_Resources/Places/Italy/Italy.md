---
type: place
place_type: country
status: visited
parent:
visited_date: 2024-09-15
rating: 5
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/rome-colosseum.jpg]]"
banner_position: center
---

# Italy

## Why visit

Dense historic cities with strong food culture; base for [[Rome and Florence 2024]].

## Practical info

- **Best time:** Spring or early autumn
- **How to get there:** FCO / FLR hubs
- **Cost / tickets:** Timed entries essential for big sites
- **Hours:** Churches often close midday

## Highlights

- Rome landmarks
- Florence museums

## Visit log

- Visited 2024-09-08 to 2024-09-15 on [[Rome and Florence 2024]].

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
