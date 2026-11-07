---
type: place
place_type: city
status: wishlist
parent: "[[Capital Region]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Reykjavik+Iceland"
location: [64.1466, -21.9426]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/reykjavik.jpg]]"
banner_position: center
---

# Reykjavik

## Dlaczego warto

Zwarta stolica do sprawdzenia sprzętu i odpoczynku przed jazdą South Coast na [[Iceland Ring Road]].

## Info praktyczne

- **Najlepszy czas:** Późna wiosna do wczesnej jesieni — łatwiejsza jazda
- **Jak dojechać:** KEF + Flybus lub wynajem auta
- **Koszt / bilety:** Jedzenie w mieście drogie; śniadania z marketu pomagają
- **Godziny:** Ekstremalna sezonowość dnia

## Najważniejsze

- Port i Harpa
- Sklepy ze sprzętem na Laugavegur
- Łatwe pierwsze/ostatnie noce

## Notatki

- Baza z listy życzeń na [[Iceland Ring Road]] (daty TBD).

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

- Rodzic: [[Capital Region]]
- Mapa: [Reykjavik Iceland](https://www.google.com/maps/search/?api=1&query=Reykjavik+Iceland)
- [[Travel]]
- [[Dashboard_Travel]]
