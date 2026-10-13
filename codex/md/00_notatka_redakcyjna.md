# Notatka redakcyjna — porządkowanie Codex Iuris Canonici Ecclesiae Domesticae

## Stan wyjściowy (pliki źródłowe .txt)

| Plik | Zawartość | Numeracja kanonów |
|------|-----------|-------------------|
| `ksiegi01.txt` | Księgi I–XI (Kanon zasadniczy) + Aneksy | 1–126 (z wklejonym blokiem Kan. 87a–87i) |
| `ksiegi02.txt` | Księga XII — respektowanie prawa kościelnego | 200–296 (+ odwołania do kan. KPK) |
| `ksiegi03.txt` | Księga XIII — cnoty, sakramentalia, dary i charyzmaty | 300–417 |
| `ksiegi04.txt` | Dwa zbiory „Poprawek i Uzupełnień” | 420–457 oraz poprawki Kan. 30–36, 87, 104, 308–309, 374 + nowe kan. 500–525 |
| `ksiegi05.txt` | Księga XIV — posługa kapłańska, współudział Małżonki i Potomka | 444–472 (Kan. 444 dubluje Kan. 444 z ksiegi04) |
| `ksiegi06.txt` | Księga XV — przyjęcie biskupa tytularnego, kompetencja Biskupa Rzymskiego | 600–634 |
| `ksiegi07.txt` | Księga XVI — przekazywanie patriarchatu | 700–753 |

## Stwierdzone nieprawidłowości

1. **Numeracja pomieszana** — kanony ponumerowane skokowo (126 → 200 → 300 → 420 → 500 → 600 → 700), z przerwami i lukami; ten sam numer (np. Kan. 444) występuje dwukrotnie w różnych księgach w różnym brzmieniu.
2. **Powtórzenia treści** — np. Kan. 55–61 (sakramentalia rzeczowe) powielone szczegółowo jako Kan. 310–321; Kan. 63–67 (rok liturgiczny) powielone jako Kan. 331–336; Kan. 46–49 (formacja w trzech obrządkach) powielona jako Kan. 73–84; Kan. 68–70 (modlitwa) powielona jako Kan. 437; Kan. 103 i 440 (komunia z Kościołem Powszechnym); Kan. 454–457 i 521–525 (podwójne przepisy końcowe poprawek).
3. **Poprawki naniesione na końcu kodeksu** — plik `ksiegi04.txt` zawiera poprawki do Kan. 30–36, 87, 104, 308–309, 374, które powinny być scalone z tekstami oryginalnymi (kanony „poprawione” zastępują macierzyste).
4. **Kanony umieszczone nie w tej księdze, co trzeba** — np. Kan. 435–439 (miejsca kultu i modlitwa rodzinna — materia liturgii, belongs to Księga o liturgii), Kan. 447–448 (udział w życiu parafii — materia relacji zewnętrznych), Kan. 420–424 (małżeństwo — powinno należeć do Księgi o Ludzie Bożym / Triarchii), Kan. 430–434 i 449–451 (ochrona godności i praw członków — materia praw i obowiązków wiernych).
5. **Błędy tekstu i formatowania** — literówki „Głowa Rodzu”, „5§” zamiast „5°”, brak formatowania markdown w bloku Kan. 87a–87i (tytuły bez nagłówków, §§ bez pogrubienia), podwojony nagówek główny w `ksiegi04.txt`.

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
4. **Zakres niniejszej partii: kanony 1–100** (Księga I pełna + początek Księgi II). Kolejne partie będą kontynuować numerację od kan. 101.

## Postęp prac

- [x] Inwentaryzacja i diagnoza (niniejsza notatka)
- [x] Kanony 1–100 → `01_ksiega_I_normy_ogolne.md` (Księga I, kan. 1–100)
- [x] Nadto wstęp do Księgi II → `02_ksiega_II_lud_bozy_cz_I.md` (kan. 101–137; kontynuacja od kan. 138 w następnej partii)
- [ ] Kanony 101+ → kolejne partie

## Postęp prac — partie

