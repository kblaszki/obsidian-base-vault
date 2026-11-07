---
type: area
status: active
tags:
  - area
  - travel
created_date: 2026-10-27
review_frequency: monthly
---

# Travel

Plan trips, capture day logs, and keep a nested place library (country → region → city → attraction).

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
TABLE WITHOUT ID file.link AS Place, place_type AS Kind, parent AS Parent
FROM "40_Resources/Places"
WHERE type = "place" AND status = "wishlist"
SORT place_type ASC, file.name ASC
```

## Recently visited

```dataview
TABLE WITHOUT ID file.link AS Place, place_type AS Kind, parent AS Parent, visited_date AS Visited, rating AS Rating
FROM "40_Resources/Places"
WHERE type = "place" AND status = "visited"
SORT visited_date DESC
LIMIT 10
```

## Standards

- Create trips with **New Trip**; QuickAdd creates a Folder Note at `20_Projects/Trips/<Trip>/<Trip>.md` plus `days/`, `tips/`, `prep/`, and `assets/`.
- Add day notes with **New Trip Day** under `<Trip>/days/` (folder name = trip title).
- Add tips with **New Trip Tip** under `<Trip>/tips/` and prep with **New Trip Prep** under `<Trip>/prep/`.
- For undated trip drafts, use `Day 01.md` … and `day_number` until dates are booked.
- Capture containers with **New Place (container)** (`Name/Name.md` folder notes) and attractions with **New Place (attraction)** inside the parent folder; always set `parent` except on countries.
- Every place should have `map_url` (Google Maps for phone use) and `location: [lat, lng]` (Map View pins).
- Link places from trip and trip-day notes instead of duplicating logistics.
- Capture food memories with **New Recipe** under `40_Resources/Recipes`; link recipes to places and trips.

## Related

- [[Dashboard_Travel]]
- [[Onigiri]]
- [[Cacio e Pepe]]
- [[Pastéis de Nata]]
