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

## Outcome

Base in Edinburgh for two nights, then drive the Highlands with Skye as the scenic peak and Glencoe as the dramatic return.

## Itinerary overview

- Days 1–2: Edinburgh
- Days 3–5: Isle of Skye (Portree area)
- Days 6–7: Glencoe / Fort William corridor
- Day 8: return to EDI and fly out
- Rental car from Edinburgh day 3

## Logistics

- **Flights / transport:** WAW → EDI. Enterprise car hire (manual) for Highlands loop. Single-track practice needed for Skye.
- **Lodging:** Motel One Edinburgh Royal (2 nights) → Cuillin Hills Hotel, Portree (3 nights) → Kingshouse Hotel, Glencoe (2 nights)
- **Documents:** Passport; UK ETA; International Driving Permit photocopies

## Prep tasks

High-level only — details live in `prep/` notes.

- [x] Book car with full insurance
- [x] Reserve Skye and Glencoe hotels (August fills early)
- [x] Download offline OS maps
- [x] Pack waterproof layers regardless of forecast

- [ ] Open [[Packing — Scottish Highlands 2025]]
- [ ] Open [[Bookings and admin — Scottish Highlands 2025]]

## Places to visit

- [[Edinburgh]]
- [[Isle of Skye]]
- [[Glencoe]]

## Budget

- ~£1,900 including car hire and Highland hotels. Weather forced two café days but scenery still delivered.

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
