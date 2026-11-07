---
type: place
place_type: attraction
status: visited
parent: "[[Scotland]]"
visited_date: 2025-08-08
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Glencoe+Scotland"
location: [56.682, -5.102]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/glencoe.jpg]]"
banner_position: center
---

# Glencoe

## Dlaczego warto

Dramat doliny Highlands i łatwe punkty widokowe przy drodze.

## Info praktyczne

- **Najlepszy czas:** Przejaśnienia między pasmami deszczu
- **Jak dojechać:** Korytarz A82 autem
- **Koszt / bilety:** Opłaty parkingowe przy popularnych lotach
- **Godziny:** Hiking tylko przy świetle dziennym, chyba że jesteś wyposażony

## Najważniejsze

- Punkty widokowe Three Sisters
- Podejścia Buachaille Etive Mòr
- Światło okolicy Kingshouse

## Notatki

- Nocleg i spacery 2025-08-07 do 2025-08-09 na [[Scottish Highlands 2025]].

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

- Rodzic: [[Scotland]]
- Mapa: [Glencoe Scotland](https://www.google.com/maps/search/?api=1&query=Glencoe+Scotland)
- [[Travel]]
- [[Dashboard_Travel]]
