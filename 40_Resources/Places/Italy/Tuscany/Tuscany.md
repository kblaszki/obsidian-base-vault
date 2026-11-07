---
type: place
place_type: region
status: visited
parent: "[[Italy]]"
visited_date: 2024-09-15
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Tuscany+Italy"
location: [43.7711, 11.2486]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/florence-skyline.jpg]]"
banner_position: center
---

# Tuscany

## Dlaczego warto

Florencja i okoliczny renesansowy rdzeń.

## Info praktyczne

- **Najlepszy czas:** Sezony przejściowe
- **Jak dojechać:** Freccia z Rzymu; lotnisko FLR
- **Koszt / bilety:** Rezerwuj Uffizi z wyprzedzeniem
- **Godziny:** Wiele obiektów zamyka się wcześniej, niż sugeruje nocne życie Rzymu

## Najważniejsze

- [[Florence]]
- [[Uffizi]]

## Notatki

- Odwiedzono we wrześniu 2024 na [[Rome and Florence 2024]].

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

- Rodzic: [[Italy]]
- Mapa: [Tuscany Italy](https://www.google.com/maps/search/?api=1&query=Tuscany+Italy)
- [[Travel]]
- [[Dashboard_Travel]]
