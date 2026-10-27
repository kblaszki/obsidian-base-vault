---
type: daily
date: <% tp.date.now("YYYY-MM-DD") %>
created_date: <% tp.date.now("YYYY-MM-DDTHH:mm") %>
tags:
  - journal/daily
---

# <% tp.date.now("dddd, MMMM D, YYYY") %>

<%*
const noteDate = moment(tp.file.title, "YYYY-MM-DD");
const previous = noteDate.clone().subtract(1, "day").format("YYYY-MM-DD");
const next = noteDate.clone().add(1, "day").format("YYYY-MM-DD");
tR += `[[${previous}|← Previous]] · [[${next}|Next →]]`;
%>

## Focus

- [ ] <% tp.file.cursor(1) %>

## Tasks

- [ ] 

## Log

- <% tp.date.now("HH:mm") %> 

## Notes


## End-of-day review

- **Win:** 
- **Learned:** 
- **Carry forward:** 

## Related

- [[Dashboard_Today]]
