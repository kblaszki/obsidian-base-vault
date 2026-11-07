---
name: maintain-vault-workflows
description: Utrzymuje szablony Obsidian, wybory QuickAdd, routing Daily Notes i dashboardy Dataview jako jeden spójny workflow. Używaj przy zmianach automatyzacji przechwytywania lub organizacji sejfu.
---

# Utrzymanie workflow sejfu

Traktuj każdy workflow jako powiązany łańcuch:

`hotkey → wybór QuickAdd → szablon → miejsce docelowe → właściwości → zapytanie Dataview`

Przy zmianie dowolnego ogniwa:

1. Sprawdź każdą ścieżkę, właściwość i zapytanie w dół łańcucha.
2. Utrzymuj stabilne nazwy promptów QuickAdd, gdy są ponownie używane w szablonie.
3. Używaj Templatera do wartości wyliczanych, a QuickAdd do interaktywnego przechwytywania.
4. Listy opcji zapisuj jako `{{VALUE:a,b,c|name:field|label:Field}}`. Nigdy nie koduj enumów jako `{{VALUE:Field (a, b, c)}}`.
5. Preferuj `{{VDATE:name,YYYY-MM-DD}}` dla dat oraz `{{FILE:folder|link}}` dla linków do notatek.
6. Upewnij się, że nowe typy notatek są widoczne na istniejącym dashboardzie albo celowo wykluczone.
7. Aktualizuj `README.md`, gdy zmienia się zachowanie, instalacja lub struktura widoczna dla użytkownika.
8. Przed zakończeniem uruchom skill `validate-vault`.

Ścieżki wsparcia wyjazdów muszą pozostać zsynchronizowane:

`Nowy dzień wyjazdu → .../<trip>/days` · `Nowa wskazówka wyjazdu → .../<trip>/tips` · `Nowe przygotowanie wyjazdu → .../<trip>/prep`

Nie zastępuj strategii formatu rdzeniowych Daily Notes: dynamiczne katalogi roku i miesiąca należą do `YYYY/MMMM/YYYY-MM-DD`.
