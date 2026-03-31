# CLAUDE.md — Instrukcje dla Claude Code

## Projekt: Strona internetowa Micro-Serwis Grudziądz

Budujesz stronę kontaktową (docelowo wielostronicową) dla firmy **Micro-Serwis** — serwisu elektroniki użytkowej z Grudziądza. Strona musi być w **100% po polsku**, z poprawnymi polskimi znakami (ą, ć, ę, ł, ń, ó, ś, ź, ż), bez jakichkolwiek błędów ortograficznych, gramatycznych ani interpunkcyjnych.

---

## 1. Dane firmy (PRAWDZIWE — użyj dokładnie tych danych)

### Nazwa
**Micro-Serwis**

### Adres
ul. Królewska 7
86-300 Grudziądz
(obok dworca PKP, naprzeciwko postoju taksówek)

### Telefon
**667 547 632** (numer główny — wyświetlaj z prefiksem +48, tj. **+48 667 547 632**)

### Godziny otwarcia
| Dzień | Godziny |
|---|---|
| Poniedziałek | 08:00 – 16:00 |
| Wtorek | 08:00 – 16:00 |
| Środa | 08:00 – 16:00 |
| Czwartek | 08:00 – 16:00 |
| Piątek | 08:00 – 16:00 |
| Sobota | Nieczynne |
| Niedziela | Nieczynne |

### E-mail
**marcin20201@gmail.com**

### Mapa Google
Współrzędne GPS: 53.4830, 18.7618
Link do Map Google: https://maps.app.goo.gl/Rs7tMK6RUURG9itB9

### Doświadczenie
Firma działa na rynku **od ponad 10 lat**.

### Ocena Google
4,6 / 5 (ponad 170 opinii)

---

## 2. Zakres usług — OFICJALNA LISTA

Micro-Serwis specjalizuje się w naprawie i serwisie:

1. **Komputerów stacjonarnych** — diagnostyka, wymiana podzespołów, czyszczenie, modernizacja
2. **Laptopów** — naprawa płyt głównych, wymiana matryc, klawiatur, gniazd zasilania
3. **Konsol do gier** — wymiana laserów, naprawa kontrolerów/padów, diagnostyka
4. **Telewizorów** — naprawa elektroniki, wymiana podświetlenia, diagnostyka usterek
5. **Telefonów komórkowych** — wymiana wyświetlaczy, naprawa uszkodzeń mechanicznych i programowych
6. **Nawigacji GPS** — serwis i naprawa urządzeń nawigacyjnych
7. **Elektroniki użytkowej** — pozostałe urządzenia elektroniczne

### Dodatkowe atuty (z opinii klientów):
- Szybka realizacja zleceń
- Przystępne ceny
- Fachowe doradztwo
- Profesjonalna i miła obsługa
- Indywidualne podejście do klienta

---

## 3. Treści stron — TEKSTY PO POLSKU

### 3.1 Nawigacja (TopNavBar)

```
Strona główna | Usługi | O nas | Kontakt
```

W prawym rogu nawigacji: `+48 667 547 632` + ikona lokalizacji

### 3.2 Strona KONTAKT — Sekcja Hero

**Nagłówek nad tytułem (label):**
```
Lokalizacja serwisu
```

