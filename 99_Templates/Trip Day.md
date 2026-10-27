---
type: trip-day
trip: "{{FILE:20_Projects/Trips|link|label:Trip}}"
date: "{{VDATE:date,YYYY-MM-DD|label:Day}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - trip-day
icon: 📅
---

# <% tp.file.title %>

## Plan

- [ ] {{VALUE:first_plan|label:First plan item|optional}}

## Log

- <% tp.date.now("HH:mm") %> 

## Places visited

- 

## Food

- 

## Costs

| Item | Amount | Notes |
|------|--------|-------|
|      |        |       |

## Notes

{{VALUE:day_notes|label:Day notes|type:multiline|optional}}

## Related

- {{FILE:20_Projects/Trips|link|label:Trip}}
- [[Dashboard_Travel]]
