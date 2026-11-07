---
type: place
place_type: country
status: planned
parent:
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Japan"
location: [35.6762, 139.6503]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/tokyo-skyline.jpg]]"
banner_position: center
---

# Japan

## Dlaczego warto

Państwo wyspiarskie z gęstymi miastami, obwodami świątyń i wiosennym kwitnieniem.

## Info praktyczne

- **Najlepszy czas:** Koniec marca do połowy kwietnia — kwitnienie
- **Jak dojechać:** NRT/HND lub KIX
- **Koszt / bilety:** Rail Pass albo IC + bilety shinkansen
- **Godziny:** Świątynie często zamykane późnym popołudniem

## Najważniejsze

- Baza w Tokio
- Dni świątyń w Kansai
- Etykieta jedzenia i transportu

## Notatki

- Planowany kwiecień 2026 przez [[Japan Spring 2026]].

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

- Mapa: [Japan](https://www.google.com/maps/search/?api=1&query=Japan)
- [[Travel]]
- [[Dashboard_Travel]]
