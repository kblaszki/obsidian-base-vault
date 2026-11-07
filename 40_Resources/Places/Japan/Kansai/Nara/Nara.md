---
type: place
place_type: city
status: planned
parent: "[[Kansai]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Nara+Japan"
location: [34.6851, 135.8048]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/nara-deer.jpg]]"
banner_position: center
---

# Nara

## Why visit

Easy day trip from Kyoto for Tōdai-ji and park walks.

## Practical info

- **Best time:** Morning arrival from Kyoto
- **How to get there:** JR or Kintetsu from Kyoto
- **Cost / tickets:** Temple fees modest
- **Hours:** Day-trip friendly

## Highlights

- Tōdai-ji
- Deer park etiquette

## Visit log

- Planned day trip 2026-04-16 on [[Japan Spring 2026]].

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

- Parent: [[Kansai]]
- [[Kyoto]]
- Map: [Nara Japan](https://www.google.com/maps/search/?api=1&query=Nara+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
