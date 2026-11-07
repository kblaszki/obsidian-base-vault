---
type: trip
status: completed
area: "[[Travel]]"
countries: United Kingdom
start_date: 2025-08-02
end_date: 2025-08-09
created_date: 2025-04-20
tags:
  - travel
  - trip
---

# Scottish Highlands 2025

## Cel

Dwie noce bazy w Edynburgu, potem jazda przez Highlands ze Skye jako scenicznym szczytem i Glencoe jako dramatycznym powrotem.

## Przegląd itinerarium

- Dni 1–2: Edynburg
- Dni 3–5: Isle of Skye (rejon Portree)
- Dni 6–7: korytarz Glencoe / Fort William
- Dzień 8: powrót do EDI i wylot
- Wynajem auta z Edynburga od dnia 3

## Logistyka

- **Loty / transport:** WAW → EDI. Wynajem Enterprise (manual) na pętlę Highlands. Potrzebna praktyka single-track na Skye.
- **Noclegi:** Motel One Edinburgh Royal (2 noce) → Cuillin Hills Hotel, Portree (3 noce) → Kingshouse Hotel, Glencoe (2 noce)
- **Dokumenty:** Paszport; UK ETA; kopie International Driving Permit

## Zadania przygotowawcze

Tylko na wysokim poziomie — szczegóły w notatkach `prep/`.

- [x] Zarezerwować auto z pełnym ubezpieczeniem
- [x] Zarezerwować hotele na Skye i w Glencoe (sierpień zapełnia się wcześnie)
- [x] Pobrać mapy OS offline
- [x] Spakować warstwy wodoodporne niezależnie od prognozy

- [ ] Otwórz [[Packing — Scottish Highlands 2025]]
- [ ] Otwórz [[Bookings and admin — Scottish Highlands 2025]]

## Miejsca do odwiedzenia

- [[Edinburgh]]
- [[Isle of Skye]]
- [[Glencoe]]

## Budżet

- ~£1900 z wynajmem auta i hotelami w Highlands. Pogoda wymusiła dwa dni kawiarniane, ale krajobrazy i tak dostarczyły wrażeń.

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
