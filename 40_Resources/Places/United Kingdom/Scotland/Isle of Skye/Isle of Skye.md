---
type: place
place_type: region
status: visited
parent: "[[Scotland]]"
visited_date: 2025-08-06
rating: 5
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/skye-storr.jpg]]"
banner_position: center
---

# Isle of Skye

## Why visit

Dramatic cliffs and short walks; scenic peak of [[Scottish Highlands 2025]].

## Practical info

- **Best time:** Long daylight months
- **How to get there:** Rental car via Kyle of Lochalsh
- **Cost / tickets:** Mostly parking honesty boxes
- **Hours:** Outdoor; weather dependent

## Highlights

- Old Man of Storr
- Kilt Rock
- Neist Point

## Visit log

- Base in Portree 2025-08-04 to 2025-08-07 on [[Scottish Highlands 2025]].

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

- Parent: [[Scotland]]
- [[Travel]]
- [[Dashboard_Travel]]
