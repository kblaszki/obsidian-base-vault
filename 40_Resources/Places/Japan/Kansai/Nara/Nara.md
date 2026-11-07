---
type: place
place_type: city
status: planned
parent: "[[Kansai]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Nara+Japan"
location: [34.6851, 135.8048]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/nara-deer.jpg]]"
banner_position: center
---

# Nara

## Dlaczego warto

Łatwa jednodniówka z Kioto do Tōdai-ji i spacerów po parku.

## Info praktyczne

- **Najlepszy czas:** Poranny przyjazd z Kioto
- **Jak dojechać:** JR lub Kintetsu z Kioto
- **Koszt / bilety:** Opłaty świątynne umiarkowane
- **Godziny:** Przyjazne jednodniówce

## Najważniejsze

- Tōdai-ji
- Etykieta parku z jeleniami

## Notatki

- Planowana jednodniówka 2026-04-16 w [[Japan Spring 2026]].

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

- Rodzic: [[Kansai]]
- [[Kyoto]]
- Mapa: [Nara Japan](https://www.google.com/maps/search/?api=1&query=Nara+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
