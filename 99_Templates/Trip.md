---
type: trip
status: "{{VALUE:planned,active,completed,cancelled|name:status|label:Status}}"
area: "{{FILE:30_Areas|link|label:Area}}"
countries: "{{VALUE:countries|label:Countries (comma-separated)}}"
start_date: "{{VDATE:start_date,YYYY-MM-DD|label:Start date}}"
end_date: "{{VDATE:end_date,YYYY-MM-DD|label:End date|optional}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - trip
icon: ✈️
---

# <% tp.file.title %>

## Outcome

{{VALUE:outcome|label:What should this trip achieve?|type:multiline}}

## Itinerary overview

-

## Logistics

- **Flights / transport:**
- **Lodging:**
- **Documents:**

## Prep tasks

High-level only — details live in `prep/` notes.

- [ ] {{VALUE:next_action|label:First prep action}}
- [ ] Create prep notes under `prep/` (packing, bookings)

## Places to visit

-

## Budget

-

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
