---
type: place
place_type: city
status: planned
parent: "[[Kansai]]"
visited_date:
rating:
map_url: "https://www.google.com/maps/search/?api=1&query=Kyoto+Japan"
location: [35.0116, 135.7681]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/kyoto-temple.jpg]]"
banner_position: center
---

# Kyoto

## Dlaczego warto

Obwody świątyń i spokojniejsze wieczory po Tokio podczas [[Japan Spring 2026]].

## Info praktyczne

- **Najlepszy czas:** Początek do połowy kwietnia
- **Jak dojechać:** Shinkansen z Tokio
- **Koszt / bilety:** Lokalne busy i spacery pokrywają większość atrakcji
- **Godziny:** Świątynie często zamykane późnym popołudniem

## Najważniejsze

- [[Fushimi Inari]]
- Wieczory w Gion
- Arashiyama

## Notatki

- Planowane dni w Kioto w [[Japan Spring 2026]].

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
- [[Fushimi Inari]]
- [[Nara]]
- Mapa: [Kyoto Japan](https://www.google.com/maps/search/?api=1&query=Kyoto+Japan)
- [[Travel]]
- [[Dashboard_Travel]]
