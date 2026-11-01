---
type: area
status: active
tags:
  - area
  - travel
created_date: 2026-10-27
review_frequency: monthly
icon: 🧭
---

# Travel

Plan trips, capture day logs, and keep a reusable place library grouped by country.

## Open trips

Includes dated upcoming trips and undated drafts (empty `start_date`).

```dataview
TABLE status AS Status, start_date AS Start, end_date AS End, countries AS Countries
FROM "20_Projects/Trips"
WHERE type = "trip" AND status != "completed" AND status != "cancelled"
SORT start_date ASC
```

## Completed trips

```dataview
TABLE start_date AS Start, end_date AS End, countries AS Countries
FROM "20_Projects/Trips"
WHERE type = "trip" AND status = "completed"
SORT start_date DESC
```

## Wishlist places

```dataview
TABLE place_type AS Kind, country AS Country, city AS City
FROM "40_Resources/Places"
WHERE type = "place" AND status = "wishlist"
SORT country ASC, file.name ASC
```

## Recently visited

```dataview
TABLE country AS Country, visited_date AS Visited, rating AS Rating
FROM "40_Resources/Places"
WHERE type = "place" AND status = "visited"
SORT visited_date DESC
LIMIT 10
```

## Standards

- Create trips with **New Trip**; keep the trip note in `20_Projects/Trips`.
- Add day notes with **New Trip Day** under `<Trip>/days/` (folder name = trip title).
- Add tips with **New Trip Tip** under `<Trip>/tips/` and prep with **New Trip Prep** under `<Trip>/prep/`.
- For undated trip drafts, use `Day 01.md` … and `day_number` until dates are booked.
- Capture places with **New Place** so they land under `40_Resources/Places/<Country>/`.
- Link places from trip and trip-day notes instead of duplicating logistics.

## Related

- [[Dashboard_Travel]]
