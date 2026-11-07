---
type: place
place_type: region
status: wishlist
parent: "[[Iceland]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=South+Iceland"
location: [63.4194, -19.0066]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/skogafoss.jpg]]"
banner_position: center
---

# South Iceland

## Dlaczego warto

Wodospady, czarne plaże i podejścia do lodowców — kluczowy odcinek krajobrazowy.

## Info praktyczne

- **Najlepszy czas:** Unikaj szczytów sztormów, jeśli się da
- **Jak dojechać:** Route 1 na wschód z Reykjaviku / Selfoss
- **Koszt / bilety:** Dominują parking i paliwo
- **Godziny:** Outdoor; respektuj strefy sneaker-wave

## Najważniejsze

- [[South Coast]]
- [[Blue Lagoon]]

## Notatki

- Szkic dni 04–05 na [[Iceland Ring Road]].

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

- Rodzic: [[Iceland]]
- Mapa: [South Iceland](https://www.google.com/maps/search/?api=1&query=South+Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
