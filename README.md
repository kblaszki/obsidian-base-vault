# Szkielet sejfu Obsidian PARA

Gotowy sejf Obsidian zoptymalizowany pod szybkie przechwytywanie, okresowy przegląd
i stopniową organizację. Otwórz to repozytorium jako sejf, a następnie zainstaluj
wtyczki społecznościowe wymienione poniżej.

## Drzewo katalogów

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
│   │   └── <Trip title>/                      # Folder Note wyjazdu
│   │       ├── <Trip title>.md                # plan wyjazdu (folder note)
│   │       ├── days/                          # notatki dni wyjazdu
│   │       ├── tips/                          # transport, jazda, pieniądze, …
│   │       ├── prep/                          # pakowanie, rezerwacje, admin
│   │       └── assets/                        # banery / zdjęcia
│   └── Dashboard_Projects.md
├── 30_Areas/
│   ├── Knowledge Management.md
│   ├── Software Development.md
│   └── Travel.md
├── 40_Resources/
│   ├── Books/                                 # 5 notatek demo
│   ├── Articles/                              # 5 notatek demo
│   ├── Videos/                                # 5 notatek demo
│   ├── Courses/                               # 5 notatek demo
│   ├── Recipes/                               # przepisy + demo
│   └── Places/                                # zagnieżdżona hierarchia miejsc
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

`90_Dashboards` to jedyny dodatek do żądanej struktury najwyższego poziomu. Trzyma
widoki operacyjne osobno od materiału referencyjnego i nie zaśmieca wyników
wyszukiwania PARA.

## Pierwsze uruchomienie

1. Otwórz ten katalog przez **Open folder as vault**.
2. W **Settings → Community plugins** wyłącz Restricted mode.
3. Zainstaluj i włącz: Dataview, Templater, QuickAdd, Calendar, Pretty
   Properties, Omnisearch, Linter, Folder Notes (`folder-notes`) oraz Map View
   (`obsidian-map-view`). `community-plugins.json` włącza je po instalacji;
   binaria wtyczek celowo nie są w repozytorium. Folder Notes działają dla
   kontenerów Places i Trips (`Name/Name.md`); foldery pomocnicze jak `days/`
   i `assets/` są wykluczone. Banery Pretty Properties pozostają włączone;
   ikony są wyłączone. W ustawieniach Map View podaj e-mail użytkownika
   OpenStreetMap (wymóg Nominatim); opcjonalnie przełącz geokodowanie na Google
   z lokalnym kluczem API — nigdy nie commituj kluczy API.
4. Zrestartuj Obsidian raz, żeby wczytać wszystkie commitowane `data.json`.
5. Otwórz `90_Dashboards/Home.md`.

Wtyczka rdzeniowa Daily Notes używa:

```json
{
  "folder": "10_Journals/Daily_notes",
  "format": "YYYY/MMMM/YYYY-MM-DD",
  "template": "99_Templates/Daily Note"
}
```

`YYYY/MMMM` w `format` jest wymagane, bo wtyczka rdzeniowa nie interpoluje
zmiennych w ustawieniu folderu. Format sam tworzy żądaną ścieżkę.

## Przepływy przechwytywania

- **Ctrl+N** otwiera wybór QuickAdd. Wybierz: Nowy projekt, Nowy zasób, Nowy przepis,
  Nowe zadanie / notatka, Nowy wyjazd, Nowy dzień wyjazdu, Nowa wskazówka wyjazdu,
  Nowe przygotowanie wyjazdu, Nowe miejsce (kontener) lub Nowe miejsce (atrakcja).
  QuickAdd pyta o tytuł i metadane, umieszcza plik i uruchamia wyrażenia Templatera.
- **Nowy projekt** tworzy notatkę w `20_Projects/Active` i pyta o status, obszar,
  tag oraz datę docelową.
- **Nowy zasób** pyta o katalog docelowy w `40_Resources` (`Books`, `Articles`,
  `Videos` lub `Courses`) oraz o typ, autora, status i tag tematyczny.
