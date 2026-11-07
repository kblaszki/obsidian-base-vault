---
type: trip-day
trip: "{{FILE:20_Projects/Trips|link|label:Wyjazd}}"
date: "{{VDATE:date,YYYY-MM-DD|label:Dzień}}"
day_number:
created_date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - travel
  - trip-day
banner:
banner_position: center
---

# <% tp.file.title %>

{{VALUE:summary|label:Krótki opis dnia|type:multiline}}


## Harmonogram dnia

- {{VALUE:first_time|label:Pierwsza godzina|default:09:00}} — {{VALUE:first_timeline|label:Pierwszy punkt harmonogramu}}

## Logistyka

-

## Miejsca

- [[]] — *(krótki przystanek / 1–2h / pół dnia)*

## Jedzenie

- **Śniadanie:**
- **Obiad:**
- **Kolacja:**
- **Zakupy / przekąski:**

### Koszty

| Pozycja | Kwota | Uwagi |
|---------|-------|-------|
|         |       |       |

## Spakuj dziś

- **Dokumenty:**
- **Ubrania:**
- **Gotówka / karty:**
- **Sprzęt:**

## Notatki

{{VALUE:day_notes|label:Dodatkowe notatki|type:multiline|optional}}

## Powiązane

- {{FILE:20_Projects/Trips|link|label:Wyjazd}}
- [[Dashboard_Travel]]
