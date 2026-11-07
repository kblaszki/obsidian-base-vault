---
type: dashboard
tags:
  - dashboard
  - travel
---

# Travel

## Nadchodzące i bez daty

```dataview
TABLE WITHOUT ID
  file.link AS Wyjazd,
  status AS Status,
  start_date AS Start,
  end_date AS Koniec,
  countries AS Kraje
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

## Ukończone wyjazdy

```dataview
TABLE WITHOUT ID
  file.link AS Wyjazd,
  start_date AS Start,
  end_date AS Koniec,
  countries AS Kraje
FROM "20_Projects/Trips"
WHERE type = "trip" AND status = "completed"
SORT start_date DESC
```

## Dni wyjazdów

```dataview
TABLE WITHOUT ID
  file.link AS Dzień,
  trip AS Wyjazd,
  date AS Data,
  day_number AS NrDnia
FROM "20_Projects/Trips"
WHERE type = "trip-day"
SORT date DESC, day_number DESC
LIMIT 25
```

## Mapa miejsc

Osadzony Map View notatek z `40_Resources/Places` (wymaga wtyczki Map View). Pinezki biorą `location`; otwórz pinezkę albo **Open in → Google Maps**. Każde miejsce ma też klikalne `map_url` w sekcji Powiązane.

```mapview
{"name":"Places","query":"path:\"40_Resources/Places\"","autoFit":true,"embeddedHeight":420,"chosenMapSource":0}
```

## Miejsca według rodzaju

```dataview
TABLE WITHOUT ID
  file.link AS Miejsce,
  place_type AS Rodzaj,
  parent AS Rodzic,
  status AS Status,
  map_url AS GoogleMaps
FROM "40_Resources/Places"
WHERE type = "place"
SORT place_type ASC, file.name ASC
```

## Lista życzeń

```dataview
TABLE WITHOUT ID
  file.link AS Miejsce,
  place_type AS Rodzaj,
  parent AS Rodzic,
  map_url AS GoogleMaps
FROM "40_Resources/Places"
WHERE type = "place" AND status = "wishlist"
SORT place_type ASC, file.name ASC
```

## Odwiedzone

```dataview
TABLE WITHOUT ID
  file.link AS Miejsce,
  place_type AS Rodzaj,
  parent AS Rodzic,
  visited_date AS Odwiedzono,
  rating AS Ocena,
  map_url AS GoogleMaps
FROM "40_Resources/Places"
WHERE type = "place" AND status = "visited"
SORT visited_date DESC
```

## Nawigacja

- [[Travel]]
- [[Home]]
