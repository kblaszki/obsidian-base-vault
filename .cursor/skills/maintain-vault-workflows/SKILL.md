---
name: maintain-vault-workflows
description: Maintains Obsidian templates, QuickAdd choices, Daily Notes routing, and Dataview dashboards as one coherent workflow. Use when changing capture automation or vault organization.
---

# Maintain vault workflows

Treat each workflow as a connected chain:

`hotkey → QuickAdd choice → template → destination → properties → Dataview query`

When changing any link:

1. Inspect every downstream path, property, and query.
2. Keep QuickAdd prompt names stable when reused within a template.
3. Use Templater for computed values and QuickAdd for interactive capture.
4. Write option lists as `{{VALUE:a,b,c|name:field|label:Field}}`. Never encode enums as `{{VALUE:Field (a, b, c)}}`.
5. Prefer `{{VDATE:name,YYYY-MM-DD}}` for dates and `{{FILE:folder|link}}` for note links.
6. Ensure new note types are visible in an existing dashboard or intentionally excluded.
7. Update `README.md` when behavior, installation, or user-facing structure changes.
8. Run the `validate-vault` skill before completion.

Do not replace the core Daily Notes format strategy: dynamic year and month directories belong in `YYYY/MMMM/YYYY-MM-DD`.
