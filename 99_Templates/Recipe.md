---
type: recipe
status: "{{VALUE:wishlist,tried,favorite|name:status|label:Status}}"
cuisine: "{{VALUE:cuisine|label:Kuchnia}}"
meal: "{{VALUE:breakfast,lunch,dinner,snack,dessert,drink|name:meal|label:Posiłek}}"
servings: "{{VALUE:servings|label:Porcje}}"
prep_minutes: "{{VALUE:prep_minutes|label:Minuty przygotowania|optional}}"
cook_minutes: "{{VALUE:cook_minutes|label:Minuty gotowania|optional}}"
source_url: "{{VALUE:source_url|label:URL źródła|optional}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
rating:
tags:
  - recipe
  - "{{VALUE:topic|label:Tag tematu bez #|optional}}"
---

# <% tp.file.title %>

## Podsumowanie

{{VALUE:summary|label:Dlaczego zapisujesz ten przepis?|type:multiline}}

## Składniki

- <% tp.file.cursor(1) %>

## Kroki

1.

## Notatki

-

## Powiązane

- Kuchnia / miejsce:
- Wyjazd:
- [[Travel]]
