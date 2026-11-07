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

## Outcome

Drive a condensed south-focused Ring Road sample: Reykjavik base, Golden Circle, and South Coast highlights, with Blue Lagoon as a flexible add-on. Dates not fixed yet — day files are provisional drafts (`Day 01`–`Day 07`) until travel dates are booked.

## Itinerary overview

- Day 01: Arrive KEF → Reykjavik
- Day 02: Reykjavik city
- Day 03: Golden Circle loop
- Day 04–05: South Coast (waterfalls, black sand, glacier views)
- Day 06: Buffer / Blue Lagoon
- Day 07: Depart KEF
- Full circumference Ring Road is out of scope for this first Iceland trip

## Logistics

- **Flights / transport:** Long-haul into KEF; 4x4 or compact SUV rental recommended for wind and gravel shoulders. No winter dates until confident with ice driving.
- **Lodging (targets):** Downtown Reykjavik hotel (2 nights) → Selfoss or Hella guesthouse (1 night) → Vík area hotel (2 nights) → Reykjavik or Keflavik final night
- **Documents:** Passport; rental insurance with gravel/sandstorm awareness; offline maps

## Prep tasks

High-level only — details live in `prep/` notes.

- [ ] Pick travel season (prefer late spring or early autumn)
- [ ] Compare campervan vs hotel hop costs
- [ ] Read wind and sandstorm guidance for South Coast
- [ ] Decide Blue Lagoon vs Sky Lagoon

- [ ] Open [[Packing — Iceland Ring Road]]
- [ ] Open [[Bookings and admin — Iceland Ring Road]]

## Places to visit

- [[Reykjavik]]
- [[Golden Circle]]
- [[South Coast]]
- [[Blue Lagoon]]

## Budget

- Roughly €2,000–2,600 for one week excluding flights, heavily driven by car hire and lodging. Food costs drop with grocery breakfasts.

## Day notes

Provisional day files use `day_number` instead of calendar `date` until this trip is scheduled.

```dataview
TABLE WITHOUT ID file.link AS Note, date AS Date, day_number AS Day
FROM "20_Projects/Trips"
WHERE type = "trip-day" AND trip = this.file.link
SORT date ASC, day_number ASC
```

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
