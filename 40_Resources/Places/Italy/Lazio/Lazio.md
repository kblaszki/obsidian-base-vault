---
type: place
place_type: region
status: visited
parent: "[[Italy]]"
visited_date: 2024-09-11
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

# Lazio

## Why visit

Rome and surrounding Lazio; capital density of landmarks.

## Practical info

- **Best time:** Spring or early autumn
- **How to get there:** FCO + Leonardo Express
- **Cost / tickets:** Timed entries essential
- **Hours:** Churches often close midday

## Highlights

- [[Rome]] historic center

## Visit log

- Visited September 2024 on [[Rome and Florence 2024]].

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

- Parent: [[Italy]]
- [[Travel]]
- [[Dashboard_Travel]]
