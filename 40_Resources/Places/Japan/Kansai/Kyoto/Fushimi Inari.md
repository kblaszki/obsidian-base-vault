---
type: place
place_type: attraction
status: wishlist
parent: "[[Kyoto]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Fushimi+Inari+Taisha+Kyoto"
location: [34.9671, 135.7727]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/kyoto-fushimi.jpg]]"
banner_position: center
---

# Fushimi Inari

## Why visit

Iconic torii gates above Kyoto; high priority for [[Japan Spring 2026]].

## Practical info

- **Best time:** Before 08:00
- **How to get there:** JR Inari Station
- **Cost / tickets:** Free shrine grounds
- **Hours:** Open 24 hours; shops vary

## Highlights

- Lower gate path
- Optional higher hike

## Visit log

- Planned early visit on 2026-04-15 in [[Japan Spring 2026]].

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

- Parent: [[Kyoto]]
- Map: [Fushimi Inari Taisha Kyoto](https://www.google.com/maps/search/?api=1&query=Fushimi+Inari+Taisha+Kyoto)
- [[Travel]]
- [[Dashboard_Travel]]
