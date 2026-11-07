---
type: place
place_type: attraction
status: wishlist
parent: "[[South Iceland]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Blue+Lagoon+Iceland"
location: [63.8804, -22.4495]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/blue-lagoon.jpg]]"
banner_position: center
---

# Blue Lagoon

## Dlaczego warto

Opcjonalny dzień spa w okolicy KEF; rezerwuj z wyprzedzeniem albo rozważ Sky Lagoon.

## Info praktyczne

- **Najlepszy czas:** Elastyczny dzień przed wylotem
- **Jak dojechać:** Pakiety autobusowe lub wynajem auta koło KEF
- **Koszt / bilety:** Drogo; rezerwuj z góry
- **Godziny:** Sloty sesji

## Najważniejsze

- Kąpiel geotermalna
- Wygodne z logistyką lotniska

## Notatki

- Opcjonalny Dzień 06 na [[Iceland Ring Road]].

## Miejsca podrzędne

```dataview
TABLE WITHOUT ID file.link AS Miejsce, place_type AS Rodzaj, status AS Status
FROM "40_Resources/Places"
WHERE parent = this.file.link
SORT place_type ASC, file.name ASC
```

## Wyjazdy

```dataview
LIST
FROM "20_Projects/Trips"
WHERE type = "trip" AND contains(file.outlinks, this.file.link)
SORT start_date DESC
```

## Powiązane

- Rodzic: [[South Iceland]]
- [[Reykjavik]]
- Mapa: [Blue Lagoon Iceland](https://www.google.com/maps/search/?api=1&query=Blue+Lagoon+Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
