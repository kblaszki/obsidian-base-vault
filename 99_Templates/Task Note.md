---
type: "{{VALUE:task,note|name:type|label:Typ}}"
status: "{{VALUE:inbox,next,waiting,done|name:status|label:Status}}"
project: "{{FILE:20_Projects|link|label:Projekt|optional}}"
due: "{{VDATE:due,YYYY-MM-DD|label:Termin|optional}}"
tags:
  - inbox
  - "{{VALUE:topic|label:Tag tematu bez #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
---

# <% tp.file.title %>

## Kontekst

{{VALUE:context|label:Co wymaga uwagi?|type:multiline}}

## Następne działanie

- [ ] <% tp.file.cursor(1) %> {{VDATE:due,[📅 ]YYYY-MM-DD|optional}}

## Notatki


## Lista przetwarzania

- [ ] Uściślij pożądany rezultat
- [ ] Połącz z projektem lub obszarem
- [ ] Przenieś ze `00_Inbox` lub zarchiwizuj
