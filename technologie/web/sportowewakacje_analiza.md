# Analiza repozytorium sportowewakacje

**Repo:** https://github.com/brooda/sportowewakacje
**Data analizy:** 2026-03-25
**Ostatni push:** 2021-11-04 (ponad 4 lata temu)

---

## 1. Czym jest ta strona

Strona internetowa firmy **MAJ Joanna Maciej Jowko** z Ozarowa Mazowieckiego (sportowewakacje.com.pl). Firma organizuje:
- **Obozy sportowe** (letnie i zimowe - narciarskie, np. Szwajcaria Jungfrau, Wlochy Claviere)
- **Zajecia tenisa ziemnego** na kortach w Ozarowie Mazowieckim
- **Zajecia plywackie** na plywalni w Ozarowie Mazowieckim

Strona pelni role wizytowki/katalogu ofert. Jest w jezyku polskim.

Kontakt: Maciej Jowko (603 762 608), Wojciech Galecki (503 007 947), biuro@sportowewakacje.com.pl

---

## 2. Stack technologiczny

### Jekyll (minimalna konfiguracja)
- Uzywa Jekyll do templating (katalogi `_includes`, `_layouts`, `_site`)
- **Brak `_config.yml`** - brak jawnej konfiguracji Jekyll
- **Brak `Gemfile`** - brak zarzadzania zaleznosci Ruby
- **Brak informacji o wersji Jekyll** - prawdopodobnie bardzo stara wersja
- `.jekyll-cache` commitowany do repo (powinien byc w .gitignore)
- `_site` (output build) commitowany do repo (powinien byc w .gitignore)

### Frontend
- **jQuery 2.1.0** (2014) - bardzo przestarzaly
- **Bootstrap 3.1.1** (2014) - bardzo przestarzaly (aktualna wersja: 5.3.x)
- **Font Awesome 4.x** (stara wersja, ladowana z plikow .eot/.woff/.ttf)
- **Google Fonts** - Open Sans, Yellowtail (ladowane po HTTP, nie HTTPS!)
- **Revolution Slider** (ThemePunch) - komercyjny slider jQuery
- **bxSlider** - jQuery slider
- **FlexSlider** - jQuery slider
- **Fancybox** - lightbox
- **WOW.js** - animacje przy scrollu
- **Isotope/MixItUp** - filtrowanie (nieuzywane w praktyce)
- **Modernizr, Respond.js, html5shiv** - polyfille dla IE8/9

### CSS
- **Glowny szablon: "Automotive" by Theme Suite** (v1.8) - szablon HTML dla dealera samochodowego(!) przerobiony na strone sportowa
- 16 plikow CSS, w tym `style.css` (125KB) - ogromny, nieuzywany w wiekszosci
- `custom.css` - wlasne nadpisania (stosunkowo krotki, czytelny)
- `mobile.css` - osobny plik na responsywnosc (podejscie sprzed ery mobile-first)

### PHP
- Formularze kontaktowe w PHP (`forms/` - friend.php, offer.php, request.php, schedule.php, trade.php)
- Integracja z Twitter API (tmhOAuth) - prawdopodobnie nieczynna
- reCAPTCHA v1 (przestarzala, wylogowana z uzycia)

### Fonty
- Lokalne pliki fontow (Open Sans, Yellowtail, FontAwesome, Glyphicons, FlexSlider icons, RevIcons)
- Formaty: .eot, .svg, .ttf, .woff (brak .woff2)

---

## 3. Struktura strony

### Layouty (`_layouts/`)
- `index.html` - glowna strona (caly HTML inline, z headerem, sliderem, trescia, footerem)
- `subpage.html` - podstrona jednokolumnowa
- `subpage_twocol.html` - podstrona dwukolumnowa (kontakt)

### Includy (`_includes/`)
- `head.html` - sekcja <head> (CSS, JS, meta)
- `header.html` - nawigacja
- `footer.html` - tylko przycisk "back to top" (!)
- `slider_mala_akademia.html`, `slider_oboz_tenis.html`, `slider_oboz_zima.html`, `slider_tenis.html` - slajdy Revolution Slider

### Strony glowne
- `index.html` - strona glowna (tenis + plywanie)
- `tenis.html` - oferta tenisa
- `plywanie.html` - oferta plywania
- `contact.html` - kontakt z mapa Google
- `faq.html` - FAQ

### Strony ofert (archiwalne)
- `oboz_letni_2018.html` - oboz letni 2018
- `oboz_letni_2019.html` - oboz letni 2019
- `oboz_zimowy_2019.html` - oboz zimowy 2019
- `oboz_zimowy_2020.html` - oboz zimowy Szwajcaria 2020

### Archiwum (`stare/`)
- Starsze wersje stron (akademia, oboz pilkarski, plywacko-tenisowy, zimowy)
- Pliki .doc (deklaracja, karta uczestnika)

---

## 4. Zarzadzanie trescia

- **Brak CMS** - tresc pisana recznie w HTML wewnatrz plikow .html z front matter Jekyll
- **Brak Markdown** - strony uzywaja czystego HTML (z drobnymi wyjatkami)
- **Brak systemu blogu** - kazdy oboz to oddzielny plik HTML
- **Brak kolekcji Jekyll** (collections) - obozy moglyby byc kolekcja
- **Brak data files** (_data/) - dane kontaktowe zduplikowane w wielu plikach

---

## 5. Problemy i ocena jakosci kodu

### Krytyczne
1. **Brak HTTPS** - skrypty i fonty ladowane po HTTP (Cookie Script, Google Fonts, Google Maps)
2. **_site i .jekyll-cache w repo** - build output nie powinien byc w wersjonowaniu
3. **Brak .gitignore**
4. **Dane wrazliwe w repo** - numery kont bankowych, numery telefonow, adresy
5. **Google Maps API bez klucza** - `key&sensor=false` - mapa prawdopodobnie nie dziala

