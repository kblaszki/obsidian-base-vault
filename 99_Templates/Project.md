---
type: project
status: "{{VALUE:Status (planned, active, on-hold)}}"
area: "[[{{VALUE:Area note name}}]]"
tags:
  - project
  - "{{VALUE:Topic tag without #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
review_date: <% moment().add(7, "days").format("YYYY-MM-DD") %>
target_date: "{{VALUE:Target date YYYY-MM-DD}}"
icon: 🚀
---

# <% tp.file.title %>

## Outcome

{{VALUE:What does done look like?}}

## Why


## Next actions

- [ ] {{VALUE:First next action}} 📅 {{VALUE:Target date YYYY-MM-DD}}

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
