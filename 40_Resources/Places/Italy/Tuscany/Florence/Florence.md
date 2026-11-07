---
type: place
place_type: city
status: visited
parent: "[[Tuscany]]"
visited_date: 2024-09-15
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Florence+Italy"
location: [43.7696, 11.2558]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/florence-duomo.jpg]]"
banner_position: center
---

# Florence

## Dlaczego warto

Renesansowe centrum ze spacerowymi wieczorami i [[Uffizi]] jako kotwicą muzealną.

## Info praktyczne

- **Najlepszy czas:** Sezony przejściowe
- **Jak dojechać:** Freccia z Rzymu; lotnisko FLR przy wylocie
- **Koszt / bilety:** Rezerwuj Uffizi z wyprzedzeniem
- **Godziny:** Wiele obiektów zamyka się wcześniej, niż sugeruje nocne życie Rzymu

## Najważniejsze

- Oltrarno
- Zachód słońca z Piazzale Michelangelo
- Ponte Vecchio (licz się z tłumami)

## Notatki

- Odwiedzono 2024-09-12 do 2024-09-15 na [[Rome and Florence 2024]].

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

- Rodzic: [[Tuscany]]
- [[Uffizi]]
- Mapa: [Florence Italy](https://www.google.com/maps/search/?api=1&query=Florence+Italy)
- [[Travel]]
- [[Dashboard_Travel]]
