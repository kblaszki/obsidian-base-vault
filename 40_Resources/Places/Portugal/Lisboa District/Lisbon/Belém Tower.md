---
type: place
place_type: attraction
status: visited
parent: "[[Lisbon]]"
visited_date: 2025-05-12
rating: 4
map_url: "https://www.google.com/maps/search/?api=1&query=Bel%C3%A9m+Tower+Lisbon"
location: [38.6916, -9.216]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/lisbon-belem.jpg]]"
banner_position: center
---

# Belém Tower

## Dlaczego warto

Ikoniczny zabytek nad Tagiem; łączy się z Pastéis de Belém i Jerónimos.

## Info praktyczne

- **Najlepszy czas:** Wczesny poranek
- **Jak dojechać:** Tramwaj 15 lub pociąg do Belém
- **Koszt / bilety:** Kolejka na wejście na wieżę osobno od zdjęć z zewnątrz
- **Godziny:** W dzień; sprawdź zamknięcia w poniedziałki

## Najważniejsze

- Wiatr i widoki nad rzeką
- Połącz ze strategią kolejki po ciastka

## Notatki

- Wizyta z zewnątrz i okolica 2025-05-12 na [[Lisbon and Porto 2025]].

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

- Rodzic: [[Lisbon]]
- Mapa: [Belém Tower Lisbon](https://www.google.com/maps/search/?api=1&query=Bel%C3%A9m+Tower+Lisbon)
- [[Travel]]
- [[Dashboard_Travel]]
