---
type: dashboard
tags:
  - dashboard
  - travel
---

# Travel

## Upcoming trips

```dataview
TABLE WITHOUT ID
  file.link AS Trip,
  status AS Status,
  start_date AS Start,
  end_date AS End,
  countries AS Countries
FROM "20_Projects/Trips"
WHERE type = "trip"
  AND status != "cancelled"
  AND (status = "planned" OR status = "active" OR (start_date AND date(start_date) >= date(today)))
SORT start_date ASC
```

## Trip days

```dataview
TABLE WITHOUT ID
  file.link AS Day,
  trip AS Trip,
  date AS Date
FROM "20_Projects/Trips"
WHERE type = "trip-day"
SORT date DESC
LIMIT 20
```

## Places by country

```dataview
TABLE WITHOUT ID
  key AS Country,
  rows.file.link AS Places,
  rows.place_type AS Kind,
  rows.status AS Status
FROM "40_Resources/Places"
WHERE type = "place"
GROUP BY country
SORT key ASC
```

## Wishlist

```dataview
LIST
FROM "40_Resources/Places"
WHERE type = "place" AND status = "wishlist"
SORT country ASC, file.name ASC
```

## Visited

```dataview
TABLE country AS Country, city AS City, visited_date AS Visited, rating AS Rating
FROM "40_Resources/Places"
WHERE type = "place" AND status = "visited"
SORT visited_date DESC
```

## Navigate

- [[Travel]]
- [[Home]]
