---
type: "{{VALUE:Type (task or note)}}"
status: "{{VALUE:Status (inbox, next, waiting, done)}}"
project: "{{VALUE:Project link (optional)}}"
due: "{{VALUE:Due date YYYY-MM-DD (optional)}}"
tags:
  - inbox
  - "{{VALUE:Topic tag without #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
icon: 📥
---

# <% tp.file.title %>

## Context

{{VALUE:What needs attention?}}

## Next action

- [ ] <% tp.file.cursor(1) %>

## Notes


## Processing checklist

- [ ] Clarify the desired outcome
- [ ] Link to a project or area
- [ ] Move out of `00_Inbox` or archive
