---
type: trip-day
trip: "{{FILE:20_Projects/Trips|link|label:Trip}}"
date: "{{VDATE:date,YYYY-MM-DD|label:Day}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - trip-day
banner:
banner_position: center
---

# <% tp.file.title %>

{{VALUE:summary|label:Short day summary|type:multiline}}


## Day timeline

- {{VALUE:first_time|label:First timeline time|default:09:00}} — {{VALUE:first_timeline|label:First timeline item}}

## Logistics

-

## Places

- [[]] — *(quick stop / 1–2h / half day)*

## Food

- **Breakfast:**
- **Lunch:**
- **Dinner:**
- **Groceries / snacks:**

### Costs

| Item | Amount | Notes |
|------|--------|-------|
|      |        |       |

## Pack today

- **Documents:**
- **Clothes:**
- **Cash / cards:**
- **Gear:**

## Notes

{{VALUE:day_notes|label:Extra notes|type:multiline|optional}}

## Related

- {{FILE:20_Projects/Trips|link|label:Trip}}
- [[Dashboard_Travel]]
