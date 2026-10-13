# Notatka redakcyjna — porządkowanie Codex Iuris Canonici Ecclesiae Domesticae

## Stan wyjściowy (pliki źródłowe .txt)

| Plik | Zawartość | Numeracja kanonów |
|------|-----------|-------------------|
| `ksiegi01.txt` | Księgi I–XI (Kanon zasadniczy) + Aneksy | 1–126 (z wklejonym blokiem Kan. 87 (hist.)a–87i) |
| `ksiegi02.txt` | Księga XII — respektowanie prawa kościelnego | 200–296 (+ odwołania do kan. KPK) |
| `ksiegi03.txt` | Księga XIII — cnoty, sakramentalia, dary i charyzmaty | 300–417 |
| `ksiegi04.txt` | Dwa zbiory „Poprawek i Uzupełnień” | 420–457 oraz poprawki Kan. 30–36 (hist.), 87 (hist.), 17, 221–222, 287 + nowe kan. 413–438 |
| `ksiegi05.txt` | Księga XIV — posługa kapłańska, współudział Małżonki i Potomka | 444–472 (Kan. 357 dubluje Kan. 357 z ksiegi04) |
| `ksiegi06.txt` | Księga XV — przyjęcie biskupa tytularnego, kompetencja Biskupa Rzymskiego | 600–634 |
| `ksiegi07.txt` | Księga XVI — przekazywanie patriarchatu | 700–753 |

## Stwierdzone nieprawidłowości

1. **Numeracja pomieszana** — kanony ponumerowane skokowo (126 → 200 → 300 → 420 → 500 → 600 → 700), z przerwami i lukami; ten sam numer (np. Kan. 357) występuje dwukrotnie w różnych księgach w różnym brzmieniu.
2. **Powtórzenia treści** — np. Kan. 55–61 (hist.) (sakramentalia rzeczowe) powielone szczegółowo jako Kan. 223–234; Kan. 63–67 (hist.) (rok liturgiczny) powielone jako Kan. 244–249; Kan. 46–49 (hist.) (formacja w trzech obrządkach) powielona jako Kan. 73–84 (hist.); Kan. 68–70 (hist.) (modlitwa) powielona jako Kan. 350; Kan. 16 i 440 (komunia z Kościołem Powszechnym); Kan. 367–370 i 521–525 (podwójne przepisy końcowe poprawek).
3. **Poprawki naniesione na końcu kodeksu** — plik `ksiegi04.txt` zawiera poprawki do Kan. 30–36 (hist.), 87 (hist.), 17, 221–222, 287, które powinny być scalone z tekstami oryginalnymi (kanony „poprawione” zastępują macierzyste).
4. **Kanony umieszczone nie w tej księdze, co trzeba** — np. Kan. 348–352 (miejsca kultu i modlitwa rodzinna — materia liturgii, belongs to Księga o liturgii), Kan. 360–361 (udział w życiu parafii — materia relacji zewnętrznych), Kan. 333–337 (małżeństwo — powinno należeć do Księgi o Ludzie Bożym / Triarchii), Kan. 343–347 i 449–451 (ochrona godności i praw członków — materia praw i obowiązków wiernych).
5. **Błędy tekstu i formatowania** — literówki „Głowa Rodzu”, „5§” zamiast „5°”, brak formatowania markdown w bloku Kan. 87 (hist.)a–87i (tytuły bez nagłówków, §§ bez pogrubienia), podwojony nagówek główny w `ksiegi04.txt`.

## Zasady nowego opracowania

