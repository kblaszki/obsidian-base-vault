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
icon: ✈️
---

# Lisbon and Porto 2025

## Outcome

Combine Lisbon's hills and Belém with a Porto base for Ribeira, port lodges, and a Douro evening.

## Itinerary overview

- Days 1–4: Lisbon (Baixa / Chiado)
- Day 5: Alfa Pendular to Porto
- Days 5–8: Porto + Gaia riverside
- Slow mornings; prioritize walking over too many paid attractions

## Logistics

- **Flights / transport:** WAW → LIS; return OPO → WAW. Metro + tram in Lisbon; Alfa Pendular LIS→POR; Porto metro to airport.
- **Lodging:** Independente Hostel & Suites rooftop room, Lisbon (4 nights) → Pestana Vintage Porto (3 nights)
- **Documents:** EU ID; CP train tickets in app

## Prep tasks

High-level only — details live in `prep/` notes.

- [x] Book Alfa Pendular seats
- [x] Reserve Belém pastry stop timing (early)
- [x] Buy Lisboa Card 48h for tram + museums
- [x] Note Gaia lodge tasting hours

- [ ] Open [[Packing — Lisbon and Porto 2025]]
- [ ] Open [[Bookings and admin — Lisbon and Porto 2025]]

## Places to visit

- [[Lisbon]]
- [[Belém Tower]]
- [[Porto]]
- [[Ribeira]]

## Budget

- About €1,400 total. Pestana riverside hotel pushed Porto lodging up; food stayed affordable.

## Days

```dataview
TABLE WITHOUT ID file.link AS Note, date AS Date, day_number AS Day
FROM "20_Projects/Trips"
WHERE type = "trip-day" AND trip = this.file.link
SORT date ASC, day_number ASC
```

## Tips

```dataview
TABLE WITHOUT ID file.link AS Tip, topic AS Topic, status AS Status
FROM "20_Projects/Trips"
WHERE type = "trip-tip" AND trip = this.file.link
SORT topic ASC, file.name ASC
```

## Prep

```dataview
TABLE WITHOUT ID file.link AS Note, prep_kind AS Kind, status AS Status
FROM "20_Projects/Trips"
WHERE type = "trip-prep" AND trip = this.file.link
SORT prep_kind ASC, file.name ASC
```

## Related

- [[Travel]]
- [[Dashboard_Travel]]
