---
type: place
place_type: region
status: wishlist
parent: "[[Iceland]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Reykjavik+Capital+Region+Iceland"
location: [64.1466, -21.9426]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/reykjavik.jpg]]"
banner_position: center
---

# Capital Region

## Dlaczego warto

Logistyka Reykjaviku i lotniska na starty i końce ring-road.

## Info praktyczne

- **Najlepszy czas:** Późna wiosna do wczesnej jesieni
- **Jak dojechać:** KEF + Flybus lub wynajem auta
- **Koszt / bilety:** Jedzenie w mieście jest drogie
- **Godziny:** Ekstremalna sezonowość dnia

## Najważniejsze

- [[Reykjavik]]

## Notatki

- Baza z listy życzeń na [[Iceland Ring Road]].

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
- Mapa: [Reykjavik Capital Region Iceland](https://www.google.com/maps/search/?api=1&query=Reykjavik+Capital+Region+Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
