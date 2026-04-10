# Analiza strony SPMPZ (brooda/SPMPZ)

Data analizy: 2026-03-25
Repo: https://github.com/brooda/SPMPZ
Live: https://brooda.github.io/SPMPZ/

---

## 1. Czym jest ta strona

Strona internetowa **Stowarzyszenia Przyjaciol Miast Partnerskich Zamoscia** (SPMPZ) -- organizacji pozarzadowej z Zamoscia (KRS: 0000158936, rok powstania: 2003).

Misja stowarzyszenia: utrzymywanie kontaktow z miastami partnerskimi, nauka jezyka, wymiana mieszkancow, promowanie Zamoscia za granica, promowanie kultury i integracja europejska.

Glowne projekty:
- **Youth For Europe** -- spotkania mlodziezy z 8 miast europejskich (Francja, Niemcy, Hiszpania, Belgia, Wlochy, Wegry, Anglia, Polska)
- **Migration Project** -- projekt o migracji z partnerami z grupy "7 Cities"
- **Wspolpraca z Loughborough** (Anglia) -- coroczna wymiana mieszkancow
- **Weaving a Europe of Solidarity**
- **ImagE50** -- zakonczony projekt (raport z 2022)

Kontakt: kontakt@spmpz.zamosc.pl
Strona dwujezyczna: polski + angielski

---

## 2. Stack technologiczny

