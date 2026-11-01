---
type: place
place_type: attraction
status: visited
parent: "[[Porto]]"
visited_date: 2025-05-15
rating: 5
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
---

# Ribeira

## Why visit

Historic riverfront district; best Porto evening atmosphere.

## Practical info

- **Best time:** Dusk
- **How to get there:** Walk from São Bento / Dom Luís bridge
- **Cost / tickets:** Free to wander; cruises optional
- **Hours:** Always open; restaurants busy after 19:00

## Highlights

- Colored façades
- Crossing to Gaia for tastings

## Visit log

- Multiple evenings during [[Lisbon and Porto 2025]].

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

- Parent: [[Porto]]
- [[Travel]]
- [[Dashboard_Travel]]
