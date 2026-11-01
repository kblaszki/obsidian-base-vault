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
icon: ✈️
---

# Rome and Florence 2024

## Outcome

See major Rome landmarks with timed tickets, then switch to Florence for Renaissance museums and evening walks along the Arno.

## Itinerary overview

- Days 1–4: Rome base near Termini
- Day 5: morning Frecciarossa to Florence
- Days 5–8: Florence + optional day trip mindset (stayed in city)
- Focus: Colosseum, Pantheon, Uffizi, Duomo exterior and Oltrarno

## Logistics

- **Flights / transport:** WAW → FCO (Ryanair); return FLR → WAW. Roma Pass day tickets + Trenitalia Freccia.
- **Lodging:** Hotel Artemide, Via Nazionale, Rome (3 nights) → Hotel Davanzati, Via Porta Rossa, Florence (4 nights)
- **Documents:** EU ID; museum reservations printed offline

## Prep tasks

High-level only — details live in `prep/` notes.

- [x] Book Colosseum + Forum timed entry
- [x] Reserve Uffizi morning slot
- [x] Buy Freccia Rome→Florence tickets
- [x] Confirm both hotel cancellations windows

- [ ] Open [[Packing — Rome and Florence 2024]]
- [ ] Open [[Bookings and admin — Rome and Florence 2024]]

## Places to visit

- [[Rome]]
- [[Colosseum]]
- [[Pantheon]]
- [[Florence]]
- [[Uffizi]]

## Budget

- Total ~€1,650 for two soft days of museums + mid-range meals. Lodging was the largest line item.

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
