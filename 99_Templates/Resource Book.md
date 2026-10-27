---
type: resource
resource_type: "{{VALUE:Resource type (book, article, video, course)}}"
status: "{{VALUE:Status (to-read, reading, processed)}}"
author: "{{VALUE:Author or creator}}"
source_url: "{{VALUE:Source URL or ISBN}}"
tags:
  - resource
  - "{{VALUE:Topic tag without #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
finished_date:
rating:
icon: 📚
---

# <% tp.file.title %>

## Summary

{{VALUE:One-sentence reason for saving this}}

## Key ideas

- <% tp.file.cursor(1) %>

## Highlights

> 

## My interpretation


## Actions

- [ ] 

## Connections

- Area: [[{{VALUE:Related area note name}}]]
- Project: 
