---
type: place
place_type: city
status: planned
parent: "[[Kanto]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Tokyo+Japan"
location: [35.6762, 139.6503]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/tokyo-skyline.jpg]]"
banner_position: center
---

# Tokyo

## Dlaczego warto

Gęste dzielnice i parki z kwitnieniem; pierwsza baza na [[Japan Spring 2026]].

## Info praktyczne

- **Najlepszy czas:** Koniec marca do połowy kwietnia — kwitnienie
- **Jak dojechać:** NRT/HND + kolej do Shinjuku
- **Koszt / bilety:** Suica do lokalnego transportu
- **Godziny:** Zależne od dzielnicy

## Najważniejsze

- Wieczory w Shinjuku
- Meiji Shrine / Harajuku
- Poranek w Asakusa

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

- Rodzic: [[Kanto]]
- Mapa: [Tokyo Japan](https://www.google.com/maps/search/?api=1&query=Tokyo+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
