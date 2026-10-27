---
type: place
place_type: "{{VALUE:country,city,attraction|name:place_type|label:Place type}}"
status: "{{VALUE:wishlist,planned,visited|name:status|label:Status}}"
country: "{{VALUE:country|label:Country}}"
city: "{{VALUE:city|label:City|optional}}"
visited_date: "{{VDATE:visited_date,YYYY-MM-DD|label:Visited date|optional}}"
rating:
map_url: "{{VALUE:map_url|label:Map URL|optional}}"
source_url: "{{VALUE:source_url|label:Source URL|optional}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - place
  - "{{VALUE:topic|label:Topic tag without #|optional}}"
icon: 📍
---

# <% tp.file.title %>

## Why visit

{{VALUE:why_visit|label:Why visit?|type:multiline}}

## Practical info

- **Best time:** 
- **How to get there:** 
- **Cost / tickets:** 
- **Hours:** 

## Highlights

- <% tp.file.cursor(1) %>

## Visit log

- 

## Trips

```dataview
LIST
FROM "20_Projects/Trips"
WHERE type = "trip" AND contains(file.outlinks, this.file.link)
SORT start_date DESC
```

## Related

- Country: [[{{VALUE:country}}]]
- [[Travel]]
- [[Dashboard_Travel]]
