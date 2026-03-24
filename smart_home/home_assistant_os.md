# Home Assistant OS

---

## Co to jest?

**Home Assistant OS (HAOS)** to dedykowany system operacyjny stworzony specjalnie do uruchamiania Home Assistanta. Jest to pełny, zoptymalizowany Linux, który zawiera:
- Home Assistant Core (silnik automatyzacji)
- Home Assistant Supervisor (zarządza add-onami, backupami, aktualizacjami)
- System operacyjny (zarządza siecią, dyskiem, bootloaderem)

To jest ta wersja, którą instalujesz na Proxmox jako VM (zgodnie z Twoim planem).

---

## HAOS vs inne metody instalacji

| Metoda | Supervisor | Add-ony | Backupy | Aktualizacje | Dla kogo |
|--------|-----------|---------|---------|-------------|----------|
| **Home Assistant OS** | ✅ | ✅ | ✅ automatyczne | ✅ jednym klikiem | Większość użytkowników, Twój wybór |
| HA Container (Docker) | ❌ | ❌ | ręczne | ręczne | Zaawansowani, którzy chcą kontrolę nad Dockerem |
| HA Core (Python venv) | ❌ | ❌ | ręczne | ręczne | Deweloperzy |
| HA Supervised (na Debianie) | ✅ | ✅ | ✅ | ✅ | Zaawansowani, chcą pełny Debian + Supervisor |

**Dlaczego HAOS na Proxmox to najlepsza opcja?**
- Masz pełną funkcjonalność (add-ony, backupy, aktualizacje)
- Proxmox daje snapshoty na poziomie VM (dodatkowa warstwa bezpieczeństwa)
- Możesz odpalić inne VM/kontenery obok (Pi-hole, NAS itp.)

---

## Kluczowe funkcje HAOS

### Add-ony (dodatki)
Add-ony to usługi uruchamiane wewnątrz HAOS, zarządzane przez Supervisor. Przykłady:

| Add-on | Do czego |
|--------|----------|
| **File Editor** | Edycja plików konfiguracyjnych z poziomu przeglądarki |
| **Samba Share** | Dostęp do plików HA z komputera przez sieć (SMB) |
| **Terminal & SSH** | Dostęp do konsoli HA |
| **Mosquitto MQTT** | Broker MQTT (jeśli będziesz miał urządzenia MQTT) |
| **ESPHome** | Programowanie urządzeń ESP32/ESP8266 |
| **Zigbee2MQTT** | Alternatywa dla ZHA — bardziej konfigurowalny |
| **Let's Encrypt** | Certyfikat SSL za darmo |
| **Google Drive Backup** | Automatyczny backup na Google Drive |
| **AdGuard Home** | Blokowanie reklam w całej sieci (alternatywa Pi-hole) |

### Backupy
- HAOS robi automatyczne backupy konfiguracji
- Można ustawić harmonogram (codziennie, co tydzień)
- Backup zawiera: konfigurację, add-ony, automatyzacje, dashboardy
- Można przywrócić na nowej instalacji — pełna migracja

### Aktualizacje
- Powiadomienie w UI gdy jest nowa wersja
- Aktualizacja jednym kliknięciem
- HAOS aktualizuje się oddzielnie od Core (system vs aplikacja)
- **Zawsze rób snapshot w Proxmox przed aktualizacją!**

---

## Wymagania systemowe

| Parametr | Minimum | Twój GMKtec G3 |
|----------|---------|-----------------|
| CPU | 2 rdzenie x86-64 | ✅ N100, 4 rdzenie |
| RAM | 2 GB | ✅ 8/16 GB |
| Dysk | 32 GB | ✅ wystarczający |
| Sieć | Ethernet (zalecane) | ✅ |

Twój sprzęt spokojnie wystarczy — N100 z HAOS zużywa ~5–10W.

---

## Ważne ścieżki i pliki

| Ścieżka | Co zawiera |
|---------|------------|
| `/config/configuration.yaml` | Główny plik konfiguracyjny |
| `/config/automations.yaml` | Automatyzacje (lub w UI) |
| `/config/scenes.yaml` | Sceny |
| `/config/scripts.yaml` | Skrypty |
| `/config/secrets.yaml` | Hasła i tokeny (nie wrzucać do gita!) |
| `/config/custom_components/` | Integracje z HACS |

---

## HACS — dodatkowy "sklep" z integracjami

**HACS** (Home Assistant Community Store) to nieoficjalny marketplace z integracjami i kartami dashboardu tworzonymi przez społeczność. Nie jest częścią HAOS, ale warto zainstalować.

Popularne integracje z HACS:
- **Mushroom Cards** — nowoczesne karty dashboardu
- **Browser Mod** — kontrola przeglądarki z HA
- **Xiaomi Miot** — pełna obsługa urządzeń Xiaomi
- **Adaptive Lighting** — automatyczne dopasowanie temperatury barwowej światła do pory dnia

---

## Wskazówki

- **Nie edytuj plików systemowych HAOS** — tylko `/config/`
- **Zainstaluj add-on Samba** od razu — łatwiej edytować pliki z komputera
- **Add-on Google Drive Backup** — ustaw jako pierwszy, zanim cokolwiek skonigurujesz
- **Snapshoty Proxmox + backupy HA** = podwójne zabezpieczenie
