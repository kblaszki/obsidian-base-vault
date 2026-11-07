---
type: trip-tip
trip: "{{FILE:20_Projects/Trips|link|label:Wyjazd}}"
topic: "{{VALUE:transit,driving,money,connectivity,safety,culture,other|name:topic|label:Temat}}"
status: "{{VALUE:draft,ready|name:status|label:Status}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - tip
---

# <% tp.file.title %>

{{VALUE:summary|label:Podsumowanie w jednym akapicie|type:multiline}}

## Kluczowe punkty

- {{VALUE:first_point|label:Pierwszy kluczowy punkt}}

## Szczegóły

-

## Źródła

-

## Powiązane

- {{FILE:20_Projects/Trips|link|label:Wyjazd}}
- [[Dashboard_Travel]]
