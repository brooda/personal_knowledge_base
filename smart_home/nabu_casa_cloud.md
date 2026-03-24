  # Nabu Casa — Home Assistant Cloud

---

## Co to jest?

**Nabu Casa** to firma stojąca za Home Assistantem. Oferuje płatną usługę **Home Assistant Cloud**, która dodaje kilka kluczowych funkcji "na kliknięcie" — bez konfiguracji serwerów, VPN-ów czy portów.

**Cena:** ~$6.50/miesiąc (lub $65/rok)

Pieniądze idą na rozwój Home Assistanta (open source) — to główne źródło finansowania projektu.

---

## Co daje Home Assistant Cloud?

### 1. Zdalny dostęp (Remote Access)
- Dostęp do Home Assistanta **spoza domu** przez internet
- Bez konfiguracji portów, DDNS, VPN czy reverse proxy
- Szyfrowane połączenie (TLS) przez serwery Nabu Casa
- Adres: `https://twoja-instancja.ui.nabu.casa`

**Bez Nabu Casa** musisz sam skonfigurować:
- Port forwarding na routerze
- DuckDNS / Cloudflare Tunnel
- Certyfikat SSL (Let's Encrypt)
- Lub VPN (WireGuard / Tailscale)

### 2. Asystent głosowy — Alexa i Google Home
- **Natywna integracja z Alexa** — sterowanie urządzeniami HA głosem
- **Natywna integracja z Google Home** — j.w.
- Jedno kliknięcie w ustawieniach HA → działa
- Bez Nabu Casa: trzeba ręcznie ustawiać Smart Home Skill (Alexa) lub Google Actions — skomplikowane i wymaga konta deweloperskiego

### 3. Webhooks
- Pozwala tworzyć automatyzacje wyzwalane z zewnątrz
- Np. IFTTT, Tasker, Shortcuts (iOS) mogą triggerować HA

### 4. Text-to-Speech (TTS)
- Zamiana tekstu na mowę przez chmurę
- Lepszej jakości niż lokalne TTS

---

## Czy warto? Porównanie

| Funkcja | Bez Nabu Casa | Z Nabu Casa |
|---------|---------------|-------------|
| Zdalny dostęp | Sam konfigurujesz (VPN/Cloudflare/DuckDNS) | Działa od razu |
| Alexa/Google | Skomplikowana ręczna konfiguracja | Jedno kliknięcie |
| Backup do chmury | Google Drive add-on (darmowy) | Google Drive add-on (darmowy) |
| TTS | Lokalne (gorsze) lub Google TTS (darmowe) | Nabu Casa TTS (lepsze) |
| Koszt | $0 | ~$6.50/mies. |
| Wspiera projekt | ❌ | ✅ |

### Kiedy warto?
- Chcesz zdalny dostęp bez zabawy z siecią
- Masz Alexę lub Google Home i chcesz głosowe sterowanie
- Chcesz wspierać rozwój HA

### Kiedy nie musisz?
- Używasz HA tylko w domu (LAN)
- Umiesz skonfigurować Cloudflare Tunnel lub Tailscale
- Nie masz asystenta głosowego

---

## Darmowe alternatywy dla zdalnego dostępu

| Metoda | Trudność | Opis |
|--------|----------|------|
| **Tailscale** | ⭐ łatwa | VPN mesh — instalujesz na telefonie i HA, działa jak LAN. Darmowy do 100 urządzeń |
| **Cloudflare Tunnel** | ⭐⭐ średnia | Tunel przez Cloudflare, wymaga domeny. Darmowy |
| **WireGuard** | ⭐⭐⭐ trudna | VPN na routerze/serwerze. Szybki, ale wymaga konfiguracji |
| **DuckDNS + Let's Encrypt** | ⭐⭐ średnia | Darmowa domena + SSL. Wymaga port forwarding na routerze |
| **Nginx Proxy Manager** | ⭐⭐ średnia | Reverse proxy z SSL. Kontener na Proxmox obok HA |

> 💡 **Rekomendacja na start:** Zacznij bez Nabu Casa. Jeśli będziesz potrzebował zdalnego dostępu, wypróbuj **Tailscale** (najłatwiejszy, darmowy). Jeśli chcesz Alexę/Google Home bezproblemowo — wtedy Nabu Casa się opłaca.

---

## Jak aktywować?

1. W Home Assistant: **Ustawienia → Home Assistant Cloud**
2. Zarejestruj konto na Nabu Casa
3. Zaloguj się w HA
4. Włącz Remote Access, Alexa, Google Home — co potrzebujesz
5. 30 dni trial za darmo

---

## Prywatność

- Nabu Casa **nie ma dostępu** do Twoich danych z Home Assistanta
- Serwery Cloud działają jako proxy (przekazują ruch, nie czytają go)
- Dane i automatyzacje wciąż działają lokalnie
- Jeśli Nabu Casa padnie, HA działa dalej — tylko zdalny dostęp i asystenci głosowi nie działają
