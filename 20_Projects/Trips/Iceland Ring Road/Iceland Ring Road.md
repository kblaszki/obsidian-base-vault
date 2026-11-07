---
type: trip
status: planned
area: "[[Travel]]"
countries: Iceland
start_date:
end_date:
created_date: 2026-10-31
tags:
  - travel
  - trip
---

# Iceland Ring Road

## Cel

Przejechać skondensowaną, południową próbkę Ring Road: baza w Reykjaviku, Golden Circle i atrakcje South Coast, z Blue Lagoon jako elastycznym dodatkiem. Daty jeszcze nieustalone — pliki dni to tymczasowe szkice (`Day 01`–`Day 07`), dopóki nie zarezerwujemy terminów podróży.

## Przegląd itinerarium

- Dzień 01: Przylot KEF → Reykjavik
- Dzień 02: Reykjavik (miasto)
- Dzień 03: pętla Golden Circle
- Dni 04–05: South Coast (wodospady, czarny piasek, widoki lodowca)
- Dzień 06: Bufor / Blue Lagoon
- Dzień 07: Wylot z KEF
- Pełny obwód Ring Road jest poza zakresem tego pierwszego wyjazdu na Islandię

## Logistyka

- **Loty / transport:** Daleki przylot do KEF; zalecany wynajem 4x4 lub kompaktowego SUV ze względu na wiatr i żwirowe pobocza. Bez dat zimowych, dopóki nie będziemy pewni jazdy po lodzie.
- **Noclegi (cele):** Hotel w centrum Reykjaviku (2 noce) → pensjonat Selfoss lub Hella (1 noc) → hotel w rejonie Vík (2 noce) → ostatnia noc w Reykjaviku lub Keflaviku
- **Dokumenty:** Paszport; ubezpieczenie wynajmu z uwzględnieniem żwiru/burz piaskowych; mapy offline

## Zadania przygotowawcze

Tylko na wysokim poziomie — szczegóły w notatkach `prep/`.

- [ ] Wybrać sezon podróży (preferowane późna wiosna lub wczesna jesień)
- [ ] Porównać koszty kampera vs przeskoków hotelowych
- [ ] Przeczytać wskazówki o wietrze i burzach piaskowych na South Coast
- [ ] Zdecydować: Blue Lagoon vs Sky Lagoon

- [ ] Otwórz [[Packing — Iceland Ring Road]]
- [ ] Otwórz [[Bookings and admin — Iceland Ring Road]]

## Miejsca do odwiedzenia

- [[Reykjavik]]
- [[Golden Circle]]
- [[South Coast]]
- [[Blue Lagoon]]

## Budżet

- Około €2000–2600 na tydzień bez lotów; głównie napędzane wynajmem auta i noclegami. Koszty jedzenia spadają dzięki śniadaniom z marketu.

## Notatki o dniach

Tymczasowe pliki dni używają `day_number` zamiast kalendarzowego `date`, dopóki wyjazd nie dostanie terminów.

```dataview
TABLE WITHOUT ID file.link AS Notatka, date AS Data, day_number AS Dzień
FROM "20_Projects/Trips"
WHERE type = "trip-day" AND trip = this.file.link
SORT date ASC, day_number ASC
```

## Dni

```dataview
TABLE WITHOUT ID file.link AS Notatka, date AS Data, day_number AS Dzień
FROM "20_Projects/Trips"
WHERE type = "trip-day" AND trip = this.file.link
SORT date ASC, day_number ASC
```

## Wskazówki

```dataview
TABLE WITHOUT ID file.link AS Wskazówka, topic AS Temat, status AS Status
FROM "20_Projects/Trips"
WHERE type = "trip-tip" AND trip = this.file.link
SORT topic ASC, file.name ASC
```

## Przygotowanie

```dataview
TABLE WITHOUT ID file.link AS Notatka, prep_kind AS Rodzaj, status AS Status
FROM "20_Projects/Trips"
WHERE type = "trip-prep" AND trip = this.file.link
SORT prep_kind ASC, file.name ASC
```

## Powiązane

- [[Travel]]
- [[Dashboard_Travel]]
