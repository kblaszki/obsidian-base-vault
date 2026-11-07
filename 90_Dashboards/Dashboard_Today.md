---
type: dashboard
tags:
  - dashboard
  - review/daily
---

# Today

## Dziennik

```dataview
LIST
FROM "10_Journals/Daily_notes"
WHERE date = date(today)
```

## Termin dziś lub zaległe

```dataview
TASK
FROM "00_Inbox" OR "20_Projects" OR "30_Areas" OR "10_Journals"
WHERE !completed AND due AND date(due) <= date(today)
SORT due ASC
```

## Zadania dodane dziś

```dataviewjs
const today = dv.date("today");
const tasks = dv.pages()
  .where(p => !p.file.path.startsWith("99_Templates/"))
  .file.tasks
  .where(t => !t.completed && t.created && dv.date(t.created).hasSame(today, "day"));

dv.taskList(tasks, false);
```

## Dziennik na dziś

```dataviewjs
const today = dv.date("today").toFormat("yyyy-MM-dd");
const page = dv.pages('"10_Journals/Daily_notes"')
  .where(p => p.date && dv.date(p.date).toFormat("yyyy-MM-dd") === today)
  .first();

if (page) {
  dv.paragraph(`Otwórz ${page.file.link}, aby dodać lub przejrzeć wpisy dziennika.`);
} else {
  dv.paragraph("Brak notatki dziennej. Użyj **Open today's daily note**.");
}
```
