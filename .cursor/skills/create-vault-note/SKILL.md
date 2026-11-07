---
name: create-vault-note
description: Tworzy lub aktualizuje notatki Obsidian według folderów PARA, właściwości, linków i konwencji zadań tego sejfu. Używaj przy dodawaniu projektów, obszarów, zasobów, skrzynki, dzienników, wyjazdów, miejsc lub MOC-ów.
---

# Tworzenie notatki sejfu

1. Określ typ notatki i skieruj ją:
   - surowa lub niejasna → `00_Inbox`
   - wynik ograniczony w czasie → `20_Projects/Active`
   - plan wyjazdu → `20_Projects/Trips/<Trip title>/<Trip title>.md` (Folder Note; foldery wsparcia `days/`, `tips/`, `prep/`, `assets/`)
   - dziennik dnia wyjazdu → `20_Projects/Trips/<Trip title>/days/`
   - wskazówka wyjazdu → `20_Projects/Trips/<Trip title>/tips/`
   - przygotowanie wyjazdu → `20_Projects/Trips/<Trip title>/prep/`
   - stała odpowiedzialność → `30_Areas`
   - materiał referencyjny → `40_Resources`
   - przepis → `40_Resources/Recipes`
   - miejsce (kraj) → `40_Resources/Places/<Country>/<Country>.md`
   - miejsce (region/miasto) → pod folderem rodzica jako `<Name>/<Name>.md` z `parent: "[[Parent]]"`
   - miejsce (atrakcja) → plik w folderze rodzica `<ParentPath>/<Attraction>.md` z ustawionym `parent`
   - materiał nieaktywny → `50_Archives`
2. Ponownie użyj najbliższego pliku z `99_Templates` i ustalonego kontraktu właściwości.
3. Używaj dat ISO i poprawnych wartości statusu już obecnych dla danego typu notatki.
4. Wyjazdy to Folder Notes (`<Title>/<Title>.md`). Notatki wsparcia leżą obok folder note; nazwa folderu wyjazdu musi zgadzać się z tytułem notatki wyjazdu.
5. Notatki dnia wyjazdu mają: krótkie podsumowanie, Plan dnia, Logistyka, Miejsca, Jedzenie (z kosztami), Spakuj dziś, Notatki, Powiązania. Banery z folderu `assets` korzenia wyjazdu: `banner: "[[../assets/<file>]]"`.
6. Nazwy plików prep muszą być unikalne między wyjazdami (np. `Packing — <Trip title>.md`).
7. Dla miejsc: zawsze ustaw `place_type`; ustaw `parent` na każdej notatce nie-krajowej; kontenery używają ścieżek Folder Note (`Name/Name.md`). Folder Notes są używane tylko dla kontenerów Places i Trips. Ustaw `map_url` (Google Maps) oraz `location: [lat, lng]` (Map View). Notatki miejsc używają `banner: "[[./assets/<file>]]"` i `banner_position: center`; atrybuuj źródła Commons w `40_Resources/Places/SOURCES.md`.
8. Nie ustawiaj `icon` Pretty Properties na notatkach; banery pozostają dozwolone.
9. Załączniki trafiają do `./assets` względem notatki (vault `attachmentFolderPath`).
10. Dodaj co najmniej jeden sensowny link, gdy istnieje realna relacja; nie wymuszaj linków.
11. Dodaj jedną konkretną kolejną akcję dla notatek actionable.
12. Przed zakończeniem uruchom skill `validate-vault`.
