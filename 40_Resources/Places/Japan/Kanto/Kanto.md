---
type: place
place_type: region
status: planned
parent: "[[Japan]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Kanto+region+Japan"
location: [35.6762, 139.6503]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/tokyo-skyline.jpg]]"
banner_position: center
---

# Kanto

## Why visit

Greater Tokyo plain; first landing region for [[Japan Spring 2026]].

## Practical info

- **Best time:** Late March to mid-April
- **How to get there:** NRT/HND into Tokyo
- **Cost / tickets:** Suica / Pasmo
- **Hours:** Neighborhood dependent

## Highlights

- [[Tokyo]] neighborhoods
- Day trips within the metro

## Visit log

- Planned Tokyo stay in [[Japan Spring 2026]].

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

- Parent: [[Japan]]
- Map: [Kanto region Japan](https://www.google.com/maps/search/?api=1&query=Kanto+region+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
