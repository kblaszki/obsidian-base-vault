---
type: place
place_type: region
status: planned
parent: "[[Japan]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Kanto+region+Japan"
location: [35.6762, 139.6503]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/tokyo-skyline.jpg]]"
banner_position: center
---

# Kanto

## Dlaczego warto

Nizina Wielkiego Tokio; pierwszy region lądowania na [[Japan Spring 2026]].

## Info praktyczne

- **Najlepszy czas:** Koniec marca do połowy kwietnia
- **Jak dojechać:** NRT/HND do Tokio
- **Koszt / bilety:** Suica / Pasmo
- **Godziny:** Zależne od dzielnicy

## Najważniejsze

- Dzielnice [[Tokyo]]
- Jednodniówki w obrębie metra

## Notatki

- Planowany pobyt w Tokio w [[Japan Spring 2026]].

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

- Rodzic: [[Japan]]
- Mapa: [Kanto region Japan](https://www.google.com/maps/search/?api=1&query=Kanto+region+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
