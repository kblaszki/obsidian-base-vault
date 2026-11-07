---
type: place
place_type: attraction
status: visited
parent: "[[Porto]]"
visited_date: 2025-05-15
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Ribeira+Porto"
location: [41.1406, -8.6132]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/porto-ribeira.jpg]]"
banner_position: center
---

# Ribeira

## Dlaczego warto

Historyczna dzielnica nadbrzeżna; najlepsza wieczorna atmosfera Porto.

## Info praktyczne

- **Najlepszy czas:** Zmierzch
- **Jak dojechać:** Spacer z São Bento / most Dom Luís
- **Koszt / bilety:** Spacer darmowy; rejsy opcjonalne
- **Godziny:** Zawsze dostępne; restauracje tłocznie po 19:00

## Najważniejsze

- Kolorowe fasady
- Przejście do Gaia na degustacje

## Notatki

- Kilka wieczorów podczas [[Lisbon and Porto 2025]].

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

- Rodzic: [[Porto]]
- Mapa: [Ribeira Porto](https://www.google.com/maps/search/?api=1&query=Ribeira+Porto)
- [[Travel]]
- [[Dashboard_Travel]]
