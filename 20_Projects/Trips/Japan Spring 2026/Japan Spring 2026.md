---
type: trip
status: planned
area: "[[Travel]]"
countries: Japan
start_date: 2026-04-10
end_date: 2026-04-18
created_date: 2026-10-27
tags:
  - travel
  - trip
---

# Japan Spring 2026

## Cel

Złapać późny sezon kwitnienia wiśni w Tokio i Kioto, zobaczyć co najmniej trzy klasyczne świątynie lub sanktuaria i zostawić jedno popołudnie buforowe na pogodę.

## Przegląd itinerarium

- Dni 1–4: Tokio (baza w Shinjuku)
- Dzień 5: rano shinkansen do Kioto
- Dni 5–8: świątynie w Kioto + [[Fushimi Inari]] + jednodniowa wycieczka do [[Nara]]
- Dzień 9: powrót w trybie lotniska Kansai (przejazd przez Osakę)

## Logistyka

- **Loty / transport:** WAW → NRT (wylot); powrót KIX → WAW. Suica + shinkansen Tokio→Kioto. Karta IC do lokalnego transportu.
- **Noclegi:** Hotel Gracery Shinjuku (4 noce) → Hotel Vista Premio Kyoto (4 noce)
- **Dokumenty:** Paszport; eSIM (Airalo Japan); zapisane offline obszary Google Maps

## Zadania przygotowawcze

Tylko na wysokim poziomie — szczegóły w notatkach `prep/`.

- [ ] Zarezerwować hotele w Tokio i Kioto 📅 2025-11-15
- [ ] Zarezerwować miejsca w shinkansenie Tokio→Kioto
- [ ] Kupić bilety teamLab / muzea tylko jeśli zostanie energia
- [ ] Wstępnie wybrać wegetariańskie kolacje w Kioto blisko hotelu

- [ ] Otwórz [[Packing — Japan Spring 2026]]
- [ ] Otwórz [[Bookings and admin — Japan Spring 2026]]

## Miejsca do odwiedzenia

- [[Tokyo]]
- [[Kyoto]]
- [[Fushimi Inari]]
- [[Nara]]
- [[Osaka]]

## Budżet

- Cel: ¥280 000–320 000 bez lotów międzynarodowych. Dominują noclegi i shinkansen; jedzenie można utrzymać umiarkowanie dzięki śniadaniom z convenience store.

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
