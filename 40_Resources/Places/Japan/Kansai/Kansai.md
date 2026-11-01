---
type: place
place_type: region
status: planned
parent: "[[Japan]]"
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

# Kansai

## Why visit

Kyoto, Nara, and Osaka corridor for temples and departure logistics.

## Practical info

- **Best time:** Early to mid-April
- **How to get there:** Shinkansen from Tokyo; Haruka to KIX
- **Cost / tickets:** Local buses and walking cover most sights
- **Hours:** Temples often close late afternoon

## Highlights

- [[Kyoto]] temples
- [[Nara]] day trip
- [[Osaka]] transit to KIX

## Visit log

- Planned Kansai days in [[Japan Spring 2026]].

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
- [[Travel]]
- [[Dashboard_Travel]]