| Partia | Zakres numeracji | Pliki markdown | Status weryfikacji |
|--------|------------------|----------------|--------------------|
| I | kan. 1–100 | `01_ksiega_I_normy_ogolne.md` (Księga I) | ✅ ciąg 1–100 |
| II | kan. 101–230 | `02_ksiega_II_lud_bozy_cz_I.md` (Księga II, cz. I: 101–135); `03_ksiega_III_prawo_koscielne.md` (Księga III: 136–230) | ✅ obie księgi bez luk i duplikatów |
| III | kan. 231–379 | `04_ksiega_IV_prawo_liturgiczne.md` (Księga IV — uświęcające zadanie: liturgia, sakramentalia, obrządki, cnoty/dary/charyzmaty) | ✅ ciąg 231–379 |

### Zasada numeracji
Zbiór prowadzi **jednolitą, ciągłą numerację międzyksiężną**: Księga I — kan. 1–100; Księga II (cz. I) — kan. 101–135; Księga III — kan. 136–230; Księga IV — kan. 231–379. Ciąg jest nieprzerwany (1–379, bez luk i duplikatów).

### Mapowanie dawnej numeracji
**Księga III** (źródło: ksiegi02.txt, „Księga XII”, kan. 200–296):
- dawne 200–289 → nowe 136–225 (−64); dawne 292–296 → nowe 226–230 (Tyt. XIII, przepisy końcowe); dawne 290–291 → materia trzech obrządków wydana w Księdze IV.

**Księga IV** (źródła: ksiegi01.txt Księgi V–VI, ksiegi03.txt „Księga XIII”, ksiegi04.txt kan. 435–439):
- ksiegi01 kan. 50–67 → nowe 231–248 (liturgia domowa, sakramentalia, rok liturgiczny);
- ksiegi01 kan. 68–70 → nowe 249–251 (modlitwa i kult);
- ksiegi01 kan. 71–84 → nowe 252–265 (trzy obrządki domowe);
- ksiegi04 kan. 435–439 → nowe 266–270 (miejsca kultu, dzień Pański);
- ksiegi03 kan. 300–390 → nowe 271–361 (cnoty, sakramentalia rzeczowe, dary, charyzmaty, formacja, celebracje; w tym narzędziowe 370–390 → 341–361);
- ksiegi03 kan. 400–417 → nowe 362–379 (sakramentalia kultowe).

### Wykonane poprawki ( partie II–III )
1. Ujednolicenie pisowni „Głowa Rodu” (literówki „Rodzu” w źródłach).
2. Przeliczenie wszystkich wewnętrznych odesłań do nowej numeracji w Księgach III i IV; odwołania do KPK nietknięte (zweryfikowane porównaniem zbiorów odesłań KPK ze źródłem).
3. Usunięcie powtórzeń: dawne kan. 55–61 ↔ pełne przepisy sakramentaliów Tytułu IX; dawne kan. 46–49 ↔ dawne 73–84 (zachowano wersje pełne); treść modlitwy (68–70) zachowana jako osobny tytuł.
4. Scalono naniesione „poprawki” źródłowe (adnotacje *(poprawiony)* — przyjęto brzmienie poprawione, np. kan. 440–441).
5. Przywrócono pełne brzmienie kan. 29 w Księdze I; naprawiono odesłanie w kan. 3 (→ kan. 103 § 2 Księgi II).

### Stan weryfikacji maszynowej
- `01`: 1–100 ✔ | `02`: 101–135 ✔ | `03`: 136–230 ✔ | `04`: 231–379 ✔ | GLOBAL: ciąg 1–379 kompletny, 0 luk, 0 duplikatów.

### Plan dalszych partii
Partia IV (kontynuacja od **kan. 380**): na podstawie `ksiegi04.txt` (pozostałe: relacje zewnętrzne, prawo karne, środki naprawcze, administracja, archiwum), `ksiegi05.txt`, `ksiegi06.txt`, `ksiegi07.txt` — z jednoczesnym scaleniem poprawek (m.in. Kan. 68–70 ↔ 437 sprawdzone przy Księgach I/IV; 103 ↔ 440; 454–457 ↔ 521–525) i wykryciem kolejnych powtórzeń.
