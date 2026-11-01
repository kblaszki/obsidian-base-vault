# Obsidian PARA Vault Skeleton

A ready-to-use Obsidian vault optimized for low-friction capture, periodic review,
and progressive organization. Open this repository as a vault, then install the
community plugins listed below.

## Directory tree

```text
.
├── 00_Inbox/
│   ├── Review mobile capture.md
│   └── Triage vendor proposal.md
├── 10_Journals/
│   ├── Daily_notes/
│   │   └── 2026/
│   │       └── October/
│   │           └── 2026-10-27.md
│   ├── Weekly/
│   │   └── README.md
│   └── Monthly/
│       └── README.md
├── 20_Projects/
│   ├── Active/
│   │   ├── Launch Knowledge Hub.md
│   │   └── Vault Automation.md
│   ├── Trips/
│   │   ├── Rome and Florence 2024.md          # completed
│   │   ├── Lisbon and Porto 2025.md           # completed
│   │   ├── Scottish Highlands 2025.md         # completed
│   │   ├── Japan Spring 2026.md               # planned soon
│   │   ├── Iceland Ring Road.md               # planned, undated
│   │   └── <Trip title>/
│   │       ├── days/                          # trip-day notes
│   │       ├── tips/                          # transit, driving, money, …
│   │       ├── prep/                          # packing, bookings, admin
│   │       └── assets/                        # banners / photos
│   └── Dashboard_Projects.md
├── 30_Areas/
│   ├── Knowledge Management.md
│   ├── Software Development.md
│   └── Travel.md
├── 40_Resources/
│   ├── Books/                                 # 5 demo notes
│   ├── Articles/                              # 5 demo notes
│   ├── Videos/                                # 5 demo notes
│   ├── Courses/                               # 5 demo notes
│   ├── Recipes/                               # recipe notes + demos
│   └── Places/                                # nested place hierarchy
│       └── <Country>/<Region>/<City>/…        # Folder Notes: Name/Name.md
├── 50_Archives/
│   └── README.md
├── 90_Dashboards/
│   ├── Home.md
│   ├── Dashboard_Today.md
│   ├── Dashboard_Inbox.md
│   └── Dashboard_Travel.md
├── 99_Templates/
│   ├── Daily Note.md
│   ├── Project.md
│   ├── Resource Book.md
│   ├── Task Note.md
│   ├── Trip.md
│   ├── Trip Day.md
│   ├── Trip Tip.md
│   ├── Trip Prep.md
│   ├── Place.md
│   └── Recipe.md
└── .obsidian/
    ├── app.json
    ├── community-plugins.json
    ├── core-plugins.json
    ├── daily-notes.json
    ├── hotkeys.json
    ├── templates.json
    └── plugins/
        ├── calendar/data.json
        ├── dataview/data.json
        ├── folder-notes/data.json
        ├── obsidian-linter/data.json
        ├── obsidian-map-view/data.json
        ├── pretty-properties/data.json
        ├── quickadd/data.json
        └── templater-obsidian/data.json
```

`90_Dashboards` is the only addition to the requested top-level structure. It
keeps operational views separate from reference material and prevents dashboards
from polluting PARA search results.

## First-run setup

1. Open this directory with **Open folder as vault**.
2. In **Settings → Community plugins**, turn off Restricted mode.
3. Install and enable: Dataview, Templater, QuickAdd, Calendar, Pretty
   Properties, Omnisearch, Linter, Folder Notes (`folder-notes`), and Map View
   (`obsidian-map-view`). `community-plugins.json` enables them after they are
   installed; plugin binaries are intentionally not committed. Folder Notes is
   scoped so only `40_Resources/Places` uses folder notes (`Name/Name.md`
   inside the folder). In Map View settings, set an OpenStreetMap user email
   (Nominatim requirement); optionally switch geocoding to Google with a local
   API key — never commit API keys.
4. Restart Obsidian once so every committed `data.json` is loaded.
5. Open `90_Dashboards/Home.md`.

The core Daily Notes plugin uses:

```json
{
  "folder": "10_Journals/Daily_notes",
  "format": "YYYY/MMMM/YYYY-MM-DD",
  "template": "99_Templates/Daily Note"
}
```

Putting `YYYY/MMMM` in `format` is required because the core plugin does not
interpolate variables in its folder setting. The format creates the desired
path automatically.

## Capture workflows

- **Ctrl+N** opens the QuickAdd chooser. Choose Project, Resource, New Recipe,
  Task / Note, Trip, Trip Day, Trip Tip, Trip Prep, New Place (container),
  or New Place (attraction). QuickAdd asks for the title and metadata, routes
  the file, and executes the Templater expressions.
- **Project** creates a note in `20_Projects/Active` and prompts for status,
  area, tag, and target date.
- **Resource** asks for a destination under `40_Resources` (`Books`,
  `Articles`, `Videos`, or `Courses`) and prompts for type, author, status,
  and topic tag.
- **New Recipe** creates a recipe in `40_Resources/Recipes` with cuisine,
  meal, servings, timing, and status (`wishlist` / `tried` / `favorite`).
- **Task / Note** creates an inbox item in `00_Inbox` and prompts for type,
  status, tag, due date, and optional project link.
- **Trip** creates a plan in `20_Projects/Trips` with dates, countries, and
  prep tasks. Demo vault includes three completed weeks, one upcoming Japan
  itinerary, and one undated Iceland draft.
