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

## Outcome

Catch late cherry blossom season across Tokyo and Kyoto, visit at least three classic temples or shrines, and keep one buffer afternoon for weather.

## Itinerary overview

- Days 1–4: Tokyo (Shinjuku base)
- Day 5: morning shinkansen to Kyoto
- Days 5–8: Kyoto temples + [[Fushimi Inari]] + [[Nara]] day trip
- Day 9: return via Kansai airport mindset (Osaka transit)

## Logistics

- **Flights / transport:** WAW → NRT (outbound); return KIX → WAW. Suica + shinkansen Tokyo→Kyoto. IC card for local transit.
- **Lodging:** Hotel Gracery Shinjuku (4 nights) → Hotel Vista Premio Kyoto (4 nights)
- **Documents:** Passport; eSIM (Airalo Japan); offline Google Maps areas saved

## Prep tasks

High-level only — details live in `prep/` notes.

- [ ] Book Tokyo and Kyoto hotels 📅 2025-11-15
- [ ] Reserve shinkansen seats Tokyo→Kyoto
- [ ] Buy teamLab / museum slots only if energy remains
- [ ] Shortlist vegetarian-friendly Kyoto dinners near hotel

- [ ] Open [[Packing — Japan Spring 2026]]
- [ ] Open [[Bookings and admin — Japan Spring 2026]]

## Places to visit

- [[Tokyo]]
- [[Kyoto]]
- [[Fushimi Inari]]
- [[Nara]]
- [[Osaka]]

## Budget

- Target ¥280,000–320,000 excluding international flights. Lodging and shinkansen dominate; food can stay moderate with convenience-store breakfasts.

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
