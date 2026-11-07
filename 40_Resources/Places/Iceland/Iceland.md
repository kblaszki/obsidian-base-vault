---
type: place
place_type: country
status: wishlist
parent:
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Iceland"
location: [64.1466, -21.9426]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/skogafoss.jpg]]"
banner_position: center
---

# Iceland

## Dlaczego warto

Krajobrazy drogi okrężnej: wybrzeża, geotermia i pętle wodospadów.

## Info praktyczne

- **Najlepszy czas:** Późna wiosna do wczesnej jesieni — łatwiejsza jazda
- **Jak dojechać:** Hub KEF
- **Koszt / bilety:** Dominują wynajem auta i paliwo
- **Godziny:** Ekstremalna sezonowość dnia

## Najważniejsze

- Baza [[Reykjavik]]
- [[South Coast]]
- [[Golden Circle]]

## Notatki

- Szkic itinerariusza na [[Iceland Ring Road]] (daty TBD).

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

- Mapa: [Iceland](https://www.google.com/maps/search/?api=1&query=Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
