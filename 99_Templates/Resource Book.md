---
type: resource
resource_type: "{{VALUE:book,article,video,course|name:resource_type|label:Resource type}}"
status: "{{VALUE:to-read,reading,processed|name:status|label:Status}}"
author: "{{VALUE:author|label:Author or creator}}"
source_url: "{{VALUE:source_url|label:Source URL or ISBN|optional}}"
tags:
  - resource
  - "{{VALUE:topic|label:Topic tag without #}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
finished_date:
rating:
icon: 📚
---

# <% tp.file.title %>

## Summary

{{VALUE:summary|label:Why save this?|type:multiline}}

## Key ideas

- <% tp.file.cursor(1) %>

## Highlights

> 

## My interpretation


## Actions

- [ ] 

## Connections

- Area: {{FILE:30_Areas|link|label:Related area|optional}}
- Project: {{FILE:20_Projects|link|label:Related project|optional}}
