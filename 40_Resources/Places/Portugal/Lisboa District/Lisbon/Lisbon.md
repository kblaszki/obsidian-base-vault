---
type: place
place_type: city
status: visited
parent: "[[Lisboa District]]"
visited_date: 2025-05-13
rating: 4
map_url: "https://www.google.com/maps/search/?api=1&query=Lisbon+Portugal"
location: [38.7223, -9.1393]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/lisbon-view.jpg]]"
banner_position: center
---

# Lisbon

## Dlaczego warto

Wzgórza, miradouro i jednodniówki do Belém; energiczna baza na [[Lisbon and Porto 2025]].

## Info praktyczne

- **Najlepszy czas:** Maj–czerwiec lub wrzesień
- **Jak dojechać:** Metro z LIS do Baixa-Chiado
- **Koszt / bilety:** Lisboa Card przydatna w dni tramwajowe
- **Godziny:** Restauracje późno; atrakcje standardowo w dzień

## Najważniejsze

- Uliczki Alfamy
- Strategia tramwaju 28 (więcej spaceru niż jazdy)
- Poranna kawa w LX Factory

## Notatki

- Odwiedzono 2025-05-10 do 2025-05-14 na [[Lisbon and Porto 2025]].

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

- Rodzic: [[Lisboa District]]
- [[Belém Tower]]
- Mapa: [Lisbon Portugal](https://www.google.com/maps/search/?api=1&query=Lisbon+Portugal)
- [[Travel]]
- [[Dashboard_Travel]]
