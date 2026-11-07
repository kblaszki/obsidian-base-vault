---
type: place
place_type: city
status: visited
parent: "[[Scotland]]"
visited_date: 2025-08-03
rating: 4
map_url: "https://www.google.com/maps/search/?api=1&query=Edinburgh+Scotland"
location: [55.9533, -3.1883]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/edinburgh-castle.jpg]]"
banner_position: center
---

# Edinburgh

## Dlaczego warto

Mocny miejski start przed jazdą w Highlands na [[Scottish Highlands 2025]].

## Info praktyczne

- **Najlepszy czas:** Unikaj szczytu festiwalu, jeśli chcesz ciszy; sierpień jest żywy
- **Jak dojechać:** Tramwaj EDI
- **Koszt / bilety:** Timed entry do zamku
- **Godziny:** Długie letnie światło

## Najważniejsze

- Royal Mile
- Widoki zamku
- Uliczki kawiarni New Town

## Notatki

- Odwiedzono 2025-08-02 do 2025-08-04 na [[Scottish Highlands 2025]].

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

- Rodzic: [[Scotland]]
- Mapa: [Edinburgh Scotland](https://www.google.com/maps/search/?api=1&query=Edinburgh+Scotland)
- [[Travel]]
- [[Dashboard_Travel]]
