---
type: place
place_type: attraction
status: visited
parent: "[[Rome]]"
visited_date: 2024-09-08
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Pantheon+Rome"
location: [41.8986, 12.4769]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/rome-pantheon.jpg]]"
banner_position: center
---

# Pantheon

## Dlaczego warto

Najlepiej zachowana starożytna kopuła w centrum Rzymu.

## Info praktyczne

- **Najlepszy czas:** Wieczorem z zewnątrz; rano wnętrze, jeśli wymagane bilety
- **Jak dojechać:** Spacer z Trevi / Piazza Navona
- **Koszt / bilety:** Sprawdź aktualne zasady wejścia przed wyjazdem
- **Godziny:** Dostęp do wnętrza w dzień

## Najważniejsze

- Światło przez oculus
- Atmosfera placu o zmierzchu

## Notatki

- Spacer wokół i okolica 2024-09-08 podczas [[Rome and Florence 2024]].

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

- Rodzic: [[Rome]]
- Mapa: [Pantheon Rome](https://www.google.com/maps/search/?api=1&query=Pantheon+Rome)
- [[Travel]]
- [[Dashboard_Travel]]
