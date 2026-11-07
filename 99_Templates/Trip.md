---
type: trip
status: "{{VALUE:planned,active,completed,cancelled|name:status|label:Status}}"
area: "{{FILE:30_Areas|link|label:Obszar}}"
countries: "{{VALUE:countries|label:Kraje (po przecinku)}}"
start_date: "{{VDATE:start_date,YYYY-MM-DD|label:Data rozpoczęcia}}"
end_date: "{{VDATE:end_date,YYYY-MM-DD|label:Data zakończenia|optional}}"
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - trip
---

# <% tp.file.title %>

## Cel

{{VALUE:outcome|label:Co ma osiągnąć ten wyjazd?|type:multiline}}

## Przegląd itinerarium

-

## Logistyka

- **Loty / transport:**
- **Noclegi:**
- **Dokumenty:**

## Zadania przygotowawcze

Tylko na wysokim poziomie — szczegóły w notatkach `prep/`.

- [ ] {{VALUE:next_action|label:Pierwsze zadanie przygotowawcze}}
- [ ] Utwórz notatki w `prep/` (pakowanie, rezerwacje)

## Miejsca do odwiedzenia

-

## Budżet

-

## Dni

```dataview
TABLE WITHOUT ID file.link AS Notatka, date AS Data, day_number AS Dzień
FROM "20_Projects/Trips"
WHERE type = "trip-day" AND trip = this.file.link
SORT date ASC, day_number ASC
```

## Wskazówki

```dataview
TABLE WITHOUT ID file.link AS Wskazówka, topic AS Temat, status AS Status
FROM "20_Projects/Trips"
WHERE type = "trip-tip" AND trip = this.file.link
SORT topic ASC, file.name ASC
```

## Przygotowanie

```dataview
TABLE WITHOUT ID file.link AS Notatka, prep_kind AS Rodzaj, status AS Status
FROM "20_Projects/Trips"
WHERE type = "trip-prep" AND trip = this.file.link
SORT prep_kind ASC, file.name ASC
```

## Powiązane

- [[Travel]]
- [[Dashboard_Travel]]

<%*
const folder = tp.file.folder(true);
for (const sub of ["days", "tips", "prep", "assets"]) {
  const path = `${folder}/${sub}`;
  if (!(await tp.app.vault.adapter.exists(path))) {
    await tp.app.vault.createFolder(path);
  }
}
%>
