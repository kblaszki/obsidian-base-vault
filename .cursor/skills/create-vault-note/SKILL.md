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
   - place country → `40_Resources/Places/<Country>/<Country>.md`
   - place region/city → under parent folder as `<Name>/<Name>.md` with `parent: "[[Parent]]"`
   - place attraction → file inside parent folder `<ParentPath>/<Attraction>.md` with `parent` set
   - inactive material → `50_Archives`
2. Reuse the closest file in `99_Templates` and the established property contract.
3. Use ISO dates and valid status values already present for that note type.
4. For trip support notes, the folder name must match the trip note title.
5. Trip-day notes use: short summary, Day timeline, Logistics, Places, Food (with costs), Pack today, Notes, Related. Banners from the trip root assets folder use `banner: "[[../assets/<file>]]"`.
6. Keep prep note filenames unique across trips (e.g. `Packing — <Trip title>.md`).
7. For places: always set `place_type`; set `parent` on every non-country note; containers use Folder Note paths (`Name/Name.md`); do not add Folder Notes outside `40_Resources/Places`.
8. Attachments go to `./assets` relative to the note (vault `attachmentFolderPath`).
9. Add at least one meaningful link when a real relationship exists; do not manufacture links.
10. Add one concrete next action for actionable notes.
11. Run the `validate-vault` skill before completion.
