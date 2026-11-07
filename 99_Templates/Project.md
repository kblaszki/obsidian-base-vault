---
type: project
status: "{{VALUE:planned,active,on-hold|name:status|label:Status}}"
area: "{{FILE:30_Areas|link|label:Obszar}}"
tags:
  - project
  - "{{VALUE:topic|label:Tag tematu bez #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
review_date: <% moment().add(7, "days").format("YYYY-MM-DD") %>
target_date: "{{VDATE:target_date,YYYY-MM-DD|label:Termin docelowy|optional}}"
---

# <% tp.file.title %>

## Cel

{{VALUE:outcome|label:Jak wygląda „zrobione”?|type:multiline}}

## Dlaczego


## Następne działania

- [ ] {{VALUE:next_action|label:Pierwsze następne działanie}} {{VDATE:target_date,[📅 ]YYYY-MM-DD|optional}}

## Kamienie milowe

- [ ] 

## Notatki


## Zasoby

- 

## Przegląd

- **Ostatni przegląd:** <% tp.date.now("YYYY-MM-DD") %>
- **Następny przegląd:** <% moment().add(7, "days").format("YYYY-MM-DD") %>

## Powiązane

- [[Dashboard_Projects]]