- **Nowy przepis** tworzy przepis w `40_Resources/Recipes` z kuchnią, posiłkiem,
  porcjami, czasem i statusem (`wishlist` / `tried` / `favorite`).
- **Nowe zadanie / notatka** tworzy element w `00_Inbox` i pyta o typ, status,
  tag, termin oraz opcjonalny link do projektu.
- **Nowy wyjazd** tworzy Folder Note pod
  `20_Projects/Trips/<Trip title>/<Trip title>.md` i zapewnia foldery `days/`,
  `tips/`, `prep/` oraz `assets/`. Sejf demo zawiera trzy ukończone tygodnie,
  nadchodzący itinerariusz Japonii oraz niedatowany szkic Islandii.
- **Nowy dzień wyjazdu** tworzy dziennik dnia w
  `20_Projects/Trips/<Trip folder name>/days/`. Użyj dokładnego tytułu notatki
  wyjazdu jako nazwy folderu. Niedatowane szkice mogą używać `Day 01.md` …
  z `day_number`. Notatki dnia mają: podsumowanie, Plan dnia, Logistyka, Miejsca,
  Jedzenie, Spakuj dziś, Notatki. Banery używają `[[../assets/<file>]]`, bo dni
  leżą poziom głębiej niż `assets/` (ścieżka załączników sejfu to nadal `./assets`).
- **Nowa wskazówka wyjazdu** tworzy wskazówki terenowe w
  `20_Projects/Trips/<Trip folder name>/tips/` (`type: trip-tip`).
- **Nowe przygotowanie wyjazdu** tworzy checklisty przed wyjazdem w
  `20_Projects/Trips/<Trip folder name>/prep/` (`type: trip-prep`), np. pakowanie
  i rezerwacje. Nazwy plików prep powinny być unikalne między wyjazdami.
- **Nowe miejsce (kontener)** tworzy Folder Note kraju/regionu/miasta jako
  `<Parent>/<Title>/<Title>.md` pod `40_Resources/Places` (wybierz folder
  nadrzędny; korzeń Places dla kraju). Ustaw `place_type` odpowiednio i zostaw
  `parent` puste tylko dla krajów.
- **Nowe miejsce (atrakcja)** tworzy `<Title>.md` w wybranym folderze rodzica
  (miasto lub region) z `parent` wskazującym to miejsce.
- Notatki miejsc używają banerów zdjęć przez `banner: "[[./assets/<file>]]"` (oraz
  `banner_position: center`). Przechowuj obrazy obok notatki w `./assets`
  i zapisuj atrybucję Commons w `40_Resources/Places/SOURCES.md`.
- Miejsca mają podwójne pola mapy: `map_url` (link Google Maps na telefon/wakacje)
  oraz `location: [lat, lng]` (pinezki Map View w Obsidian). Related zawiera
  klikalną linię Mapa. Open in Google Maps w Map View używa tych samych
  współrzędnych.
- **Notatka dzienna** powstaje z Calendar lub komendy Daily Notes. Trafia pod
  ścieżkę rok/miesiąc i zawiera nawigację, zadania, log oraz pytania przeglądu.

Prompty enumów QuickAdd używają list opcji z `|name:` i `|label:`, na przykład
`{{VALUE:book,article,video,course|name:resource_type|label:Typ zasobu}}`.
Nie wstawiaj przecinków do zwykłego nazwanego promptu jak
`{{VALUE:Status (a, b, c)}}` — QuickAdd traktuje te przecinki jako opcje.
Daty używają `{{VDATE:...}}`, a wybór notatek `{{FILE:...|link}}`.
Włączone jest wprowadzanie na jednej stronie, więc powiązane prompty pojawiają
się razem. Templater potem uruchamia JavaScript dla wartości wyliczanych,
takich jak daty przeglądu i nawigacja dzienna.

## Kontrakt właściwości

Używaj właściwości do faktów strukturalnych i zapytywalnych, a tagów inline do kontekstu:

