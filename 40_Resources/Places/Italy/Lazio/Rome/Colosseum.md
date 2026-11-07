---
type: place
place_type: attraction
status: visited
parent: "[[Rome]]"
visited_date: 2024-09-09
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Colosseum+Rome"
location: [41.8902, 12.4922]
source_url:
created_date: 2026-10-27
tags:
  - travel
  - place
  - topic/history
banner: "[[./assets/rome-colosseum.jpg]]"
banner_position: center
---

# Colosseum

## Dlaczego warto

Kluczowy zabytek Rzymu i główna ruina plenerowa z [[Rome and Florence 2024]].

## Info praktyczne

- **Najlepszy czas:** Najwcześniejszy timed entry
- **Jak dojechać:** Metro Colosseo
- **Koszt / bilety:** Rezerwuj timed entry z combo Forum/Palatine
- **Godziny:** Sezonowe last admission wcześniej niż godzina zamknięcia

## Najważniejsze

- Widoki z poziomu areny, gdy w bilecie
- Połącz z Forum i Palatynem tego samego poranka

## Notatki

- Odwiedzono 2024-09-09 na [[Rome and Florence 2024]]; mimo timed ticket kolejka ~25 minut.

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
- Mapa: [Colosseum Rome](https://www.google.com/maps/search/?api=1&query=Colosseum+Rome)
- [[Travel]]
- [[Dashboard_Travel]]
