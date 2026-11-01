---
type: place
place_type: attraction
status: visited
parent: "[[Lisbon]]"
visited_date: 2025-05-12
rating: 4
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/lisbon-belem.jpg]]"
banner_position: center
---

# Belém Tower

## Why visit

Iconic Tagus landmark; pairs with Pastéis de Belém and Jerónimos.

## Practical info

- **Best time:** Early morning
- **How to get there:** Tram 15 or train to Belém
- **Cost / tickets:** Tower climb queues separately from exterior photos
- **Hours:** Daytime; check Monday closures

## Highlights

- River wind and views
- Combine with pastry queue strategy

## Visit log

- Exterior and area visit 2025-05-12 on [[Lisbon and Porto 2025]].

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

- Parent: [[Lisbon]]
- [[Travel]]
- [[Dashboard_Travel]]
