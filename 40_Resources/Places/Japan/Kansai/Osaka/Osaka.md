---
type: place
place_type: city
status: planned
parent: "[[Kansai]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Osaka+Castle+Japan"
location: [34.6873, 135.5262]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/osaka-castle.jpg]]"
banner_position: center
---

# Osaka

## Dlaczego warto

Węzeł przesiadkowy w stronę KIX w ostatnim dniu [[Japan Spring 2026]].

## Info praktyczne

- **Najlepszy czas:** Przelotowo lub postój na jedzenie
- **Jak dojechać:** Kolej z Kioto; Haruka do KIX
- **Koszt / bilety:** Karty IC działają
- **Godziny:** Pociągi lotniskowe częste

## Najważniejsze

- Logistyka transferu na lotnisko
- Opcjonalny postój na jedzenie, jeśli plan pozwala

## Notatki

- Planowany tranzyt wylotowy 2026-04-18 w [[Japan Spring 2026]].

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
- Mapa: [Osaka Castle Japan](https://www.google.com/maps/search/?api=1&query=Osaka+Castle+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
