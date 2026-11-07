---
type: trip
status: completed
area: "[[Travel]]"
countries: Portugal
start_date: 2025-05-10
end_date: 2025-05-17
created_date: 2025-02-10
tags:
  - travel
  - trip
---

# Lisbon and Porto 2025

## Cel

Połączyć wzgórza Lizbony i Belém z bazą w Porto na Ribeirę, lodge’e porto i wieczór nad Douro.

## Przegląd itinerarium

- Dni 1–4: Lizbona (Baixa / Chiado)
- Dzień 5: Alfa Pendular do Porto
- Dni 5–8: Porto + nabrzeże Gaia
- Spokojne poranki; priorytet spacerów zamiast zbyt wielu płatnych atrakcji

## Logistyka

- **Loty / transport:** WAW → LIS; powrót OPO → WAW. Metro + tramwaj w Lizbonie; Alfa Pendular LIS→POR; metro w Porto na lotnisko.
- **Noclegi:** Independente Hostel & Suites (pokój z tarasem), Lizbona (4 noce) → Pestana Vintage Porto (3 noce)
- **Dokumenty:** Dowód UE; bilety CP w aplikacji

## Zadania przygotowawcze

Tylko na wysokim poziomie — szczegóły w notatkach `prep/`.

- [x] Zarezerwować miejsca w Alfa Pendular
- [x] Zaplanować wczesny przystanek na pastéis w Belém
- [x] Kupić Lisboa Card 48h na tramwaj + muzea
- [x] Zanotować godziny degustacji w lodge’ach w Gaia

- [ ] Otwórz [[Packing — Lisbon and Porto 2025]]
- [ ] Otwórz [[Bookings and admin — Lisbon and Porto 2025]]

## Miejsca do odwiedzenia

- [[Lisbon]]
- [[Belém Tower]]
- [[Porto]]
- [[Ribeira]]

## Budżet

- Około €1400 łącznie. Hotel Pestana nad rzeką podbił koszty noclegu w Porto; jedzenie pozostało przystępne.

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