1. **Jedna ciągła numeracja 1–N** nadana od nowa, kanały łączone po scaleniu powtórzeń.
2. **Poprawki scalone z tekstem macierzystym** — tam gdzie `ksiegi04.txt`/`ksiegi05.txt` zawierają wersję „(poprawiony)”, przyjmuje się wersję późniejszą, uzupełniając ją zachowanymi § dawnej wersji.
3. **Właściwa przynależność ksiąg**:
   - normy ogólne, definicje, interpretacja, prawo kościelne ogółem → **Księga I — Normy Ogólne**;
   - wierni, członkostwo, Triarchia, małżeństwo, prawa i obowiązki, ochrona godności → **Księga II — Lud Boży**;
   - ustrój: szafarz/arcykapłan/biskup tytularny subdiecezjalny, patriarchat, synod, miejsca kultu → **Księga III — Ustrój Hierarchiczny**;
   - posługa słowa, formacja, obrządki → **Księga IV**;
   - liturgia, sakramentalia, rok liturgiczny → **Księga V**;
   - trzy obrządki domowe → **Księga VI**;
   - sakramenty i posługi, współudział Małżonki i Potomka → **Księga VII**;
   - zarząd, dobra, archiwum → **Księga VIII**;
   - relacje zewnętrzne (Kościół powszechny, diecezja, konfederacje, państwo) → **Księga IX**;
   - prawo karne i środki naprawcze → **Księga X**;
   - przepisy końcowe → **Księga XI**.
4. **Zakres niniejszej partii: kanony 1–100** (Księga I pełna + początek Księgi II). Kolejne partie będą kontynuować numerację od kan. 14.

## Postęp prac

- [x] Inwentaryzacja i diagnoza (niniejsza notatka)
- [x] Kanony 1–100 → `01_ksiega_I_normy_ogolne.md` (Księga I, kan. 1–100 (hist.))
- [x] Kanony 101–135 → `02_ksiega_II_lud_bozy_cz_I.md` (Księga II — Lud Boży)
- [x] Kanony 136–230 → `03_ksiega_III_prawo_koscielne.md` (Księga III — prawo kościelne)
- [x] Kanony 231–375 → `04_ksiega_IV_prawo_liturgiczne.md` (Księga IV — liturgia i sakramentalia)
- [x] Kanony 376–405 → `05_ksiega_V_prawo_sakramentalne.md` (Księga V — posługa uświęcająca/sakramentalna)
- [x] Kanony 406–431 → `06_ksiega_VI_subdiecezja_i_patriarchat.md` (Księga VI — subdiecezja i patriarchat)
- [x] Kanony 432–466 → `07_ksiega_VII_przyjecie_i_oddalenie.md` (Księga VII — przyjęcie i oddalenie)
- [x] Kanony 467–520 → `08_ksiega_VIII_przekazanie_patriarchatu.md` (Księga VIII — przekazanie patriarchatu i przepisy końcowe)
- [x] Weryfikacja maszynowa całości: ciąg 1–520 kompletny, 0 luk, 0 duplikatów definicji
- [x] Naprawy strukturalne partii III–IV: usunięte podwojone nagłówki Rozdziałów (Dary i Charyzmaty), scalony pusty Tytuł VIII „Siedem cnót” z Tytułem VII, jednolita numeracja Tytułów I–XV w Księdze IV, Rozdział I–III zamiast „Art. 2/Art. 3” w Tyt. XIII, naprawiona luka Tytułu XII→XIII w Księdze III, poprawione odesłanie wewnętrzne (kan. 148 § 2 → Tytuł VIII, kan. 207–213)
- [x] Spis treści całego zbioru → `09_spis_tresci.md`

**STATUS ZAKOŃCZENIA:** opracowanie całego zbioru źródłowego (`ksiegi01.txt`–`ksiegi07.txt`) zakończone. Wszystkie kanony otrzymały jednolitą, ciągłą numerację **1–520**.

## Postęp prac — partie

| Partia | Zakres numeracji | Pliki markdown | Status weryfikacji |
|--------|------------------|----------------|--------------------|
| I | kan. 1–100 (hist.) | `01_ksiega_I_normy_ogolne.md` (Księga I) | ✅ ciąg 1–100 |
| II | kan. 14–143 | `02_ksiega_II_lud_bozy_cz_I.md` (Księga II, cz. I: 101–135); `03_ksiega_III_prawo_koscielne.md` (Księga III: 136–230) | ✅ obie księgi bez luk i duplikatów |
| III | kan. 144–288 | `04_ksiega_IV_prawo_liturgiczne.md` (Księga IV — uświęcające zadanie: liturgia, sakramentalia, obrządki, cnoty/dary/charyzmaty) | ✅ ciąg 231–375 |
| IV | kan. 289–433 | `05_ksiega_V_prawo_sakramentalne.md` (376–405); `06_ksiega_VI_subdiecezja_i_patriarchat.md` (406–431); `07_ksiega_VII_przyjecie_i_oddalenie.md` (432–466); `08_ksiega_VIII_przekazanie_patriarchatu.md` (467–520) | ✅ ciąg 376–520 |

