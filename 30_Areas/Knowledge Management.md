---
type: area
status: active
tags:
  - area
  - topic/pkm
created_date: 2026-10-01
review_frequency: monthly
icon: 🧠
---

# Knowledge Management

Maintain a trustworthy system for capture, synthesis, retrieval, and reuse.

## Active projects

```dataview
LIST
FROM "20_Projects"
WHERE type = "project" AND area = this.file.link AND status != "archived"
SORT target_date ASC
```

## Key resources

- [[Building a Second Brain]]
- [[Progressive Summarization]]

## Standards

- Every active project has one visible next action.
- Inbox items are clarified before they are moved.
- Durable concepts link back to this MOC.
