---
type: trip-tip
trip: "{{FILE:20_Projects/Trips|link|label:Trip}}"
topic: "{{VALUE:transit,driving,money,connectivity,safety,culture,other|name:topic|label:Topic}}"
status: "{{VALUE:draft,ready|name:status|label:Status}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - tip
icon: 💡
---

# <% tp.file.title %>

{{VALUE:summary|label:One-paragraph summary|type:multiline}}

## Key points

- {{VALUE:first_point|label:First key point}}

## Details

-

## Sources

-

## Related

- {{FILE:20_Projects/Trips|link|label:Trip}}
- [[Dashboard_Travel]]