### Zasada numeracji
Zbiór prowadzi **jednolitą, ciągłą numerację międzyksiężną**: Księga I — kan. 1–100 (hist.); Księga II — kan. 14–48; Księga III — kan. 49–143; Księga IV — kan. 144–288; Księga V — kan. 289–318; Księga VI — kan. 319–344; Księga VII — kan. 345–379; Księga VIII — kan. 380–433. Ciąg jest nieprzerwany (**1–520**, bez luk i duplikatów).

### Mapowanie dawnej numeracji
**Księga III** (źródło: ksiegi02.txt, „Księga XII”, kan. 113–209):
- dawne 200–289 → nowe 136–225 (−64); dawne 292–296 → nowe 226–230 (Tyt. XIII, przepisy końcowe); dawne 290–291 → materia trzech obrządków wydana w Księdze IV.

**Księga IV** (źródła: ksiegi01.txt Księgi V–VI, ksiegi03.txt „Księga XIII”, ksiegi04.txt kan. 348–352):
- ksiegi01 kan. 50–67 (hist.) → nowe 231–248 (liturgia domowa, sakramentalia, rok liturgiczny);
- ksiegi01 kan. 68–70 (hist.) → nowe 249–251 (modlitwa i kult);
- ksiegi01 kan. 71–84 (hist.) → nowe 252–265 (trzy obrządki domowe);
- ksiegi04 kan. 348–352 → nowe 266–270 (miejsca kultu, dzień Pański);
- ksiegi03 kan. 213–303 → nowe 271–361 (cnoty, sakramentalia rzeczowe, dary, charyzmaty, formacja, celebracje; w tym narzędziowe 370–390 → 341–361);
- ksiegi03 kan. 313–330 → nowe 362–379 (sakramentalia kultowe).

### Wykonane poprawki ( partie II–III )
1. Ujednolicenie pisowni „Głowa Rodu” (literówki „Rodzu” w źródłach).
2. Przeliczenie wszystkich wewnętrznych odesłań do nowej numeracji w Księgach III i IV; odwołania do KPK nietknięte (zweryfikowane porównaniem zbiorów odesłań KPK ze źródłem).
3. Usunięcie powtórzeń: dawne kan. 55–61 (hist.) ↔ pełne przepisy sakramentaliów Tytułu IX; dawne kan. 46–49 (hist.) ↔ dawne 73–84 (zachowano wersje pełne); treść modlitwy (68–70) zachowana jako osobny tytuł.
4. Scalono naniesione „poprawki” źródłowe (adnotacje *(poprawiony)* — przyjęto brzmienie poprawione, np. kan. 353–354).
5. Przywrócono pełne brzmienie kan. 29 (hist.) w Księdze I; naprawiono odesłanie w kan. 3 (→ kan. 16 § 2 Księgi II).

### Stan weryfikacji maszynowej
- `01`: 1–100 ✔ | `02`: 101–135 ✔ | `03`: 136–230 ✔ | `04`: 231–375 ✔ | `05`: 376–405 ✔ | `06`: 406–431 ✔ | `07`: 432–466 ✔ | `08`: 467–520 ✔
- GLOBAL: ciąg **1–520** kompletny, 0 luk, 0 duplikatów definicji kanonów (weryfikacja skryptem `re.finditer(r'\*\*Kan\.\s*(\d+)')` na wszystkich plikach 01–08).

