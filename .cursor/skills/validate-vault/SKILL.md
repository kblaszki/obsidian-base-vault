---
name: validate-vault
description: Waliduje ten sejf Obsidian po zmianach w notatkach, szablonach, dashboardach, folderach lub konfiguracji wtyczek. Używaj przed zakończeniem każdego zadania zmieniającego sejf.
---

# Walidacja sejfu

1. Parsuj każdy plik `.obsidian/**/*.json` jako ścisły JSON.
2. Potwierdź istnienie wymaganych katalogów PARA, dzienników, dashboardów i szablonów.
3. Sprawdź zmienione pliki Markdown pod kątem poprawnych delimiterów frontmatteru i nierozwiązanych statycznych wiki linków.
4. Dla notatek miejsc pod `40_Resources/Places` (bez `SOURCES.md`): wymagaj niepustego `map_url` zaczynającego się od `http` oraz `location` jako dwóch współrzędnych numerycznych (`[lat, lng]` lub `"lat,lng"`).
5. Uruchom `git diff --check`.
6. Sprawdź `git status --short` i upewnij się, że commitowane będą tylko zamierzone pliki.
7. Napraw błędy walidacji przed przekazaniem lub commitem.

Wygenerowane paczki wtyczek nie wymagają lintowania źródeł. Nigdy ich nie modyfikuj, by wyciszyć diagnostykę.
