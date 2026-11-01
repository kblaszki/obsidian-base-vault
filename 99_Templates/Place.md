---
type: place
place_type: "{{VALUE:country,region,city,attraction|name:place_type|label:Place type}}"
status: "{{VALUE:wishlist,planned,visited|name:status|label:Status}}"
parent: "{{FILE:40_Resources/Places|link|label:Parent place|optional}}"
visited_date: "{{VDATE:visited_date,YYYY-MM-DD|label:Visited date|optional}}"
rating:
map_url: "{{VALUE:map_url|label:Google Maps URL|optional}}"
location:
source_url: "{{VALUE:source_url|label:Source URL|optional}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - place
  - "{{VALUE:topic|label:Topic tag without #|optional}}"
icon: 📍
banner:
banner_position: center
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

## Child places

```dataview
TABLE WITHOUT ID file.link AS Place, place_type AS Kind, status AS Status
FROM "40_Resources/Places"
WHERE parent = this.file.link
SORT place_type ASC, file.name ASC
```

## Trips

```dataview
LIST
FROM "20_Projects/Trips"
WHERE type = "trip" AND contains(file.outlinks, this.file.link)
SORT start_date DESC
```

## Related

- Parent: {{FILE:40_Resources/Places|link|label:Parent place|optional}}
- Map: {{VALUE:map_url|label:Google Maps URL|optional}}
- [[Travel]]
- [[Dashboard_Travel]]
