---
type: place
place_type: city
status: visited
parent: "[[Norte]]"
visited_date: 2025-05-17
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Porto+Portugal"
location: [41.1579, -8.6291]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/porto-bridge.jpg]]"
banner_position: center
---

# Porto

## Dlaczego warto

Zwarte miasto nad rzeką z mocnymi wieczorami i łatwymi degustacjami w Gaia.

## Info praktyczne

- **Najlepszy czas:** Późna wiosna
- **Jak dojechać:** Alfa Pendular z Lizbony; metro do OPO
- **Koszt / bilety:** Jedna degustacja porto wystarczy
- **Godziny:** Loże trzymają dzienne sloty degustacji

## Najważniejsze

- Górny pokład mostu Dom Luís I
- Azulejos na São Bento
- Zachód słońca nad Douro

## Notatki

- Odwiedzono 2025-05-14 do 2025-05-17 na [[Lisbon and Porto 2025]].

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

- Rodzic: [[Norte]]
- [[Ribeira]]
- Mapa: [Porto Portugal](https://www.google.com/maps/search/?api=1&query=Porto+Portugal)
- [[Travel]]
- [[Dashboard_Travel]]
