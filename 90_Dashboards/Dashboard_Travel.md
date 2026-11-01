---
type: dashboard
tags:
  - dashboard
  - travel
---

# Travel

## Upcoming and undated trips

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
  AND status != "completed"
  AND (
    !start_date
    OR status = "planned"
    OR status = "active"
    OR date(start_date) >= date(today)
  )
SORT start_date ASC
```

## Completed trips

```dataview
TABLE WITHOUT ID
  file.link AS Trip,
  start_date AS Start,
  end_date AS End,
  countries AS Countries
FROM "20_Projects/Trips"
WHERE type = "trip" AND status = "completed"
SORT start_date DESC
```

## Trip days

```dataview
TABLE WITHOUT ID
  file.link AS Day,
  trip AS Trip,
  date AS Date,
  day_number AS DayNum
FROM "20_Projects/Trips"
WHERE type = "trip-day"
SORT date DESC, day_number DESC
LIMIT 25
```

## Places by kind

```dataview
TABLE WITHOUT ID
  file.link AS Place,
  place_type AS Kind,
  parent AS Parent,
  status AS Status
FROM "40_Resources/Places"
WHERE type = "place"
SORT place_type ASC, file.name ASC
```

## Wishlist

```dataview
TABLE WITHOUT ID
  file.link AS Place,
  place_type AS Kind,
  parent AS Parent
FROM "40_Resources/Places"
WHERE type = "place" AND status = "wishlist"
SORT place_type ASC, file.name ASC
```

## Visited

```dataview
TABLE WITHOUT ID
  file.link AS Place,
  place_type AS Kind,
  parent AS Parent,
  visited_date AS Visited,
  rating AS Rating
FROM "40_Resources/Places"
WHERE type = "place" AND status = "visited"
SORT visited_date DESC
```

## Navigate

- [[Travel]]
- [[Home]]
