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

- [ ] {{VALUE:next_action|label:First prep action}}

## Places to visit

- 

## Budget

- 

## Day notes

```dataview
TABLE date AS Day, file.link AS Note
FROM "20_Projects/Trips"
WHERE type = "trip-day" AND trip = this.file.link
SORT date ASC
```

## Related

- [[Travel]]
- [[Dashboard_Travel]]
