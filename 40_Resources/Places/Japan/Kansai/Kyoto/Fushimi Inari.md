---
type: place
place_type: attraction
status: wishlist
parent: "[[Kyoto]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Fushimi+Inari+Taisha+Kyoto"
location: [34.9671, 135.7727]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/kyoto-fushimi.jpg]]"
banner_position: center
---

# Fushimi Inari

## Dlaczego warto

Ikoniczne bramy torii nad Kioto; wysoki priorytet na [[Japan Spring 2026]].

## Info praktyczne

- **Najlepszy czas:** Przed 08:00
- **Jak dojechać:** JR Inari Station
- **Koszt / bilety:** Teren świątyni darmowy
- **Godziny:** Otwarte 24h; sklepy różnie

## Najważniejsze

- Dolna ścieżka bram
- Opcjonalny wyższy odcinek

## Notatki

- Planowana wczesna wizyta 2026-04-15 w [[Japan Spring 2026]].

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

- Rodzic: [[Kyoto]]
- Mapa: [Fushimi Inari Taisha Kyoto](https://www.google.com/maps/search/?api=1&query=Fushimi+Inari+Taisha+Kyoto)
- [[Travel]]
- [[Dashboard_Travel]]
