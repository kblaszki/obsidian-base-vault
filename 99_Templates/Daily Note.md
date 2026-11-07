---
type: daily
date: <% tp.date.now("YYYY-MM-DD") %>
created_date: <% tp.date.now("YYYY-MM-DDTHH:mm") %>
tags:
  - journal/daily
---

# <% tp.date.now("dddd, D MMMM YYYY") %>

<%*
const noteDate = moment(tp.file.title, "YYYY-MM-DD");
const previous = noteDate.clone().subtract(1, "day").format("YYYY-MM-DD");
const next = noteDate.clone().add(1, "day").format("YYYY-MM-DD");
tR += `[[${previous}|← Poprzedni]] · [[${next}|Następny →]]`;
%>

## Fokus

- [ ] <% tp.file.cursor(1) %>

## Zadania

- [ ]

## Dziennik

- <% tp.date.now("HH:mm") %>

## Notatki


## Przegląd dnia

- **Sukces:**
- **Czego się nauczyłem/am:**
- **Do przeniesienia:**

## Powiązane

- [[Dashboard_Today]]
