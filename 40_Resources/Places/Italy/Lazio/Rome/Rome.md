---
type: place
place_type: city
status: visited
parent: "[[Lazio]]"
visited_date: 2024-09-11
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Rome+Italy"
location: [41.9028, 12.4964]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/rome-pantheon.jpg]]"
banner_position: center
---

# Rome

## Dlaczego warto

Gęstość zabytków stolicy; baza na [[Colosseum]] i [[Pantheon]] podczas [[Rome and Florence 2024]].

## Info praktyczne

- **Najlepszy czas:** Wiosna lub wczesna jesień
- **Jak dojechać:** FCO + Leonardo Express / taksówki
- **Koszt / bilety:** Timed entry niezbędne przy dużych obiektach
- **Godziny:** Kościoły często zamykane w południe

## Najważniejsze

- Spacery Centro Storico
- Wieczory w Trastevere
- Forum + Palatyn w parze z Koloseum

## Notatki

- Odwiedzono 2024-09-08 do 2024-09-12 na [[Rome and Florence 2024]].

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

- Rodzic: [[Lazio]]
- [[Colosseum]]
- [[Pantheon]]
- Mapa: [Rome Italy](https://www.google.com/maps/search/?api=1&query=Rome+Italy)
- [[Travel]]
- [[Dashboard_Travel]]
