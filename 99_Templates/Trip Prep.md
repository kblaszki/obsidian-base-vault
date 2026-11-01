---
type: trip-prep
trip: "{{FILE:20_Projects/Trips|link|label:Trip}}"
prep_kind: "{{VALUE:packing,bookings,documents,health,other|name:prep_kind|label:Prep kind}}"
status: "{{VALUE:todo,in-progress,done|name:status|label:Status}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - prep
icon: ☑️
---

# <% tp.file.title %>

{{VALUE:summary|label:What this prep note covers|type:multiline}}

## Checklist

- [ ] {{VALUE:first_item|label:First checklist item}}

## Details

-

## Deadlines

-

## Related

- {{FILE:20_Projects/Trips|link|label:Trip}}
- [[Dashboard_Travel]]
