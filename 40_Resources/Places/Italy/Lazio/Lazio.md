---
type: place
place_type: region
status: visited
parent: "[[Italy]]"
visited_date: 2024-09-11
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Lazio+Italy"
location: [41.9028, 12.4964]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/rome-colosseum.jpg]]"
banner_position: center
---

# Lazio

## Dlaczego warto

Rzym i okoliczne Lazio; stolica gęsta od zabytków.

## Info praktyczne

- **Najlepszy czas:** Wiosna lub wczesna jesień
- **Jak dojechać:** FCO + Leonardo Express
- **Koszt / bilety:** Timed entry niezbędne
- **Godziny:** Kościoły często zamykane w południe

## Najważniejsze

- Historyczne centrum [[Rome]]

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
- Mapa: [Lazio Italy](https://www.google.com/maps/search/?api=1&query=Lazio+Italy)
- [[Travel]]
- [[Dashboard_Travel]]
