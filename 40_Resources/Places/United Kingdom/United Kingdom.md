---
type: place
place_type: country
status: visited
parent:
visited_date: 2025-08-09
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=United+Kingdom"
location: [55.9533, -3.1883]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/edinburgh-castle.jpg]]"
banner_position: center
---

# United Kingdom

## Dlaczego warto

Baza road trip’u Highlands przez Edynburg.

## Info praktyczne

- **Najlepszy czas:** Letnie miesiące długiego dnia
- **Jak dojechać:** EDI na starty w Szkocji
- **Koszt / bilety:** Wynajem auta niezbędny w Highlands
- **Godziny:** Długie letnie światło

## Najważniejsze

- [[Edinburgh]]
- [[Isle of Skye]]
- [[Glencoe]]

## Notatki

- Odwiedzono w sierpniu 2025 na [[Scottish Highlands 2025]].

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

- Mapa: [United Kingdom](https://www.google.com/maps/search/?api=1&query=United+Kingdom)
- [[Travel]]
- [[Dashboard_Travel]]
