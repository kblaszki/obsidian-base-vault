---
type: "{{VALUE:task,note|name:type|label:Type}}"
status: "{{VALUE:inbox,next,waiting,done|name:status|label:Status}}"
project: "{{FILE:20_Projects|link|label:Project|optional}}"
due: "{{VDATE:due,YYYY-MM-DD|label:Due date|optional}}"
tags:
  - inbox
  - "{{VALUE:topic|label:Topic tag without #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
icon: 📥
---

# <% tp.file.title %>

## Context

{{VALUE:context|label:What needs attention?|type:multiline}}

## Next action

- [ ] <% tp.file.cursor(1) %> {{VDATE:due,[📅 ]YYYY-MM-DD|optional}}

## Notes


## Processing checklist

- [ ] Clarify the desired outcome
- [ ] Link to a project or area
- [ ] Move out of `00_Inbox` or archive
