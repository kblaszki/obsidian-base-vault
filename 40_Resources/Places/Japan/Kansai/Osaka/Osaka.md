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
---

# Osaka

## Why visit

Transit hub toward KIX on the final day of [[Japan Spring 2026]].

## Practical info

- **Best time:** Pass-through or food stop
- **How to get there:** Rail from Kyoto; Haruka to KIX
- **Cost / tickets:** IC cards work
- **Hours:** Airport trains frequent

## Highlights

- Airport transfer logistics
- Optional food stop if schedule allows

## Visit log

- Planned departure transit 2026-04-18 on [[Japan Spring 2026]].

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
- [[Travel]]
- [[Dashboard_Travel]]
