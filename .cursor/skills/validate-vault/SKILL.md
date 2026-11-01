---
name: validate-vault
description: Validates this Obsidian vault after changes to notes, templates, dashboards, folders, or plugin configuration. Use before completing any task that modifies the vault.
---

# Validate the vault

1. Parse every `.obsidian/**/*.json` file as strict JSON.
2. Confirm the required PARA, journal, dashboard, and template directories exist.
3. Check changed Markdown files for valid frontmatter delimiters and unresolved static wiki links.
4. For place notes under `40_Resources/Places` (excluding `SOURCES.md`): require non-empty `map_url` starting with `http` and `location` as two numeric coordinates (`[lat, lng]` or `"lat,lng"`).
5. Run `git diff --check`.
6. Inspect `git status --short` and ensure only intended files will be committed.
7. Fix validation failures before handing off or committing.

Generated plugin bundles do not require source linting. Never modify them to silence diagnostics.