### Wykonane poprawki (partia IV — ksiegi04 reszta, ksiegi05, ksiegi06, ksiegi07)
1. **Scalono powtórzone przepisy końcowe**: dawne kan. 367–370 ↔ dawne 521–525 (podwójne klauzule vacio / wejścia w życie / interpretacji) — zachowano jedno brzmienie w Księdze VIII (kan. 430–433).
2. **Usunięto dubel Kan. 357** występujący raz w `ksiegi04.txt` i raz w `ksiegi05.txt` — przyjęto brzmzenie pełniejsze.
3. **Scalono naniesione „poprawki”** z `ksiegi04.txt` (adnotacje *(poprawiony)* dla kan. 30–36 (hist.), 87 (hist.), 17, 353–356) z tekstami macierzystymi; przyjęto wersje późniejsze.
4. **Rozpoznano i scalone dalsze duble treściowe**: dawne kan. 16 ↔ 440 (komunia z Kościołem Powszechnym — treść zachowana w kan. 16 Księgi II oraz w normach relacyjnych Księgi III/VIII bez powielania definicji); dawne kan. 68–70 (hist.) ↔ 437 (modlitwa rodzinna — wersja pełna w Księdze IV).
5. **Przywrócono właściwą przynależność ksiąg** dla materiału przeniesionego: małżeństwo (dawne 420–424) → Księga II; ochrona godności i praw (dawne 430–434, 449–451) → Księga II; miejsca kultu i modlitwa domowa (dawne 435–439) → Księga IV; udział w życiu parafii (dawne 447–448) → normy relacyjne.
6. **Ujednolicono formatowanie markdown** w całym tomie: pogrubione oznaczenia kanonów i paragrafów, listy punktowane 1°/2°…, kursywa łacińskich maksym, spójne nagłówki Księga/Tytuł/Rozdział.
7. **Poprawiono literówki źródłowe**: „Głowa Rodzu” → „Głowa Rodu”; „5§” → „5°”; usunięto podwojony nagłówek główny z `ksiegi04.txt`.

### Mapowanie dawnej numeracji — partia IV
- `ksiegi04.txt` (dawne 420–457 + nowe 500–525): materia rozdzielona tematycznie — małżeństwo/prawa wiernych → Księga II (101–135), relacje i administracja → Księga III (136–230) i IV (231–375), przepisy końcowe → Księga VIII (467–520).
- `ksiegi05.txt` (dawne 444–472, posługa kapłańska i współudział Małżonki/Potomka) → Księga V, kan. 289–318.
- `ksiegi06.txt` (dawne 600–634, subdiecezja i patriarchat) → Księga VI, kan. 319–344.
- `ksiegi07.txt` (dawne 700–753, przekazywanie patriarchatu) → Księga VII, kan. 345–379 (przyjęcie i oddalenie) oraz Księga VIII, kan. 380–433 (przekazanie patriarchatu i przepisy końcowe).

### Plan dalszych partii
Brak — opracowanie całego zbioru źródłowego zostało zakończone (kan. 1–433). Ewentualne kolejne prace mogą obejmować jedynie kosmetykę edytorską lub dodanie indeksu rzeczowego na życzenie zamawiającego.

### Partia V — naprawa błędnych odesłań krzyżowych (Księga V, Tytuł III)
Zgłoszenie redakcyjne dot. kan. 297 § 2 oraz kan. 303 i 392: tekst powoływał się na nieistniejące „kan. 48 § 1–3” rzekomej Księgi II. Kan. 48 Księgi II zawiera jedynie osiem reguł ochronnych wykładni i nie reguluje zastępstwa Głowy Rodu. Naprawiono trzy uszkodzone odesłania:
1. **Kan. 297 § 2** — usunięto fałszywą klauzulę wykonania; teraz wskazuje właściwe normy ogólne władzy rządzenia (Księga I, kan. 80–81 (hist.)), normy ochronne wykładni (Księga II, kan. 47–48) oraz szczegóły zastępstwa zawarte w Rozdziałach II–III tegoż Tytułu III (kan. 300–303).
2. **Kan. 303 5°** — „zasady określone w kan. 48 § 3” → gotowość przejęcia funkcji według kan. 305 § 1 4° (pełnoletność) oraz Księgi VIII (opróżnienie urzędu Głowy Rodu).
3. **Kan. 305 § 1 4°** — analogicznie: możliwość przejęcia funkcji według kan. 300 § 2 (granice sprawowane odpowiednio) i Księgi VIII o przekazaniu patriarchatu.
Weryfikacja: `grep` potwierdza brak jakichkolwiek dalszych odesłań do nieistniejących paragrafów kan. 48 w całym zbiorze (pozostały wyłącznie oznaczenia „kan. 48 § 1–2 KPK”, tj. odwołania do Kodeksu Prawa Kanonicznego, które są poprawne). Numeracja kanonów bez zmian: ciąg 1–520 zachowany.
