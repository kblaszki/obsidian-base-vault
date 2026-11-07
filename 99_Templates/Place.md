---
type: place
place_type: "{{VALUE:country,region,city,attraction|name:place_type|label:Rodzaj miejsca}}"
status: "{{VALUE:wishlist,planned,visited|name:status|label:Status}}"
parent: "{{FILE:40_Resources/Places|link|label:Miejsce nadrzędne|optional}}"
visited_date: "{{VDATE:visited_date,YYYY-MM-DD|label:Data wizyty|optional}}"
rating:
map_url: "{{VALUE:map_url|label:URL Google Maps|optional}}"
location:
source_url: "{{VALUE:source_url|label:URL źródła|optional}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - place
  - "{{VALUE:topic|label:Tag tematu bez #|optional}}"
banner:
banner_position: center
---

# <% tp.file.title %>

## Dlaczego warto

{{VALUE:why_visit|label:Dlaczego warto?|type:multiline}}

## Informacje praktyczne

- **Najlepszy czas:**
- **Jak dojechać:**
- **Koszt / bilety:**
- **Godziny:**

## Atrakcje

- <% tp.file.cursor(1) %>

## Dziennik wizyt

-

## Miejsca podrzędne

```dataview
TABLE WITHOUT ID file.link AS Miejsce, place_type AS Rodzaj, status AS Status
FROM "40_Resources/Places"
WHERE parent = this.file.link
SORT place_type ASC, file.name ASC
```

## Wyjazdy

```dataview
LIST
FROM "20_Projects/Trips"
WHERE type = "trip" AND contains(file.outlinks, this.file.link)
SORT start_date DESC
```

## Powiązane

- Rodzic: {{FILE:40_Resources/Places|link|label:Miejsce nadrzędne|optional}}
- Mapa: {{VALUE:map_url|label:URL Google Maps|optional}}
- [[Travel]]
- [[Dashboard_Travel]]
