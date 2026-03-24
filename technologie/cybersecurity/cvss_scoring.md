# CVSS — Common Vulnerability Scoring System

---

## Co to jest?

**CVSS** to otwarty standard oceny krytyczności podatności bezpieczeństwa. Każda podatność dostaje **ocenę 0.0–10.0** wraz z wektorem opisującym jej charakterystykę.

Aktualnie używany: **CVSS v3.1** (standard) i **CVSS v4.0** (najnowszy, od 2023).

---

## Skala ocen

| Zakres | Krytyczność | Kolor | Przykład |
|--------|-------------|-------|---------|
| 0.0 | Brak | — | — |
| 0.1–3.9 | **Niska** | 🟢 | Information disclosure, słaby XSS |
| 4.0–6.9 | **Średnia** | 🟡 | Stored XSS, CSRF |
| 7.0–8.9 | **Wysoka** | 🟠 | SQL Injection, RCE z uwierzytelnieniem |
| 9.0–10.0 | **Krytyczna** | 🔴 | Remote Code Execution bez auth, Log4Shell |

---

## Metryki CVSS v3.1

### Base Score (metryki bazowe) — najważniejsze

**Exploitability Metrics** (jak łatwo zaatakować):

| Metryka | Skrót | Wartości |
|---------|-------|----------|
| Attack Vector | AV | Network (N) / Adjacent (A) / Local (L) / Physical (P) |
| Attack Complexity | AC | Low (L) / High (H) |
| Privileges Required | PR | None (N) / Low (L) / High (H) |
| User Interaction | UI | None (N) / Required (R) |

**Impact Metrics** (jaki jest skutek ataku):

| Metryka | Skrót | Wartości |
|---------|-------|----------|
| Confidentiality | C | None (N) / Low (L) / High (H) |
| Integrity | I | None (N) / Low (L) / High (H) |
| Availability | A | None (N) / Low (L) / High (H) |
| Scope | S | Unchanged (U) / Changed (C) |

### Jak czytać wektor CVSS?

Przykład: `CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:C/C:H/I:H/A:H` = **10.0 (Krytyczny)**

Oznacza: atak przez sieć, niska złożoność, bez uprawnień, bez interakcji użytkownika, wpływa na inne systemy, pełna utrata poufności, integralności i dostępności.

### Temporal Score (opcjonalne)
- Exploit Code Maturity — czy istnieje exploit?
- Remediation Level — czy jest poprawka?
- Report Confidence — jak pewne jest zgłoszenie?

### Environmental Score (opcjonalne)
- Dostosowanie do Twojego środowiska (np. jak ważny jest dany system w Twojej firmie)

---

## CVSS v4.0 — co nowego?

- Bardziej granularne metryki ataku
- Nowa metryka: **Attack Requirements (AT)** — wymagania po stronie atakującego
- Rozdzielenie Impact na **Vulnerable System** i **Subsequent System**
- Lepsza obsługa IoT/OT/ICS
- Uproszczone nazwy grup: Base → CVSS-B, Temporal zastąpione przez Threat → CVSS-BT

---

## Narzędzia do obliczania CVSS

| Narzędzie | URL |
|-----------|-----|
| **NIST CVSS Calculator** | nvd.nist.gov/vuln-metrics/cvss/v3-calculator |
| **FIRST CVSS v4.0 Calculator** | first.org/cvss/calculator/4.0 |
| **NVD (National Vulnerability Database)** | nvd.nist.gov — baza wszystkich CVE z ocenami CVSS |

---

## Wskazówki praktyczne

- CVSS to **punkt wyjścia**, nie ostateczna decyzja — kontekst firmy jest kluczowy
- Podatność z CVSS 6.0 w systemie krytycznym może być pilniejsza niż CVSS 9.0 w systemie testowym
- Zawsze sprawdzaj czy istnieje **publiczny exploit** (Temporal Score)
- W raportach bezpieczeństwa zawsze podawaj pełny wektor, nie tylko liczbę

> **Moje przemyślenia:**
> *(tu wpisuj swoje notatki)*