### Przestarzale
1. jQuery 2.1.0 (2014) - 12 lat!
2. Bootstrap 3.1.1 (2014) - 12 lat! (EOL)
3. Font Awesome 4 - brak wsparcia
4. Revolution Slider - stara wersja
5. IE8/9 polyfille (html5shiv, respond.js, modernizr) - niepotrzebne od lat
6. Cookie Script po HTTP
7. Facebook SDK v2.4 - bardzo przestarzaly
8. Twitter feed integration - prawdopodobnie nie dziala (stare API)
9. reCAPTCHA v1 - wylogowana z uzycia przez Google

### Architektoniczne
1. Szablon "Automotive" (dealer samochodowy) - zle dopasowany do tresci sportowej
2. 125KB style.css - ogromna ilosc nieuzywanych styli (pricing tables, inventory, car listings...)
3. ~30 plikow JS zaladowanych na kazda strone - brak bundlowania
4. Zduplikowany content (footer z danymi kontaktowymi powielony w layout i stronach)
5. Brak SEO (meta description puste, brak structured data)
6. Brak optymalizacji obrazkow (duze JPG bez kompresji)
7. Inline JavaScript w layoutach
8. Uzycie tagu `<center>` (przestarzaly HTML)
9. Literowki w tresci ("umietnosci" zamiast "umiejetnosci")

### Bezpieczenstwo
1. Formularze PHP bez widocznej walidacji server-side
2. Stare biblioteki z potencjalnymi CVE (jQuery 2.1.0 ma znane podatnosci)

---

## 6. Jekyll w 2026 - czy to nadal dobry wybor?

### Stan Jekyll w 2026
- Ostatnie wieksze wydanie: Jekyll 4.3 (2023)
- Rozwoj bardzo spowolnil - maly team maintainerow
- GitHub Pages nadal wspiera Jekyll (ale tylko starsze wersje ~3.9)
- Ruby nie jest popularnym jezykiem w ekosystemie frontend
- Ekosystem pluginow stagnuje

### Porownanie alternatyw dla tego typu strony (maly biznes, wizytowka + oferty)

| Cecha | Jekyll | Hugo | Astro | 11ty (Eleventy) | Next.js |
|-------|--------|------|-------|-----------------|---------|
| **Szybkosc builda** | Wolny | Bardzo szybki | Szybki | Szybki | Sredni |
| **Jezyk** | Ruby | Go | JS/TS | JS | JS/TS |
| **Krzywa nauki** | Niska | Niska | Srednia | Niska | Wysoka |
| **Hosting** | GitHub Pages | Dowolny | Dowolny | Dowolny | Vercel/Node |
| **CMS integracja** | Ograniczona | Dobra | Doskonala | Dobra | Doskonala |
| **Spolecznosc 2026** | Malejaca | Duza, aktywna | Rosnaca, wiodaca | Stabilna | Ogromna |
| **Zero JS default** | Tak | Tak | Tak | Tak | Nie |
| **Koszt utrzymania** | Za darmo (GH Pages) | Za darmo (Cloudflare/Netlify) | Za darmo | Za darmo | Za darmo (Vercel) |

### Rekomendacja dla sportowewakacje

**Najlepszy wybor: Astro lub 11ty (Eleventy)**

#### Astro (polecane #1)
- Swietne do stron contentu (content collections idealnie dla ofert obozow)
- Zero JS domyslnie - strona bedzie szybka
- Mozliwosc uzycia dowolnych komponentow (React, Vue, Svelte) gdy potrzebne
- Integracja z headless CMS (np. Tina CMS, Decap CMS) - latwa edycja ofert
- Wbudowana optymalizacja obrazkow
- Deployment na Cloudflare Pages / Netlify za darmo
- Aktywny rozwoj, duza spolecznosc

#### 11ty / Eleventy (polecane #2)
- Najblizszy duchowy nastepca Jekyll
- Bardzo prosty, minimalny
- Moze uzywac tych samych plikow Markdown/Liquid co Jekyll
- Latwa migracja z Jekyll
- Zero JS domyslnie

#### Hugo (alternatywa)
- Najszybszy build
- Dobry do prostych stron
- Szablony w Go templates (mniej intuicyjne)

#### Next.js (overkill)
- Zdecydowanie za duzy dla tej strony
- Wymaga serwera Node.js lub Vercel
- Sens ma tylko gdy strona wymaga zaawansowanej interakcji

---

## 7. Co zrobic przy modernizacji

### Priorytet 1 - Bezpieczenstwo i dzialanie
1. Usunac _site i .jekyll-cache z repo, dodac .gitignore
2. Zamienic HTTP na HTTPS wszedzie
3. Naprawic Google Maps API key
4. Zaktualizowac lub usunac Facebook SDK

### Priorytet 2 - Migracja technologii
1. Zmigrować do Astro lub 11ty
2. Zamienic Bootstrap 3 na nowoczesny CSS (grid/flexbox) lub Tailwind
3. Usunac jQuery - nowoczesny vanilla JS wystarczy
4. Uzyc woff2 dla fontow lub Google Fonts CDN po HTTPS
5. Zoptymalizowac obrazki (WebP, lazy loading)

### Priorytet 3 - Funkcjonalnosc
1. Stworzyc content collection dla obozow (zamiast osobnych plikow HTML)
2. Dodac headless CMS (Tina/Decap) do latwej edycji ofert
3. Dodac SEO (meta tags, structured data, sitemap)
4. Zastapic PHP formularze serwisem (Formspree, Netlify Forms)
5. Dodac nowoczesna galerie zdjec (bez jQuery plugins)
