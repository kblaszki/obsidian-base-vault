---
type: place
place_type: country
status: visited
parent:
visited_date: 2025-05-17
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Portugal"
location: [38.7223, -9.1393]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/lisbon-view.jpg]]"
banner_position: center
---

# Portugal

## Dlaczego warto

Miasta atlantyckie ze wzgórzami, miradouro i wieczorami nad rzeką.

## Info praktyczne

- **Najlepszy czas:** Maj–czerwiec lub wrzesień
- **Jak dojechać:** Huby LIS / OPO
- **Koszt / bilety:** Lisboa Card przydatna w dni tramwajowe
- **Godziny:** Restauracje późno; atrakcje w dzień

## Najważniejsze

- Wzgórza Lizbony
- Nabrzeże Porto

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

- Mapa: [Portugal](https://www.google.com/maps/search/?api=1&query=Portugal)
- [[Travel]]
- [[Dashboard_Travel]]