### Framework / Generator
- **Jekyll** -- statyczny generator stron (potwierdzony przez `_config.yml`, `_layouts/`, `_includes/`)
- Hosting: **GitHub Pages** (branch `master`, https://brooda.github.io/SPMPZ/)

### HTML Template
- **"Linear" by TEMPLATED** (templated.co) -- darmowy szablon HTML (licencja CC Attribution 3.0)
- Szablon pochodzi z ok. 2013-2014 roku

### CSS
- **Skel.js** framework (przestarzaly, projekt martwy od 2017)
  - `skel.min.js` -- responsywny grid framework
  - `skel-panels.min.js` -- panele mobilne
- Breakpointy: mobile (<480px), desktop (481+), 1000px (481-1200)
- **FontAwesome 4.0.1** (lokalne fonty) -- przestarzale, aktualna wersja to 6.x
- **Google Fonts: Roboto** -- ladowane przez HTTP (nie HTTPS!)
- Wlasne CSS: `style.css`, `style-desktop.css`, `style-mobile.css`, `style-1000px.css`, `skel-noscript.css`

### JavaScript
- **jQuery 1.11.0** (z Google CDN, HTTP) -- ekstremalnie przestarzale (aktualna: 3.7.x)
- `skel.min.js` + `skel-panels.min.js` -- martwy framework
- `init.js` -- konfiguracja Skel

### Serwer
- `.htaccess` wskazuje na PHP 5.5 (`AddHandler application/x-httpd-php55`) -- PHP 5.5 jest EOL od 2016 roku
- Prawdopodobnie kiedys strona byla hostowana na serwerze z PHP, teraz na GitHub Pages

### Jekyll Config
```yaml
title: Stowarzyszenie Przyjaciol Miast Partnerskich Zamoscia
email: your-email@domain.com  # <-- NIE ZMIENIONY z domyslnego!
markdown: kramdown
```

---

## 3. Struktura strony

```
/
├── _config.yml          # Jekyll config (minimalny)
├── _includes/
│   ├── head.html        # <head> (bez jQuery -- niedostepny na subpages z layout)
│   ├── header.html      # <head> z <title>
│   ├── footer.html      # Footer (Jekyll default, nieuzywany)
│   ├── footer_pl.html   # Footer polski (uzyty w layoutach)
│   ├── menu_pl.html     # Nawigacja polska
│   ├── about_pl.html
│   ├── projects_pl.html
│   ├── license.html
│   ├── icon-github.html/svg
│   └── icon-twitter.html/svg
├── _layouts/
│   ├── main.html        # Glowny layout (strona glowna)
│   └── subpage.html     # Layout podstron
├── css/
│   ├── style.css        # Glowny CSS
│   ├── style-desktop.css
│   ├── style-mobile.css
│   ├── style-1000px.css
│   ├── skel-noscript.css
│   ├── font/            # FontAwesome 4.0.1
│   └── images/          # Obrazki CSS
├── js/
│   ├── init.js          # Konfiguracja Skel
│   ├── skel.min.js
│   └── skel-panels.min.js
├── images/              # Zdjecia (JPG, PNG, GIF)
├── index.html           # Strona glowna PL (HARDCODED, nie uzywa layout!)
├── about_pl.html        # O nas (HARDCODED)
├── projects_pl.html     # Projekty (HARDCODED)
├── projects_history_pl.html
├── partners_pl.html     # Partnerzy
├── contact_pl.html      # Kontakt (HARDCODED)
├── migration_project_pl.html
├── english.html         # Strona glowna EN
├── index_en.html / index_enn.html  # Duplikaty EN?
├── about_en.html
├── projects_en.html
├── partners_en.html
├── contact_en.html
├── weaving.html
├── statute_pl.pdf       # Statut stowarzyszenia
├── migration.pdf
├── migration_first_version.pdf
├── report_22/report.pdf # Raport ImagE50
├── en/index.html
├── .htaccess            # PHP 5.5 handler (relikt)
└── Final report/        # Folder z raportem
```

---

## 4. Jak zarzadzana jest tresc

**Odpowiedz: prawie wcale nie jest zarzadzana.**

- Wiekszosc stron to **hardcoded HTML** -- nie korzysta nawet z layoutow Jekyll
- Nawigacja jest **kopiowana recznie** do kazdego pliku HTML (nie uzywa `_includes/menu_pl.html` na wiekszosci stron)
- Brak katalogu `_posts/` -- Jekyll nie jest uzywany jako blog
- Brak front matter na wiekszosci stron (brak `---` YAML header)
- Layouty Jekyll (`main.html`, `subpage.html`) istnieja, ale **wieksznosc stron ich nie uzywa**
- Dodanie nowej tresci wymaga: edycji HTML, commit do repo, push na GitHub
- Brak CMS, brak panelu administracyjnego, brak mozliwosci edycji przez nie-technicznych uzytkownikow

---

## 5. Stan i jakosc kodu

### Problemy krytyczne
1. **HTTP zamiast HTTPS** -- Google Fonts i jQuery ladowane przez `http://` (blokowane przez przegladarki na stronach HTTPS)
2. **jQuery 1.11.0** -- wydane w 2014, zawiera znane luki bezpieczenstwa
3. **FontAwesome 4.0.1** -- z 2013 roku
4. **Skel.js** -- martwy projekt, bez wsparcia od 2017
5. **PHP 5.5 w .htaccess** -- EOL od lipca 2016
6. **email w config niezmieniony**: `your-email@domain.com`

### Problemy architektoniczne
1. **Brak DRY** -- nawigacja, head, footer kopiowane do kazdego pliku zamiast korzystac z Jekyll includes
2. **Mieszanie podejsc** -- niektorzy pliki uzywaja Jekyll layouts, inne maja caly HTML hardcoded
3. **Duplikaty stron** -- `index_en.html`, `index_enn.html`, `english.html` -- niejasne co jest aktywne
4. **Brak responsywnosci** -- opiera sie na przestarzalym Skel.js
5. **Hack z opacity** -- `body {opacity:0}` + JavaScript timeout do "ladowania" -- hack ktory moze powodowac FOUC
6. **Brak meta viewport** -- problemy na mobilnych
7. **Brak SEO** -- brak meta description, og tags, sitemap, robots.txt

### Pozytywne aspekty
- Strona jest prosta i lekka (malo JS, malo CSS)
- Hosting na GitHub Pages = darmowy, niezawodny
- Dwujezycznosc (PL/EN) jest zaimplementowana (choc prymitywnie)
- Tresc jest sensowna i kompletna

---

## 6. Historia aktualizacji

| Data | Commit |
|------|--------|
| 2017-12-30 | Initial Jekyll |
| 2017-12-31 | Polish finished, CNAME setup/delete |
| 2020-10-17 | Create README.md |
| 2022-12-17 | Report ImagE50 (ostatni commit) |

**Ostatnia aktualizacja: grudzien 2022 (ponad 3 lata temu)**
Strona jest praktycznie nieaktywna od lat.

---

## 7. Analiza opcji dodania systemu zarzadzania trescia (CMS)

### Cel: umozliwic innym uzytkownikom (nie-technicznym) dodawanie artykulow/tresci

### Opcja A: DecapCMS (dawniej Netlify CMS) -- REKOMENDOWANE

**Opis:** Git-based CMS z interfejsem webowym, dziala bezposrednio z GitHub Pages + Jekyll.

**Zalety:**
- Nie wymaga backendu ani bazy danych
- Pozostaje na GitHub Pages (darmowy hosting)
- Edytor WYSIWYG w przegladarce
- Autentykacja przez GitHub OAuth lub Netlify Identity
- Tresci zapisywane jako pliki Markdown w repo
- Minimalne zmiany w istniejacym projekcie (dodanie `admin/` folderu)

**Wady:**
- Uzytkownicy potrzebuja konta GitHub (lub Netlify Identity)
- Ograniczone mozliwosci customizacji edytora
- Brak zaawansowanych ról uzytkownikow

**Naklad pracy:** MALY (1-2 dni)
- Dodac folder `admin/` z `index.html` i `config.yml`
- Skonfigurowac kolekcje (artykuly, projekty)
- Przebudowac strony na Markdown + Jekyll layouts (obecnie hardcoded)
- Dodac OAuth backend (Netlify Identity widget lub GitHub OAuth proxy)

**Szacunkowy czas calkowity (z refactorem Jekyll):** 3-5 dni

---

### Opcja B: Przeniesienie na Astro/Next.js + headless CMS (Sanity/Contentful)

**Opis:** Nowoczesny frontend framework + headless CMS jako zrodlo tresci.

**Zalety:**
- W pelni nowoczesny stack
- Potezny edytor tresci (Sanity Studio, Contentful UI)
- Role uzytkownikow, workflow publikacji
- API do tresci
- Swietny DX

**Wady:**
- Wymaga calkowitej przebudowy strony
- Koszty: Sanity (darmowy plan do pewnego limitu), Contentful (darmowy do 5 uzytkownikow)
- Wymaga hostingu na Vercel/Netlify (darmowe plany dostepne)
- Overkill dla prostej strony stowarzyszenia

**Naklad pracy:** DUZY (2-3 tygodnie)

---

### Opcja C: WordPress

**Opis:** Klasyczny CMS, najczesciej uzywany na swiecie.

**Zalety:**
- Najbardziej znany CMS -- latwy dla uzytkownikow
- Ogromna ilosc wtyczek (wielojezycznosc, formularze, SEO)
- Wbudowane role uzytkownikow (admin, editor, author, contributor)
- WYSIWYG edytor, Gutenberg blocks

**Wady:**
- Wymaga serwera z PHP + MySQL (koniec darmowego GitHub Pages)
- Koszty hostingu: ~50-150 PLN/miesiac
- Wymaga utrzymania (aktualizacje, bezpieczenstwo, backupy)
- Wolniejszy niz strona statyczna
- Podatny na ataki (bez odpowiedniego utrzymania)

**Naklad pracy:** SREDNI (1-2 tygodnie z przeniesieniem tresci)

---

### Opcja D: Hugo/11ty + DecapCMS na Netlify/Cloudflare Pages

**Opis:** Zamiana Jekyll na nowszy SSG + ten sam CMS approach co Opcja A.

**Zalety:**
- Hugo/11ty sa szybsze i aktywniej rozwijane niz Jekyll
- Netlify/Cloudflare Pages = darmowy hosting z CI/CD
- DecapCMS dziala identycznie
- Lepszy DX niz Jekyll

**Wady:**
- Wymaga migracji z Jekyll (umiarkowany naklad)
- Jezeli zostajemy przy DecapCMS, te same ograniczenia co Opcja A

**Naklad pracy:** SREDNI (1-2 tygodnie)

---

## 8. Rekomendacja

### Dla strony SPMPZ rekomenduje: Opcja A (DecapCMS + zrefaktorowany Jekyll)

**Dlaczego:**
1. **Najnizszy koszt i naklad** -- strona zostaje na GitHub Pages (za darmo)
2. **Odpowiedni dla skali** -- to strona malego stowarzyszenia, nie potrzebuje WordPressa ani headless CMS
3. **Wystarczajacy dla celu** -- uzytkownicy moga dodawac artykuly przez przegladarke
4. **Nie wymaga utrzymania serwera** -- brak PHP, brak bazy danych

### Plan wdrozenia:
1. **Refaktor Jekyll** -- naprawic istniejacy kod:
   - Wszystkie strony uzyc z layouts i includes (usunac hardcoded HTML)
   - Naprawic HTTP -> HTTPS
   - Zastapic jQuery 1.11 nowoczesnym rozwiazaniem lub usunac
   - Zastapic Skel.js prostym CSS Grid/Flexbox
   - Dodac meta viewport, SEO basics
2. **Dodac `_posts/` kolekcje** -- artykuly jako pliki Markdown
3. **Dodac DecapCMS** -- folder `admin/` z konfiguracją
4. **Skonfigurowac autentykacje** -- Netlify Identity lub GitHub OAuth
5. **Przetestowac** -- workflow dodawania artykulu przez przegldarke

### Alternatywa jesli potrzeba wiecej:
Jesli w przyszlosci potrzeby rosna (wiele rol, zaawansowane workflow, newsletter), wtedy migracja na **Astro + Sanity** (Opcja B) bedzie naturalnym krokiem.
