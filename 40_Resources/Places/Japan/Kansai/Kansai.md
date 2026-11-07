---
type: place
place_type: region
status: planned
parent: "[[Japan]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Kansai+Japan"
location: [34.6937, 135.5023]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/kyoto-temple.jpg]]"
banner_position: center
---

# Kansai

## Dlaczego warto

Korytarz Kioto, Nara i Osaka — świątynie i logistyka wylotu.

## Info praktyczne

- **Najlepszy czas:** Początek do połowy kwietnia
- **Jak dojechać:** Shinkansen z Tokio; Haruka do KIX
- **Koszt / bilety:** Lokalne busy i spacery pokrywają większość atrakcji
- **Godziny:** Świątynie często zamykane późnym popołudniem

## Najważniejsze

- Świątynie [[Kyoto]]
- Jednodniówka [[Nara]]
- Tranzyt [[Osaka]] do KIX

## Notatki

- Planowane dni Kansai w [[Japan Spring 2026]].

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

- Rodzic: [[Japan]]
- Mapa: [Kansai Japan](https://www.google.com/maps/search/?api=1&query=Kansai+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
