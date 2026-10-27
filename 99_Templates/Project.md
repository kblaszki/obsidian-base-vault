---
type: project
status: "{{VALUE:planned,active,on-hold|name:status|label:Status}}"
area: "{{FILE:30_Areas|link|label:Area}}"
tags:
  - project
  - "{{VALUE:topic|label:Topic tag without #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
review_date: <% moment().add(7, "days").format("YYYY-MM-DD") %>
target_date: "{{VDATE:target_date,YYYY-MM-DD|label:Target date|optional}}"
icon: 🚀
---

# <% tp.file.title %>

## Outcome

{{VALUE:outcome|label:What does done look like?|type:multiline}}

## Why


## Next actions

- [ ] {{VALUE:next_action|label:First next action}} {{VDATE:target_date,[📅 ]YYYY-MM-DD|optional}}

## Milestones

- [ ] 

## Notes


## Resources

- 

## Review

- **Last reviewed:** <% tp.date.now("YYYY-MM-DD") %>
- **Next review:** <% moment().add(7, "days").format("YYYY-MM-DD") %>

## Related

- [[Dashboard_Projects]]
