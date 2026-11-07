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

Planuj wyjazdy, zapisuj dzienniki dni i prowadź zagnieżdżoną bibliotekę miejsc (kraj → region → miasto → atrakcja).

## Otwarte wyjazdy

Obejmuje datowane nadchodzące wyjazdy oraz szkice bez daty (puste `start_date`).

```dataview
TABLE status AS Status, start_date AS Start, end_date AS Koniec, countries AS Kraje
FROM "20_Projects/Trips"
WHERE type = "trip" AND status != "completed" AND status != "cancelled"
SORT start_date ASC
```

## Ukończone wyjazdy

```dataview
TABLE start_date AS Start, end_date AS Koniec, countries AS Kraje
FROM "20_Projects/Trips"
WHERE type = "trip" AND status = "completed"
SORT start_date DESC
```

## Miejsca z listy życzeń

```dataview
TABLE WITHOUT ID file.link AS Miejsce, place_type AS Rodzaj, parent AS Rodzic
FROM "40_Resources/Places"
WHERE type = "place" AND status = "wishlist"
SORT place_type ASC, file.name ASC
```

## Ostatnio odwiedzone

```dataview
TABLE WITHOUT ID file.link AS Miejsce, place_type AS Rodzaj, parent AS Rodzic, visited_date AS Odwiedzono, rating AS Ocena
FROM "40_Resources/Places"
WHERE type = "place" AND status = "visited"
SORT visited_date DESC
LIMIT 10
```

## Standardy

- Twórz wyjazdy przez **Nowy wyjazd**; QuickAdd robi Folder Note w `20_Projects/Trips/<Trip>/<Trip>.md` oraz foldery `days/`, `tips/`, `prep/`, `assets/`.
- Dni dodawaj przez **Nowy dzień wyjazdu** w `<Trip>/days/` (nazwa folderu = tytuł wyjazdu).
- Wskazówki: **Nowa wskazówka wyjazdu** w `<Trip>/tips/`; przygotowanie: **Nowe przygotowanie wyjazdu** w `<Trip>/prep/`.
- W szkicach bez dat używaj `Day 01.md` … oraz `day_number`, aż daty będą znane.
- Kontenery miejsc: **Nowe miejsce (kontener)** (`Name/Name.md`); atrakcje: **Nowe miejsce (atrakcja)** w folderze rodzica; zawsze ustawiaj `parent` poza krajami.
- Każde miejsce powinno mieć `map_url` (Google Maps na telefon) i `location: [lat, lng]` (pinezki Map View).
- Linkuj miejsca z notatek wyjazdu i dni zamiast powielać logistykę.
- Wspomnienia kulinarne zapisuj przez **Nowy przepis** w `40_Resources/Recipes`; łącz przepisy z miejscami i wyjazdami.

## Powiązane

- [[Dashboard_Travel]]
