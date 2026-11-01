---
name: create-vault-note
description: Creates or updates Obsidian notes using this vault's PARA folders, properties, links, and task conventions. Use when adding projects, areas, resources, inbox items, journals, trips, places, or MOCs.
---

# Create a vault note

1. Identify the note type and route it:
   - raw or unclear → `00_Inbox`
   - time-bound outcome → `20_Projects/Active`
   - trip plan → `20_Projects/Trips`
   - trip day log → `20_Projects/Trips/<Trip title>/days/`
   - trip tip → `20_Projects/Trips/<Trip title>/tips/`
   - trip prep → `20_Projects/Trips/<Trip title>/prep/`
   - ongoing responsibility → `30_Areas`
   - reusable reference → `40_Resources`
   - place / city / attraction → `40_Resources/Places/<Country>/`
   - inactive material → `50_Archives`
2. Reuse the closest file in `99_Templates` and the established property contract.
3. Use ISO dates and valid status values already present for that note type.
4. For trip support notes, the folder name must match the trip note title.
5. Trip-day notes use: short summary, Day timeline, Logistics, Places, Food (with costs), Pack today, Notes, Related. Banners from the trip root assets folder use `banner: "[[../assets/<file>]]"`.
6. Keep prep note filenames unique across trips (e.g. `Packing — <Trip title>.md`).
7. Attachments go to `./assets` relative to the note (vault `attachmentFolderPath`).
8. Add at least one meaningful link when a real relationship exists; do not manufacture links.
9. Add one concrete next action for actionable notes.
10. Run the `validate-vault` skill before completion.
