---
type: place
place_type: region
status: visited
parent: "[[Scotland]]"
visited_date: 2025-08-06
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Isle+of+Skye+Scotland"
location: [57.5359, -6.2263]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/skye-storr.jpg]]"
banner_position: center
---

# Isle of Skye

## Dlaczego warto

Dramatyczne klify i krótkie spacery; krajobrazowy szczyt [[Scottish Highlands 2025]].

## Info praktyczne

- **Najlepszy czas:** Miesiące długiego dnia
- **Jak dojechać:** Wynajem auta przez Kyle of Lochalsh
- **Koszt / bilety:** Głównie parking honesty boxes
- **Godziny:** Outdoor; zależne od pogody

## Najważniejsze

- Old Man of Storr
- Kilt Rock
- Neist Point

## Notatki

- Baza w Portree 2025-08-04 do 2025-08-07 na [[Scottish Highlands 2025]].

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
- Mapa: [Isle of Skye Scotland](https://www.google.com/maps/search/?api=1&query=Isle+of+Skye+Scotland)
- [[Travel]]
- [[Dashboard_Travel]]
