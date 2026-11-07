---
type: place
place_type: attraction
status: visited
parent: "[[Florence]]"
visited_date: 2024-09-13
rating: 5
map_url: "https://www.google.com/maps/search/?api=1&query=Uffizi+Gallery+Florence"
location: [43.7678, 11.2553]
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
banner: "[[./assets/uffizi.jpg]]"
banner_position: center
---

# Uffizi

## Dlaczego warto

Kluczowa kolekcja malarstwa; poranne sloty mniej męczą.

## Info praktyczne

- **Najlepszy czas:** Slot otwarcia
- **Jak dojechać:** Spacer z hoteli w centrum historycznym
- **Koszt / bilety:** Timed entry obowiązkowy w szczycie sezonu
- **Godziny:** Historycznie zamknięte w poniedziałki — weryfikuj

## Najważniejsze

- Rytm korytarzy, jeśli idziesz równo
- Sale Botticellego

## Notatki

- Poranna wizyta z timed entry 2024-09-13 na [[Rome and Florence 2024]].

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

- Rodzic: [[Florence]]
- Mapa: [Uffizi Gallery Florence](https://www.google.com/maps/search/?api=1&query=Uffizi+Gallery+Florence)
- [[Travel]]
- [[Dashboard_Travel]]
