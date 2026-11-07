---
type: place
place_type: region
status: visited
parent: "[[Portugal]]"
visited_date: 2025-05-13
rating: 4
map_url: "https://www.google.com/maps/search/?api=1&query=Lisbon+District+Portugal"
location: [38.7223, -9.1393]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/lisbon-view.jpg]]"
banner_position: center
---

# Lisboa District

## Dlaczego warto

Większy obszar Lizbony, w tym jednodniówki do Belém.

## Info praktyczne

- **Najlepszy czas:** Maj–czerwiec lub wrzesień
- **Jak dojechać:** Metro z LIS do Baixa-Chiado
- **Koszt / bilety:** Lisboa Card bywa przydatna
- **Godziny:** Atrakcje w dzień

## Najważniejsze

- [[Lisbon]]
- [[Belém Tower]]

## Notatki

- Odwiedzono w maju 2025 na [[Lisbon and Porto 2025]].

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

- Rodzic: [[Portugal]]
- Mapa: [Lisbon District Portugal](https://www.google.com/maps/search/?api=1&query=Lisbon+District+Portugal)
- [[Travel]]
- [[Dashboard_Travel]]
