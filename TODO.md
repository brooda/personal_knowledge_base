# TODO

## Strony internetowe

### sportowewakacje.com.pl (Wojtek)
- Repo: https://github.com/brooda/sportowewakacje
- [ ] Migracja z Jekyll na Astro lub 11ty
- [ ] Wymiana Bootstrap 3 + jQuery 2 na nowoczesny CSS/JS
- [ ] Usunięcie ~30 zbędnych skryptów JS i polyfilli IE8/9
- [ ] Optymalizacja obrazów i CSS (style.css 125KB - większość nieużywana)
- [ ] Poprawka HTTP -> HTTPS dla wszystkich zasobów
- [ ] Dodanie .gitignore, usunięcie _site/ z repo
- [ ] Aktualizacja formularzy kontaktowych (reCAPTCHA v1 wycofana)
- Szczegółowa analiza: technologie/web/sportowewakacje_analiza.md

### SPMPZ - Stowarzyszenie Miast Partnerskich Zamościa
- Repo: https://github.com/brooda/SPMPZ
- Live: https://brooda.github.io/SPMPZ/
- [ ] Refaktor HTML - wykorzystanie layoutów/includes Jekyll (teraz copy-paste nawigacji w każdym pliku)
- [ ] Dodanie DecapCMS (admin panel w przeglądarce) + kolekcja _posts/ na artykuły
- [ ] Konfiguracja autoryzacji (GitHub OAuth) dla wielu użytkowników
- [ ] Wymiana Skel.js (martwy framework) na CSS Grid/Flexbox
- [ ] Poprawka HTTP -> HTTPS (jQuery i fonty się nie ładują!)
- [ ] Porządek w plikach angielskich (3 duplikaty: english.html, index_en.html, index_enn.html)
- [ ] Aktualizacja zależności (jQuery 1.11, FontAwesome 4.0.1)
- Szczegółowa analiza: technologie/web/spmpz_analiza_strony.md