**Tytuł główny (headline):**
```
Znajdź nas
przy dworcu.
```
*(Słowo „dworcu" powinno być wyróżnione kolorem primary)*

**Tekst wspierający (opis po prawej):**
```
Nasz serwis elektroniki mieści się w samym centrum Grudziądza, tuż obok dworca PKP — łatwy dojazd i wygodna lokalizacja dla każdego klienta.
```

### 3.3 Karta „Dane lokalizacji" (Location Details)

**Tytuł:** `Jak do nas trafić`

**Adres:**
```
ul. Królewska 7
86-300 Grudziądz
```

**Punkt orientacyjny 1 — Postój taksówek:**
- Ikona: `local_taxi`
- Tytuł: `Postój taksówek`
- Opis: `Znajduje się bezpośrednio naprzeciwko naszego wejścia.`

**Punkt orientacyjny 2 — Dworzec PKP:**
- Ikona: `train`
- Tytuł: `Dworzec PKP`
- Opis: `Zaledwie 2 minuty spacerem od wyjścia z dworca.`

### 3.4 Mapa

Użyj osadzonej mapy Google Maps (`<iframe>`) wskazującej na ul. Królewską 7, 86-300 Grudziądz.

Nakładka (overlay) w prawym dolnym rogu:
```
Micro-Serwis
Wejście do serwisu
```

### 3.5 Karta „Dane kontaktowe" (Contact Details)

**Kolumna 1 — Telefon:**
- Nagłówek: `Zadzwoń do nas`
- Ikona: `call`
- Numer: `+48 667 547 632`
- Opis: `Dzwoń w godzinach pracy serwisu — chętnie odpowiemy na pytania dotyczące naprawy.`

**Kolumna 2 — E-mail:**
- Nagłówek: `Napisz do nas`
- Ikona: `mail`
- Adres: `marci20201@gmail.com`
- Opis: `Opisz usterkę — odpiszemy z wstępną wyceną najszybciej jak to możliwe.`

### 3.6 Karta „Godziny otwarcia" (na niebieskim tle)

**Nagłówek:** `Godziny otwarcia`

```
Poniedziałek — Piątek       08:00 — 16:00
Sobota                       Nieczynne
Niedziela                    Nieczynne
```

### 3.7 Formularz zgłoszeniowy (Repair Inquiry Form)

**Tytuł:**
```
Wyślij zgłoszenie serwisowe.
```
*(Słowa „zgłoszenie serwisowe" w kolorze primary)*

**Tekst pod tytułem:**
```
Opisz problem ze swoim urządzeniem. Nasi technicy zapoznają się ze zgłoszeniem i przygotują wstępną diagnozę jeszcze przed Twoją wizytą.
```

**Pola formularza:**
| Pole | Etykieta | Placeholder |
|---|---|---|
| Imię i nazwisko | `Imię i nazwisko` | `Jan Kowalski` |
| E-mail | `Adres e-mail` | `jan@przyklad.pl` |
| Textarea | `Urządzenie i opis usterki` | `Opisz model urządzenia i objawy usterki…` |

**Przycisk:**
```
Wyślij zgłoszenie
```

### 3.8 Stopka (Footer)

**Kolumna 1 — Logo i opis:**
```
Micro-Serwis
Profesjonalny serwis elektroniki użytkowej w Grudziądzu. Naprawiamy komputery, laptopy, konsole, telewizory i telefony od ponad 10 lat.
```

**Kolumna 2 — Nawigacja:**
- Nagłówek: `Nawigacja`
- Linki: Strona główna, Usługi, O nas

**Kolumna 3 — Informacje prawne:**
- Nagłówek: `Informacje prawne`
- Linki: Polityka prywatności, Regulamin

**Kolumna 4 — Media społecznościowe:**
- Nagłówek: `Znajdź nas`
- Linki: Facebook, Instagram *(jeśli istnieją — w przeciwnym razie oznacz `<!-- TODO: uzupełnić linki do social media -->`)*

**Pasek dolny (copyright):**
```
© 2026 Micro-Serwis. Serwis elektroniki użytkowej — Grudziądz.```

---

## 4. Treści na stronę STRONA GŁÓWNA (Home) — do przyszłego użycia

### Hero
**Label:** `Serwis elektroniki w Grudziądzu`
**Headline:**
```
Naprawiamy to,
na czym Ci zależy.
```
**Opis:**
```
Komputery, laptopy, konsole, telewizory, telefony — profesjonalna diagnoza i naprawa w centrum Grudziądza. Szybko, fachowo i w przystępnej cenie.
```
**CTA:** `Umów wizytę` / `Sprawdź usługi`

### Sekcja „Dlaczego my"
1. **Ponad 10 lat doświadczenia** — Setki naprawionych urządzeń i zadowolonych klientów z Grudziądza i okolic.
2. **Szybka realizacja** — Większość napraw wykonujemy w ciągu 1–3 dni roboczych.
3. **Uczciwe ceny** — Wycena przed naprawą, bez ukrytych kosztów.
4. **Szeroki zakres usług** — Od wymiany matrycy w laptopie po naprawę konsoli do gier.

### Sekcja „Nasze usługi"
| Usługa | Ikona (Material Symbols) | Krótki opis |
|---|---|---|
| Komputery stacjonarne | `desktop_windows` | Diagnostyka, wymiana podzespołów, modernizacja i czyszczenie. |
| Laptopy | `laptop_mac` | Naprawa płyt głównych, wymiana matryc, klawiatur i gniazd ładowania. |
| Konsole do gier | `sports_esports` | Wymiana laserów, naprawa padów, diagnostyka i serwis konsol. |
| Telewizory | `tv` | Naprawa elektroniki, wymiana podświetlenia LED, diagnostyka. |
| Telefony | `smartphone` | Wymiana wyświetlaczy, naprawa usterek programowych i mechanicznych. |
| Nawigacje GPS | `explore` | Serwis i naprawa urządzeń nawigacyjnych. |

### Sekcja „Zaufali nam"
```
Ponad 170 opinii w Google — ocena 4,6 / 5
```
Tekst: `Nasi klienci doceniają profesjonalizm, szybkość i uczciwość. Sprawdź opinie na Google Maps.`

---

## 5. Treści na stronę USŁUGI (Services) — do przyszłego użycia

### Nagłówek
**Label:** `Zakres usług`
**Headline:**
```
Naprawiamy każdy sprzęt elektroniczny.
```
**Opis:**
```
Od drobnych usterek po poważne awarie — dysponujemy wiedzą i narzędziami, by przywrócić Twoje urządzenie do pełnej sprawności.
```

### Karty usług (rozwinięte opisy)

**Naprawa komputerów stacjonarnych:**
```
Twój komputer wolno działa, nie uruchamia się lub wyłącza bez ostrzeżenia? Diagnozujemy problem i dobieramy optymalne rozwiązanie — od wymiany pasty termoprzewodzącej, przez instalację nowego dysku SSD, po kompleksową modernizację podzespołów.
```

**Naprawa laptopów:**
```
Pęknięta matryca, zepsuta klawiatura, luźne gniazdo ładowania? Specjalizujemy się w naprawach laptopów wszystkich marek. Wymieniamy ekrany, klawiatury, baterie i naprawiamy płyty główne.
```

**Naprawa konsol do gier:**
```
PlayStation, Xbox, Nintendo — serwisujemy wszystkie popularne konsole. Wymieniamy lasery, naprawiamy kontrolery i rozwiązujemy problemy z oprogramowaniem.
```

**Naprawa telewizorów:**
```
Brak obrazu, paski na ekranie, uszkodzone podświetlenie? Diagnozujemy i naprawiamy telewizory LED, LCD i Smart TV.
```

**Naprawa telefonów komórkowych:**
```
Zbity ekran, niedziałający dotyk, problemy z baterią? Wymieniamy wyświetlacze, naprawiamy usterki programowe i przywracamy sprawność Twojego telefonu.
```

**Naprawa nawigacji GPS:**
```
Problemy z sygnałem, uszkodzony ekran dotykowy, błędy oprogramowania? Serwisujemy urządzenia nawigacyjne i przywracamy im pełną funkcjonalność.
```

### CTA na dole
```
Masz problem z urządzeniem? Zadzwoń: +48 667 547 632 lub wyślij zgłoszenie online.
```

---

## 6. Treści na stronę O NAS (About) — do przyszłego użycia

### Nagłówek
**Label:** `O firmie`
**Headline:**
```
Ponad dekada w służbie elektroniki.
```

**Tekst główny:**
```
Micro-Serwis to firma serwisowa z Grudziądza, działająca na rynku od ponad 10 lat. Nasz punkt mieści się przy ul. Królewskiej 7, tuż obok dworca PKP — w samym sercu miasta.

Specjalizujemy się w naprawie komputerów, laptopów, konsol do gier, telewizorów, telefonów komórkowych i nawigacji GPS. Na przestrzeni lat zdobyliśmy zaufanie setek klientów, co potwierdzają liczne pozytywne opinie w Google.

Stawiamy na uczciwość, szybkość i fachowość. Każde urządzenie traktujemy indywidualnie — diagnozujemy problem, przedstawiamy wycenę i dopiero po akceptacji przystępujemy do naprawy. Bez niespodzianek, bez ukrytych kosztów.
```

### Wartości
1. **Uczciwość** — Wycena przed naprawą. Płacisz tylko za wykonaną usługę.
2. **Fachowość** — Ponad 10 lat doświadczenia i setki udanych napraw.
3. **Szybkość** — Większość zleceń realizujemy w 1–3 dni robocze.

---

## 7. DESIGN SYSTEM — BEZWZGLĘDNE REGUŁY

> **UWAGA: Szata graficzna została zaprojektowana w Stitch i znajduje się w pliku `DESIGN.md`. Poniższe reguły są OBOWIĄZKOWE.**

### 7.1 Plik referencyjny
Wczytaj i ściśle przestrzegaj wszystkich zasad z pliku `DESIGN.md`. Główne reguły:

### 7.2 Kolory — tokeny z Tailwind config
Używaj WYŁĄCZNIE tokenów zdefiniowanych w konfiguracji Tailwind (patrz `code.html`). Kluczowe tokeny:

- **Primary:** `#006097` — akcje, linki, wyróżnienia
- **Primary Container:** `#007abe` — tła przycisków CTA, gradienty
- **Background:** `#f9f9f9` — tło bazowe strony
- **Surface Container Low:** `#f3f3f3` — duże sekcje strukturalne
- **Surface Container Lowest:** `#ffffff` — karty na pierwszym planie
- **Surface Container Highest:** `#e2e2e2` — tła pól formularzy
- **On Surface:** `#1a1c1c` — tekst główny
- **On Surface Variant:** `#3f4851` — tekst pomocniczy, opisy

### 7.3 Zasada „Bez linii"
**ZABRANIA SIĘ** stosowania ramek `border` 1px solid do dzielenia sekcji. Granice definiuj WYŁĄCZNIE przez zmianę koloru tła (`surface` → `surface-container-low`).

### 7.4 Glassmorphism i gradienty
- Przyciski CTA: gradient od `primary` do `primary-container`
- Pływające elementy: `backdrop-filter: blur(20px)` + półprzezroczyste tło
- Nawigacja: efekt frosted glass (`bg-white/80 backdrop-blur-xl`)

### 7.5 Typografia
- **Nagłówki (Display, Headline):** `Space Grotesk` — `font-headline`
- **Tekst (Body, Label):** `Inter` — `font-body`, `font-label`
- Obie czcionki obsługują polskie znaki diakrytyczne (ą, ć, ę, ł, ń, ó, ś, ź, ż)
- Import z Google Fonts: `family=Space+Grotesk:wght@300;400;500;600;700&family=Inter:wght@300;400;500;600;700`
- Nagłówki: duży kontrast skalą — `text-5xl md:text-7xl` dla hero, z `tracking-tighter`
- Etykiety: `text-xs font-bold uppercase tracking-widest`

### 7.6 Elevation — Warstwa tonalna
- **Karty:** ZERO cieni typu box-shadow. Buduj hierarchię poprzez zagnieżdżanie `surface-container-lowest` wewnątrz `surface-container-low`.
- **Jedyny dozwolony cień:** na efektach glassmorphism — rozproszony, `on-surface` 6% opacity, blur 40px, Y-offset 12px.
- **Ghost Border:** jeśli potrzebny — `outline-variant` na 15% opacity. NIGDY 100%.

### 7.7 Zaokrąglenia
- Domyślne: `rounded` (0.125rem)
- Duże: `rounded-lg` (0.25rem)
- Większe: `rounded-xl` (0.5rem)
- Pełne: `rounded-full` (0.75rem)
- Karty i sekcje: `rounded-xl`

### 7.8 Ikony
- Biblioteka: **Material Symbols Outlined**
- Import: `fonts.googleapis.com/css2?family=Material+Symbols+Outlined:wght,FILL@100..700,0..1`
- Styl: cienkie linie, spójny rozmiar, kolor `primary` lub `outline`
- Każda ikona musi mieć sens funkcjonalny — nie używaj ikon dekoracyjnych

### 7.9 Odstępy
- Między głównymi sekcjami: `mb-20` (spacing-20)
- Wewnątrz kart: `p-8` lub `p-12`
- Między elementami w kartach: `space-y-4` do `space-y-8`
- Grid gap: `gap-6`

---

## 8. REGUŁY IMPLEMENTACJI

### 8.1 Język
- **CAŁA** zawartość strony (teksty, labele, placeholdery, atrybuty `alt`, komentarze HTML widoczne dla użytkownika) — PO POLSKU
- Kod (klasy CSS, nazwy zmiennych) — po angielsku (standard)
- `<html lang="pl">`
- `<meta charset="utf-8">`

### 8.2 Czcionki
- ZAWSZE importuj Space Grotesk i Inter z Google Fonts
- Upewnij się, że import zawiera odpowiednie wagi: 300, 400, 500, 600, 700
- Testuj polskie znaki: „Łódź", „Grudziądz", „naprzeciwko", „zgłoszenie"

### 8.3 Responsywność
- Mobile-first z breakpointami Tailwind (`md:`, `lg:`)
- Nawigacja: hamburger menu na mobile, inline na desktop
- Grid: `grid-cols-1` → `md:grid-cols-12`
- Formularz: `grid-cols-1 sm:grid-cols-2` dla pól w rzędzie

### 8.4 Struktura plików
```
/
├── index.html          ← Strona główna
├── kontakt.html        ← Strona kontaktowa (priorytet — buduj JAKO PIERWSZĄ)
├── uslugi.html         ← Strona usług
├── o-nas.html          ← O firmie
├── DESIGN.md           ← System designu (nie modyfikuj)
├── CLAUDE.md           ← Ten plik (nie modyfikuj)
└── assets/
    └── images/         ← Zdjęcia i grafiki (obsługuje Stitch)
```

### 8.5 Mapa Google — iframe embed
Na stronie kontaktowej osadź mapę Google Maps:
```html
<iframe
  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2398.5!2d18.7618!3d53.4830!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNTPCsDI4JzU5LjAiTiAxOMKwNDUnNDIuNSJF!5e0!3m2!1spl!2spl!4v1"
  width="100%"
  height="100%"
  style="border:0;"
  allowfullscreen=""
  loading="lazy"
  referrerpolicy="no-referrer-when-downgrade"
  title="Mapa — Micro-Serwis, ul. Królewska 7, Grudziądz">
</iframe>
```
*(Może wymagać aktualizacji embed URL — użyj współrzędnych 53.4830, 18.7618)*

### 8.6 Link telefoniczny
Numer telefonu powinien być klikalny:
```html
<a href="tel:+48667547632">+48 667 547 632</a>
```

### 8.7 SEO — Meta tagi
```html
<title>Micro-Serwis — Serwis komputerów, laptopów i elektroniki | Grudziądz</title>
<meta name="description" content="Profesjonalny serwis elektroniki użytkowej w Grudziądzu. Naprawiamy komputery, laptopy, konsole, telewizory i telefony. ul. Królewska 7, obok dworca PKP.">
<meta name="keywords" content="serwis komputerowy Grudziądz, naprawa laptopów, naprawa telefonów, serwis konsol, naprawa telewizorów, Micro-Serwis">
```

### 8.8 Grafiki i zdjęcia
**ABSOLUTNIE NIE generuj żadnych grafik, obrazków, SVG ilustracji ani ikon dekoracyjnych.** Grafiką zajmuje się wyłącznie Stitch. W miejscach na zdjęcia:
- Użyj placeholderów z kolorami systemu (`bg-surface-container-high`) o takich samych proporcjach jak w pliku referencyjnym `code.html`
- Dodaj opisowe atrybuty `alt` po polsku
- Oznacz komentarzem: `<!-- STITCH: tu wstaw zdjęcie [opis] -->`
- **NIE** wstawiaj losowych obrazków z internetu, unsplash, placeholder.com itp.
- **NIE** twórz grafik generatywnych (SVG, canvas, ASCII art)
- Wszystkie elementy wizualne (układ, kolory, proporcje kart, grid) wzoruj ŚCIŚLE na designie z plików projektu: `code.html` (kod referencyjny), `screen.png` (screenshot szaty graficznej) i `DESIGN.md` (system designu)

---

## 9. WZORZEC KODU — Strona kontaktowa

Wzoruj się na strukturze z pliku `code.html`. Kluczowe elementy do zachowania:
- Sticky nawigacja z efektem glassmorphism
- Bento grid layout dla kart z informacjami
- Karta adresowa (4 kolumny) + mapa (8 kolumn)
- Karta kontaktowa (6 kolumn) + godziny otwarcia (6 kolumn)
- Formularz z obrazem obok (grid 2-kolumnowy na desktop)
- Footer 4-kolumnowy

**ZACHOWAJ** dokładnie tę samą strukturę grid i proporcje jak w `code.html`, ale ZAMIEŃ:
1. Wszystkie teksty angielskie → polskie (z tego dokumentu)
2. Numer telefonu → `+48 667 547 632`
3. Adres → `ul. Królewska 7, 86-300 Grudziądz`
4. Godziny → poniedziałek–piątek 08:00–16:00, sobota–niedziela nieczynne
5. E-mail → `marci20201@gmail.com`
6. Nazwy przycisków, etykiet, placeholderów → polskie
7. Miasto z „Warszawa" → „Grudziądz"
8. Tekst copyright: `© 2026 Micro-Serwis. Serwis elektroniki użytkowej — Grudziądz.`

---

## 10. CHECKLISTA PRZED ODDANIEM

> Wszystkie poniższe punkty wynikają z systemu designu dostarczonego w plikach projektu (`DESIGN.md`, `code.html`, `screen.png`). Traktuj te pliki jako jedyne źródło prawdy wizualnej.

- [ ] Wszystkie teksty po polsku — żadnych angielskich napisów w UI
- [ ] Polskie znaki diakrytyczne wyświetlają się poprawnie
- [ ] Numer telefonu: +48 667 547 632 (klikalny `tel:`)
- [ ] E-mail: marci20201@gmail.com (klikalny `mailto:`)
- [ ] Adres: ul. Królewska 7, 86-300 Grudziądz
- [ ] Godziny: pon.–pt. 08:00–16:00, sob.–niedz. nieczynne
- [ ] Mapa Google osadzona i wskazuje właściwy adres
- [ ] Brak ramek 1px solid (zasada „Bez linii" z DESIGN.md)
- [ ] Gradient na przyciskach CTA (primary → primary-container) — jak w `code.html`
- [ ] Glassmorphism na nawigacji i pływających elementach — jak w `code.html`
- [ ] Space Grotesk na nagłówkach, Inter na body — jak w Tailwind config z `code.html`
- [ ] Responsywność — poprawne wyświetlanie na mobile
- [ ] Poprawne meta tagi SEO po polsku
- [ ] `<html lang="pl">` i `<meta charset="utf-8">`
- [ ] Placeholdery na zdjęcia oznaczone komentarzami `<!-- STITCH -->` — żadnych wygenerowanych grafik
- [ ] Układ grid, proporcje kart i sekcji identyczne jak w `screen.png` / `code.html`
- [ ] Copyright: © 2026
- [ ] Brak literówek — przeczytaj każdy tekst jeszcze raz
