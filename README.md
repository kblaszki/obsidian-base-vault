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
│   │   ├── Japan Spring 2026.md
│   │   └── Japan Spring 2026/
│   │       ├── 2026-04-10.md
│   │       └── 2026-04-12.md
│   └── Dashboard_Projects.md
├── 30_Areas/
│   ├── Knowledge Management.md
│   ├── Software Development.md
│   └── Travel.md
├── 40_Resources/
│   ├── Books/
│   │   └── Building a Second Brain.md
│   ├── Articles/
│   │   └── Progressive Summarization.md
│   ├── Videos/
│   │   └── README.md
│   ├── Courses/
│   │   └── README.md
│   └── Places/
│       ├── Japan/
│       │   ├── Tokyo.md
│       │   ├── Kyoto.md
│       │   └── Fushimi Inari.md
│       └── Italy/
│           └── Colosseum.md
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
│   └── Place.md
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
        ├── obsidian-linter/data.json
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
   Properties, Omnisearch, and Linter. `community-plugins.json` enables them
   after they are installed; plugin binaries are intentionally not committed.
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

- **Ctrl+N** opens the QuickAdd chooser. Choose Project, Resource,
  Task / Note, Trip, Trip Day, or Place. QuickAdd asks for the title and
  metadata, routes the file, and executes the Templater expressions.
- **Project** creates a note in `20_Projects/Active` and prompts for status,
  area, tag, and target date.
- **Resource** asks for a destination under `40_Resources` (`Books`,
  `Articles`, `Videos`, or `Courses`) and prompts for type, author, status,
  and topic tag.
- **Task / Note** creates an inbox item in `00_Inbox` and prompts for type,
  status, tag, due date, and optional project link.
- **Trip** creates a plan in `20_Projects/Trips` with dates, countries, and
  prep tasks.
- **Trip Day** creates a day log under `20_Projects/Trips/<Trip folder name>/`.
  Use the exact trip note title as the folder name.
- **Place** creates a country/city/attraction note under
  `40_Resources/Places/<Country>/` with wishlist/planned/visited status.
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
  `trip-day`, `place`
- `status`: stable workflow state, such as `active`, `planned`, `waiting`,
  `done`, `to-read`, `wishlist`, `visited`, `completed`, `cancelled`
- `place_type`: `country`, `city`, `attraction`
- `created_date`, `due`, `target_date`, `review_date`, `start_date`,
  `end_date`, `visited_date`: ISO dates
- `area`, `project`, `trip`: links to durable parent notes
- `country`, `city`, `countries`: travel geography
- `tags`: broad topics, not status duplication

Prefer links (`area: "[[Knowledge Management]]"`) for entities and relationships.
Prefer tags (`#topic/pkm`) for cross-cutting facets. Avoid deeply nested tags.

## Dashboard behavior

- `Dashboard_Today.md` shows today's daily note and incomplete tasks due today
  or overdue.
- `Dashboard_Projects.md` groups open projects by status and highlights review
  and target dates.
- `Dashboard_Inbox.md` lists unsorted notes and their age.
- `Dashboard_Travel.md` shows upcoming trips, trip days, and places grouped by
  country and status.

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
6. For travel, keep one trip note, optional day notes under a matching folder,
   and places grouped by country under `40_Resources/Places`.

Weekly and monthly folders are intentionally lightweight: create notes there
only when a review is performed. This avoids empty ritual notes and keeps the
system useful rather than ceremonial.
