# ZAP — Zed Attack Proxy

---

## Co to jest?

**ZAP (Zed Attack Proxy)** to darmowy, open-source'owy skaner bezpieczeństwa aplikacji webowych. Dawniej projekt OWASP, teraz rozwijany przez **SSP (Software Security Project)**.

Służy do **DAST** (Dynamic Application Security Testing) — testuje działającą aplikację, szukając podatności w runtime.

GitHub: github.com/zaproxy/zaproxy

---

## Co wykrywa?

| Kategoria | Przykłady |
|-----------|-----------|
| **Injection** | SQL Injection, OS Command Injection, LDAP Injection |
| **XSS** | Reflected XSS, Stored XSS, DOM-based XSS |
| **Broken Auth** | Słabe sesje, brak logoutu, session fixation |
| **Security Misconfiguration** | Brakujące nagłówki (CSP, HSTS, X-Frame-Options) |
| **Sensitive Data Exposure** | Dane w URL, brak HTTPS, wyciek w komentarzach |
| **CSRF** | Brak tokenów anty-CSRF |
| **Directory Traversal** | Path traversal, dostęp do plików systemowych |

---

## Instalacja

```bash
# macOS
brew install zaproxy

# Linux (snap)
snap install zaproxy --classic

# Docker
docker run -u zap -p 8080:8080 ghcr.io/zaproxy/zaproxy:stable zap-webswing.sh
```

Lub: pobierz z zaproxy.org (GUI dla Windows/Mac/Linux)

---

## Tryby pracy

### 1. Automated Scan (Quick Start)
Wpisujesz URL → ZAP automatycznie skanuje aplikację (spidering + active scan).
```bash
# Z wiersza poleceń
zap-baseline.py -t https://example.com
```

### 2. Manual Explore (proxy)
ZAP działa jako proxy HTTP (domyślnie `localhost:8080`). Przeglądasz aplikację ręcznie, a ZAP rejestruje wszystkie requesty i testuje je.

### 3. API Scan
Skanowanie API na podstawie definicji OpenAPI/Swagger:
```bash
zap-api-scan.py -t https://example.com/api/swagger.json -f openapi
```

---

## Najczęstsze użycie w CI/CD

### Baseline Scan (szybki, pasywny)
```bash
docker run ghcr.io/zaproxy/zaproxy:stable zap-baseline.py \
  -t https://myapp.com \
  -r report.html
```
- Tylko pasywne reguły (nie atakuje aplikacji)
- Szybki (~1–2 min)
- Dobry na CI/CD

### Full Scan (aktywny, agresywny)
```bash
docker run ghcr.io/zaproxy/zaproxy:stable zap-full-scan.py \
  -t https://myapp.com \
  -r report.html
```
- Aktywne ataki (SQL injection, XSS itp.)
- Wolny (~30 min+)
- Używaj na środowisku testowym, **nigdy na produkcji**

---

## ZAP vs inne skanery DAST

| Cecha | ZAP | Burp Suite | Nikto | Nuclei |
|-------|-----|-----------|-------|--------|
| Open source | ✅ | ❌ (Community Edition ograniczona) | ✅ | ✅ |
| GUI | ✅ | ✅ | ❌ | ❌ |
| Automatyzacja/CI | ✅ | ✅ (Enterprise) | ❌ | ✅ |
| API scanning | ✅ | ✅ | ❌ | ✅ |
| Aktywne skanowanie | ✅ | ✅ | Ograniczone | ✅ |
| Rozszerzalność | Add-ons, skrypty | Extensions | — | Templates YAML |
| Koszt | Darmowy | $449+/rok (Pro) | Darmowy | Darmowy |

---

## Przydatne integracje

- **Jenkins** — ZAP Plugin
- **GitHub Actions** — `zaproxy/action-baseline`, `zaproxy/action-full-scan`
- **GitLab CI** — Docker image
- **Selenium** — ZAP jako proxy podczas testów E2E

---

> **Moje przemyślenia:**
> *(tu wpisuj swoje notatki)*
