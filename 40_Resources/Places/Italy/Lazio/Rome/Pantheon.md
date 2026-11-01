---
type: place
place_type: attraction
status: visited
parent: "[[Rome]]"
visited_date: 2024-09-08
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Pantheon+Rome"
location: [41.8986, 12.4769]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/rome-pantheon.jpg]]"
banner_position: center
---

# Pantheon

## Why visit

Best preserved ancient dome experience in central Rome.

## Practical info

- **Best time:** Evening exterior; morning interior if tickets required
- **How to get there:** Walk from Trevi / Piazza Navona
- **Cost / tickets:** Check current entry rules before travel
- **Hours:** Daytime interior access

## Highlights

- Oculus light
- Piazza atmosphere at dusk

## Visit log

- Exterior and area walk on 2024-09-08 during [[Rome and Florence 2024]].

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

- Parent: [[Rome]]
- Map: [Pantheon Rome](https://www.google.com/maps/search/?api=1&query=Pantheon+Rome)
- [[Travel]]
- [[Dashboard_Travel]]