- **Trip Day** creates a day log under
  `20_Projects/Trips/<Trip folder name>/days/`. Use the exact trip note title
  as the folder name. Undated drafts may use `Day 01.md` … with `day_number`.
  Day notes use: summary, Day timeline, Logistics, Places, Food, Pack today,
  Notes. Banners use `[[../assets/<file>]]` because days sit one level deeper
  than `assets/` (vault attachment path is still `./assets`).
- **Trip Tip** creates on-the-ground guidance under
  `20_Projects/Trips/<Trip folder name>/tips/` (`type: trip-tip`).
- **Trip Prep** creates pre-departure checklists under
  `20_Projects/Trips/<Trip folder name>/prep/` (`type: trip-prep`), e.g. packing
  and bookings. Keep prep filenames unique across trips.
- **New Place (container)** creates a country/region/city Folder Note as
  `<Parent>/<Title>/<Title>.md` under `40_Resources/Places` (pick the parent
  folder; use the Places root for a country). Set `place_type` accordingly and
  leave `parent` empty only for countries.
- **New Place (attraction)** creates `<Title>.md` inside the selected parent
  folder (city or region) with `parent` pointing at that place.
- Place notes use photo banners via `banner: "[[./assets/<file>]]"` (and
  `banner_position: center`). Store images next to the note under `./assets`
  and record Commons attribution in `40_Resources/Places/SOURCES.md`.
- Places carry dual map fields: `map_url` (Google Maps link for phone/vacation)
  and `location: [lat, lng]` (Map View pins in Obsidian). Related includes a
  clickable Map line. Map View's Open in Google Maps uses the same coordinates.
- **Daily note** uses the Calendar or Daily Notes command. It is filed under
  the year/month path and includes navigation, tasks, log, and review prompts.

QuickAdd enum prompts use option lists with `|name:` and `|label:`, for
example `{{VALUE:book,article,video,course|name:resource_type|label:Resource type}}`.
Do not put commas inside a plain named prompt like
`{{VALUE:Status (a, b, c)}}` — QuickAdd treats those commas as options.
Dates use `{{VDATE:...}}`, and note pickers use `{{FILE:...|link}}`.
One-page input is enabled so related prompts appear together. Templater then
runs JavaScript for calculated values such as review dates and daily navigation.

## Properties contract

Use properties for structured, queryable facts and inline tags for context:

- `type`: `project`, `resource`, `task`, `note`, `daily`, `area`, `trip`,
  `trip-day`, `trip-tip`, `trip-prep`, `place`, `recipe`
- `status`: stable workflow state, such as `active`, `planned`, `waiting`,
  `done`, `to-read`, `wishlist`, `visited`, `completed`, `cancelled`
- `place_type`: `country`, `region`, `city`, `attraction`
- `parent`: wiki link to the parent place; empty only for countries
- `map_url`: Google Maps URL for on-the-go navigation
- `location`: `[lat, lng]` for Map View (also accepts `"lat,lng"`)
- `created_date`, `due`, `target_date`, `review_date`, `start_date`,
  `end_date`, `visited_date`: ISO dates
- `area`, `project`, `trip`: links to durable parent notes
- `countries`: travel geography on trip notes (plain names or links)
- `tags`: broad topics, not status duplication

Prefer links (`area: "[[Knowledge Management]]"`) for entities and relationships.
Prefer tags (`#topic/pkm`) for cross-cutting facets. Avoid deeply nested tags.

## Dashboard behavior

- `Dashboard_Today.md` shows today's daily note and incomplete tasks due today
  or overdue.
- `Dashboard_Projects.md` groups open projects by status and highlights review
  and target dates.
- `Dashboard_Inbox.md` lists unsorted notes and their age.
- `Dashboard_Travel.md` shows upcoming/undated trips, completed trips, trip
  days (including `day_number` drafts), places with Google Maps links, and an
  embedded Map View of `40_Resources/Places`.

Enable **Dataview → Enable JavaScript Queries** for the DataviewJS sections.

## Complementary plugins

- **Omnisearch**: fast full-text search with ranking and OCR support; useful once
  the resource collection grows.
- **Linter**: normalizes YAML, dates, headings, and whitespace. The committed
  preset runs safely on save without changing semantic content.
- **Auto Note Mover** (optional): useful for routing by `type`, but omitted from
  active configuration because it can move notes unexpectedly and conflict with
  QuickAdd. Add it only after the property taxonomy is stable.

## Operating rhythm

1. Capture first; route later if context is missing.
2. Empty `00_Inbox` during the daily shutdown or weekly review.
3. Review active projects weekly; archive completed work by moving the project
   note and its support folder to `50_Archives/Projects`.
4. Create MOCs in `30_Areas` for stable domains. Link projects and resources to
   these MOCs rather than recreating a deep folder tree.
5. Keep folders shallow. PARA describes actionability; links and properties
   describe meaning.
6. For travel, keep one trip note, optional day/tips/prep notes under a matching
   folder, and nested places under `40_Resources/Places` (`country → region →
   city → attraction` with Folder Notes on containers). Store trip photos in
   `20_Projects/Trips/<Trip>/assets/` and attribute Commons sources in
   `assets/SOURCES.md`.

Weekly and monthly folders are intentionally lightweight: create notes there
only when a review is performed. This avoids empty ritual notes and keeps the
system useful rather than ceremonial.