- `type`: `project`, `resource`, `task`, `note`, `daily`, `area`, `trip`,
  `trip-day`, `trip-tip`, `trip-prep`, `place`, `recipe`
- `status`: stabilny stan workflow, np. `active`, `planned`, `waiting`,
  `done`, `to-read`, `wishlist`, `visited`, `completed`, `cancelled`
- `place_type`: `country`, `region`, `city`, `attraction`
- `parent`: wiki link do miejsca nadrzędnego; puste tylko dla krajów
- `map_url`: URL Google Maps do nawigacji w terenie
- `location`: `[lat, lng]` dla Map View (akceptuje też `"lat,lng"`)
- `created_date`, `due`, `target_date`, `review_date`, `start_date`,
  `end_date`, `visited_date`: daty ISO
- `area`, `project`, `trip`: linki do trwałych notatek nadrzędnych
- `countries`: geografia podróży na notatkach wyjazdów (zwykłe nazwy lub linki)
- `tags`: szerokie tematy, bez duplikowania statusu

Preferuj linki (`area: "[[Knowledge Management]]"`) dla encji i relacji.
Preferuj tagi (`#topic/pkm`) dla przekrojowych facetów. Unikaj głęboko
zagnieżdżonych tagów.

## Zachowanie dashboardów

- `Dashboard_Today.md` pokazuje dzisiejszą notatkę dzienną oraz niedokończone
  zadania z terminem dziś lub przeterminowane.
- `Dashboard_Projects.md` grupuje otwarte projekty według statusu i podkreśla
  daty przeglądu oraz docelowe.
- `Dashboard_Inbox.md` listuje nieposortowane notatki i ich wiek.
- `Dashboard_Travel.md` pokazuje nadchodzące/niedatowane wyjazdy, ukończone
  wyjazdy, dni wyjazdów (w tym szkice z `day_number`), miejsca z linkami Google
  Maps oraz osadzony Map View `40_Resources/Places`.

Włącz **Dataview → Enable JavaScript Queries** dla sekcji DataviewJS.

## Wtyczki uzupełniające

- **Omnisearch**: szybkie wyszukiwanie pełnotekstowe z rankingiem i OCR; przydatne,
  gdy kolekcja zasobów urośnie.
- **Linter**: normalizuje YAML, daty, nagłówki i białe znaki. Commitowany preset
  działa bezpiecznie przy zapisie bez zmiany treści semantycznej.
- **Auto Note Mover** (opcjonalnie): przydatny do routingu po `type`, ale
  pominięty w aktywnej konfiguracji, bo może nieoczekiwanie przenosić notatki
  i kolidować z QuickAdd. Dodaj dopiero gdy taksonomia właściwości jest stabilna.

## Rytm pracy

1. Najpierw przechwytuj; kieruj później, jeśli brakuje kontekstu.
2. Opróżniaj `00_Inbox` przy codziennym zamknięciu lub tygodniowym przeglądzie.
3. Przeglądaj aktywne projekty co tydzień; archiwizuj ukończoną pracę, przenosząc
   notatkę projektu i folder wsparcia do `50_Archives/Projects`.
4. Twórz MOC-e w `30_Areas` dla stabilnych domen. Linkuj projekty i zasoby do
   tych MOC-ów zamiast budować głębokie drzewo folderów.
5. Trzymaj foldery płytkie. PARA opisuje actionable; linki i właściwości opisują
   znaczenie.
6. Dla podróży trzymaj jedną notatkę wyjazdu, opcjonalne dni/wskazówki/prep w
   pasującym folderze oraz zagnieżdżone miejsca pod `40_Resources/Places`
   (`country → region → city → attraction` z Folder Notes na kontenerach).
   Zdjęcia wyjazdów trzymaj w `20_Projects/Trips/<Trip>/assets/` i atrybuuj
   źródła Commons w `assets/SOURCES.md`.

Foldery tygodniowe i miesięczne są celowo lekkie: twórz tam notatki tylko gdy
wykonujesz przegląd. Unika to pustych rytualnych notatek i utrzymuje system
użytecznym, a nie ceremonialnym.
