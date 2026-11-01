---
type: recipe
status: "{{VALUE:wishlist,tried,favorite|name:status|label:Status}}"
cuisine: "{{VALUE:cuisine|label:Cuisine}}"
meal: "{{VALUE:breakfast,lunch,dinner,snack,dessert,drink|name:meal|label:Meal}}"
servings: "{{VALUE:servings|label:Servings}}"
prep_minutes: "{{VALUE:prep_minutes|label:Prep minutes|optional}}"
cook_minutes: "{{VALUE:cook_minutes|label:Cook minutes|optional}}"
source_url: "{{VALUE:source_url|label:Source URL|optional}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
rating:
tags:
  - recipe
  - "{{VALUE:topic|label:Topic tag without #|optional}}"
icon: 🍽️
---

# <% tp.file.title %>

## Summary

{{VALUE:summary|label:Why save this recipe?|type:multiline}}

## Ingredients

- <% tp.file.cursor(1) %>

## Steps

1. 

## Notes

- 

## Related

- Cuisine / place: 
- Trip: 
- [[Travel]]
