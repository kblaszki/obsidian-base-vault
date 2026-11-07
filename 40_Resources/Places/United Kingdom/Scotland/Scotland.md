---
type: place
place_type: region
status: visited
parent: "[[United Kingdom]]"
visited_date: 2025-08-09
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Scotland"
location: [56.4907, -4.2026]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/glencoe.jpg]]"
banner_position: center
---

# Scotland

## Dlaczego warto

Korytarz Highlands i wysp na [[Scottish Highlands 2025]].

## Info praktyczne

- **Najlepszy czas:** Miesiące długiego dnia
- **Jak dojechać:** EDI + wynajem auta
- **Koszt / bilety:** Częste parking honesty boxes
- **Godziny:** Outdoor zależny od pogody

## Najważniejsze

- Miejski start [[Edinburgh]]
- Klify [[Isle of Skye]]
- Dolina [[Glencoe]]

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

- Rodzic: [[United Kingdom]]
- Mapa: [Scotland](https://www.google.com/maps/search/?api=1&query=Scotland)
- [[Travel]]
- [[Dashboard_Travel]]
