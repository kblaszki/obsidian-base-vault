---
type: place
place_type: attraction
status: visited
parent: "[[Florence]]"
visited_date: 2024-09-13
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Uffizi+Gallery+Florence"
location: [43.7678, 11.2553]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/uffizi.jpg]]"
banner_position: center
---

# Uffizi

## Why visit

Essential painting collection; morning slots reduce fatigue.

## Practical info

- **Best time:** Opening slot
- **How to get there:** Walk from historic center hotels
- **Cost / tickets:** Timed entry mandatory in peak season
- **Hours:** Closed Mondays historically — verify

## Highlights

- Corridor rhythm if you move steadily
- Botticelli rooms

## Visit log

- Timed morning visit 2024-09-13 on [[Rome and Florence 2024]].

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

- Parent: [[Florence]]
- Map: [Uffizi Gallery Florence](https://www.google.com/maps/search/?api=1&query=Uffizi+Gallery+Florence)
- [[Travel]]
- [[Dashboard_Travel]]
