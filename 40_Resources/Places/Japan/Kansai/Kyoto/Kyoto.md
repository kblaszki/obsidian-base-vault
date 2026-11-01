---
type: place
place_type: city
status: planned
parent: "[[Kansai]]"
visited_date:
rating:
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/kyoto-temple.jpg]]"
banner_position: center
---

# Kyoto

## Why visit

Temple circuits and quieter evenings after Tokyo during [[Japan Spring 2026]].

## Practical info

- **Best time:** Early to mid-April
- **How to get there:** Shinkansen from Tokyo
- **Cost / tickets:** Local buses and walking cover most sights
- **Hours:** Temples often close late afternoon

## Highlights

- [[Fushimi Inari]]
- Gion evenings
- Arashiyama

## Visit log

- Planned Kyoto days in [[Japan Spring 2026]].

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
- [[Fushimi Inari]]
- [[Nara]]
- [[Travel]]
- [[Dashboard_Travel]]
