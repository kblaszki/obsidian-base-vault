---
type: place
place_type: city
status: visited
parent: "[[Lazio]]"
visited_date: 2024-09-11
rating: 5
map_url:
source_url:
created_date: 2026-10-31
tags:
  - travel
  - place
icon: 📍
banner: "[[./assets/rome-pantheon.jpg]]"
banner_position: center
---

# Rome

## Why visit

Capital density of landmarks; base for [[Colosseum]] and [[Pantheon]] during [[Rome and Florence 2024]].

## Practical info

- **Best time:** Spring or early autumn
- **How to get there:** FCO + Leonardo Express / taxis
- **Cost / tickets:** Timed entries essential for big sites
- **Hours:** Churches often close midday

## Highlights

- Centro Storico walks
- Trastevere evenings
- Forum + Palatine pairing with the Colosseum

## Visit log

- Visited 2024-09-08 to 2024-09-12 on [[Rome and Florence 2024]].

## Child places

```dataview
TABLE WITHOUT ID file.link AS Place, place_type AS Kind, status AS Status
FROM "40_Resources/Places"
WHERE parent = this.file.link
SORT place_type ASC, file.name ASC
```

## Trips

```dataview
LIST
FROM "20_Projects/Trips"
WHERE type = "trip" AND contains(file.outlinks, this.file.link)
SORT start_date DESC
```

## Related

- Parent: [[Lazio]]
- [[Colosseum]]
- [[Pantheon]]
- [[Travel]]
- [[Dashboard_Travel]]
