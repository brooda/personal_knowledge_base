# Porządki w skrzynce (piotrbrodka95@gmail.com)

## Diagnoza
- ~80% inboxa to szum: newslettery (~40%), powiadomienia o paczkach/zakupach (~20%), stare alerty kalendarza, Google security
- Realna korespondencja trafia się rzadko (Genesio, kontakty biznesowe)
- Etykiety są już dobrze zdefiniowane (Praca, Osobiste, SPMPZ, Erasmus, Potwierdzenia, Loty, Newslettery, 4 adresy) — tylko nieużywane

## Plan (kolejność wg ROI)

### 1. Bulk-unsubscribe z newsletterów (ręcznie w Gmail UI)
- Otworzyć `category:promotions`, zaznaczyć wszystko, kliknąć "Wypisz się" przy każdym źródle
- Główni kandydaci do wypisania:
  - AI Ninjas (kontakt@aininjas.pl)
  - Claude (no-reply@email.claude.com)
  - Warp (feedback+customerio@warp.dev)
  - Cursor (team@mail.cursor.com)
  - Adobe (mail@mail.adobe.com)
  - Neo4j (webinar@neo4j.com)
  - Magene (no-reply@news.magenefitness.com)
  - Wahoo (noreply@mail.wahoofitness.com)
  - Packt (packt@mail.packtpub.com)
  - Azure/Microsoft (Azure@promomail.microsoft.com)
  - Meetup (info@meetup.com)
  - Netflix promo (info@members.netflix.com)
  - eobuwie (info@eobuwie.pl)
  - onthatass (noreply-pl@onthatass.com)
  - InPost newsletter (newsletter-info@inpost.pl)
  - restaurant@week.pl
  - transparentworld (mirek@transparentworld.pl) — jeśli to newsletter a nie osoba

### 2. Filtry na powiadomienia transakcyjne

**Ręcznie w Gmail UI** (Ustawienia → Filtry → Utwórz nowy filtr):
- Dla każdego `from:` poniżej: Skip Inbox + Apply label "Potwierdzenia"
- Nadawcy:
  - `transaction@notice.aliexpress.com`
  - `info@paczkomaty.pl`
  - `powiadomienia@allegromail.pl`
  - `powiadomienia@allegropay.pl`
  - `powiadomienia@ankiety.allegro.pl`
  - `no-reply@accounts.google.com` (security alerts — opcjonalnie, bo warto je widzieć)

**Retroaktywnie (MCP może)**: znaleźć istniejące maile od tych nadawców, nadać etykietę "Potwierdzenia" i zdjąć INBOX

### 3. Inbox Zero lite — reguła czego chcesz widzieć
- Inbox pokazuje tylko:
  - maile od ludzi (nie no-reply/marketing)
  - faktury/rzeczy wymagające akcji
- Wszystko inne → etykieta + out of inbox

### 4. Bulk-archive historii (MCP może)
- `in:inbox older_than:1y is:read` → Archive (zdjęcie etykiety INBOX)
- Nic nie jest kasowane, tylko znika z głównego widoku
- Bezpieczne — w razie czego wszystko znajdziesz przez wyszukiwanie

### 5. Stare powiadomienia "stoicki cytat" (MCP może)
- `from:calendar-notification@google.com subject:"stoicki cytat"` → Trash
- Setki starych maili, cykl kalendarza już usunięty (2026-04-17)

## Podział pracy

**Co mogę zrobić ja (MCP Gmail)**:
- Masowe wyszukiwanie, nadawanie/zdejmowanie etykiet, archiwizacja, przenoszenie do TRASH
- Retroaktywne "udawanie filtra" dla istniejącej historii

**Co musisz ty (Gmail UI)**:
- Klikanie "Unsubscribe" (MCP nie obsługuje)
- Tworzenie filtrów Gmail dla przyszłych maili (API Gmail nie wystawia `filters.create` przez MCP)

## Status
- Plan spisany: 2026-04-17
- Wykonanie: na kiedy indziej
