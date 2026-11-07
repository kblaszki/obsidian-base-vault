---
type: trip
status: completed
area: "[[Travel]]"
countries: Italy
start_date: 2024-09-08
end_date: 2024-09-15
created_date: 2024-07-01
tags:
  - travel
  - trip
---

# Rome and Florence 2024

## Cel

Zobaczyć główne zabytki Rzymu z biletami czasowymi, a potem przenieść się do Florencji na muzea renesansu i wieczorne spacery wzdłuż Arno.

## Przegląd itinerarium

- Dni 1–4: baza w Rzymie w okolicy Termini
- Dzień 5: rano Frecciarossa do Florencji
- Dni 5–8: Florencja + opcjonalny mindset jednodniówki (zostaliśmy w mieście)
- Fokus: Koloseum, Panteon, Uffizi, zewnątrz Duomo i Oltrarno

## Logistyka

- **Loty / transport:** WAW → FCO (Ryanair); powrót FLR → WAW. Dzienny Roma Pass + Trenitalia Freccia.
- **Noclegi:** Hotel Artemide, Via Nazionale, Rzym (3 noce) → Hotel Davanzati, Via Porta Rossa, Florencja (4 noce)
- **Dokumenty:** Dowód UE; rezerwacje muzeów wydrukowane offline

## Zadania przygotowawcze

Tylko na wysokim poziomie — szczegóły w notatkach `prep/`.

- [x] Zarezerwować Koloseum + Forum z wejściem czasowym
- [x] Zarezerwować poranny slot Uffizi
- [x] Kupić bilety Freccia Rzym→Florencja
- [x] Potwierdzić okna anulacji obu hoteli

- [ ] Otwórz [[Packing — Rome and Florence 2024]]
- [ ] Otwórz [[Bookings and admin — Rome and Florence 2024]]

## Miejsca do odwiedzenia

- [[Rome]]
- [[Colosseum]]
- [[Pantheon]]
- [[Florence]]
- [[Uffizi]]

## Budżet

- Łącznie ~€1650 za dwa spokojniejsze dni muzealne + posiłki średniej półki. Noclegi były największą pozycją.

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
