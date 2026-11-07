---
type: place
place_type: region
status: planned
parent: "[[Iceland]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Gullfoss+Golden+Circle+Iceland"
location: [64.3271, -20.1211]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/gullfoss.jpg]]"
banner_position: center
---

# Golden Circle

## Dlaczego warto

Najwydajniejsza pętla dnia z Reykjaviku: dolina ryftowa, gejzery i wodospad.

## Info praktyczne

- **Najlepszy czas:** Start wcześnie, by wyprzedzić busy
- **Jak dojechać:** Dzienna pętla wynajętym autem
- **Koszt / bilety:** Punkty widokowe głównie darmowe; parkingi różnie
- **Godziny:** Zależne od światła dziennego

## Najważniejsze

- Þingvellir
- Okolica Geysir
- Gullfoss

## Notatki

- Szkic dnia 03 na [[Iceland Ring Road]].

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
- [[Reykjavik]]
- Mapa: [Gullfoss Golden Circle Iceland](https://www.google.com/maps/search/?api=1&query=Gullfoss+Golden+Circle+Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
