---
type: trip-prep
trip: "{{FILE:20_Projects/Trips|link|label:Wyjazd}}"
prep_kind: "{{VALUE:packing,bookings,documents,health,other|name:prep_kind|label:Rodzaj przygotowania}}"
status: "{{VALUE:todo,in-progress,done|name:status|label:Status}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - prep
---

# <% tp.file.title %>

{{VALUE:summary|label:Czego dotyczy ta notatka przygotowawcza?|type:multiline}}

## Lista

- [ ] {{VALUE:first_item|label:Pierwszy punkt listy}}

## Szczegóły

-

## Terminy

-

## Powiązane

- {{FILE:20_Projects/Trips|link|label:Wyjazd}}
- [[Dashboard_Travel]]
