---
type: resource
resource_type: "{{VALUE:book,article,video,course|name:resource_type|label:Rodzaj zasobu}}"
status: "{{VALUE:to-read,reading,processed|name:status|label:Status}}"
author: "{{VALUE:author|label:Autor lub twórca}}"
source_url: "{{VALUE:source_url|label:URL źródła lub ISBN|optional}}"
tags:
  - resource
  - "{{VALUE:topic|label:Tag tematu bez #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
finished_date:
rating:
---

# <% tp.file.title %>

## Podsumowanie

{{VALUE:summary|label:Dlaczego to zapisujesz?|type:multiline}}

## Kluczowe idee

- <% tp.file.cursor(1) %>

## Fragmenty

> 

## Moja interpretacja


## Działania

- [ ] 

## Powiązania

- Obszar: {{FILE:30_Areas|link|label:Powiązany obszar|optional}}
- Projekt: {{FILE:20_Projects|link|label:Powiązany projekt|optional}}
