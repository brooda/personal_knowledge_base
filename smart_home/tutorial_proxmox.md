# Tutorial: Proxmox VE na GMKtec G3 (N100)

## Spis treści

1. [Co to jest Proxmox?](#1-co-to-jest-proxmox)
2. [Co będzie potrzebne](#2-co-będzie-potrzebne)
3. [Pobranie i nagranie ISO na pendrive](#3-pobranie-i-nagranie-iso-na-pendrive)
4. [Instalacja Proxmox na GMKtec](#4-instalacja-proxmox-na-gmktec)
5. [Pierwsze logowanie do panelu webowego](#5-pierwsze-logowanie-do-panelu-webowego)
6. [Konfiguracja po instalacji](#6-konfiguracja-po-instalacji)
7. [Ustawienie stałego IP](#7-ustawienie-stałego-ip)
8. [Tworzenie pierwszego snapshota](#8-tworzenie-pierwszego-snapshota)
9. [Połączenie SSH z Maca](#9-połączenie-ssh-z-maca)
10. [Rozwiązywanie problemów](#10-rozwiązywanie-problemów)

---

## 1. Co to jest Proxmox?

Proxmox VE (Virtual Environment) to darmowy system operacyjny oparty na Debianie, który zamienia komputer w **hypervisor** — maszynę do uruchamiania maszyn wirtualnych (VM) i kontenerów (LXC).

Dlaczego Proxmox a nie zwykły Linux z Dockerem?
- **Panel webowy** — zarządzasz wszystkim z przeglądarki, nie musisz siedzieć w terminalu
- **Snapshoty** — zrobiłeś coś głupiego? Cofasz do poprzedniego stanu w 10 sekund
- **Izolacja** — Home Assistant działa w osobnej VM, jak zepsujesz jedną rzecz, reszta dalej chodzi
- **USB passthrough** — możesz przekazać dongle Zigbee bezpośrednio do VM

N100 w GMKtec G3 to idealny procesor pod Proxmox — mało prądu ciągnie, a mocy wystarczy na kilka VM naraz.

---

## 2. Co będzie potrzebne

| Rzecz | Uwagi |
|-------|-------|
| GMKtec G3 | Podłączony do monitora, klawiatury i prądu |
| Pendrive | Min. 2 GB, zostanie wyczyszczony! |
| Kabel Ethernet | Proxmox wymaga połączenia kablowego podczas instalacji |
| Drugi komputer (Mac) | Do pobrania ISO i nagrania pendrive'a |
| Monitor + klawiatura | Tylko na czas instalacji, potem zarządzasz zdalnie |

**UWAGA:** Instalacja Proxmox **wymaże cały dysk** GMKtec. Jeśli masz na nim coś ważnego — zrób backup przed instalacją.

---

## 3. Pobranie i nagranie ISO na pendrive

### Krok 3.1 — Pobierz ISO

Wejdź na: https://www.proxmox.com/en/downloads/proxmox-virtual-environment

Pobierz najnowszy **Proxmox VE ISO Installer**.

Albo z terminala Maca:
```bash
cd ~/Downloads
curl -LO https://enterprise.proxmox.com/iso/proxmox-ve_8.4-1.iso
```

> Sprawdź aktualny numer wersji na stronie — powyższy link może być nieaktualny.

### Krok 3.2 — Nagraj ISO na pendrive (Mac)

Podłącz pendrive i sprawdź jego identyfikator:
```bash
diskutil list
```

Szukaj pendrive'a po rozmiarze (np. `/dev/disk4`). **Upewnij się, że to na pewno pendrive, nie dysk Maca!**

Odmontuj pendrive (ale nie wyjmuj fizycznie):
```bash
diskutil unmountDisk /dev/diskX
```
*(zamień `diskX` na właściwy numer)*

Nagraj ISO:
```bash
sudo dd if=~/Downloads/proxmox-ve_8.4-1.iso of=/dev/rdiskX bs=4M status=progress
```

> Użyj `rdiskX` (z literką `r`) — jest dużo szybsze niż `diskX`.
> To potrwa kilka minut. Jak zakończy się bez błędu — pendrive jest gotowy.

Po zakończeniu:
```bash
diskutil eject /dev/diskX
```

---

## 4. Instalacja Proxmox na GMKtec

### Krok 4.1 — Boot z pendrive'a

1. Włóż pendrive do GMKtec
2. Podłącz monitor, klawiaturę i kabel Ethernet
3. Włącz komputerek
4. Wciśnij **F7** lub **DEL** podczas startu (zależy od BIOS-u GMKtec) żeby wejść w Boot Menu
5. Wybierz pendrive jako urządzenie do uruchomienia

### Krok 4.2 — Instalator Proxmox

1. **Welcome** → wybierz `Install Proxmox VE (Graphical)`
2. **EULA** → zaakceptuj licencję
3. **Target Harddisk** → wybierz dysk wewnętrzny GMKtec (zwykle jest tylko jeden)
   - Opcje domyślne (ext4) są OK
4. **Country, Time zone, Keyboard** →
   - Country: `Poland`
   - Timezone: `Europe/Warsaw`
   - Keyboard: `Polish`
5. **Password and Email** →
   - Ustaw hasło root (zapamiętaj je!)
   - Email: wpisz cokolwiek (np. swój mail — służy tylko do alertów)
6. **Network Configuration** →
   - Management Interface: wybierz kartę Ethernet (nie WiFi!)
   - Hostname: `pve.local` (lub inna nazwa, np. `smarthome.local`)
   - IP Address: zostaw co podpowiedział (DHCP) — później ustawimy stałe IP w routerze
   - Gateway: adres routera (zwykle `192.168.1.1` lub `192.168.0.1`)
   - DNS: `8.8.8.8` lub adres routera
7. **Summary** → sprawdź podsumowanie i kliknij `Install`

Instalacja trwa ok. 5-10 minut. Po zakończeniu komputerek się zrestartuje.

### Krok 4.3 — Po restarcie

**Wyjmij pendrive!** Inaczej znów uruchomi się instalator.

Po starcie zobaczysz na ekranie:
```
Welcome to the Proxmox Virtual Environment. Please use your web browser to
configure this server - connect to:

  https://192.168.1.XXX:8006/
```

**Zapisz ten adres IP** — to jest adres Twojego serwera Proxmox.

---

## 5. Pierwsze logowanie do panelu webowego

1. Na Macu otwórz przeglądarkę
2. Wpisz adres z ekranu komputerka: `https://192.168.1.XXX:8006`
3. Przeglądarka pokaże ostrzeżenie o certyfikacie — to normalne, kliknij "Zaawansowane" → "Przejdź mimo to"
4. Zaloguj się:
   - User: `root`
   - Password: hasło ustawione podczas instalacji
   - Realm: `Linux PAM`
5. Wyskakujące okienko o subskrypcji — kliknij OK (ignoruj, Proxmox działa bez płatnej licencji)

Powinieneś zobaczyć panel Proxmox z Twoim serwerem po lewej stronie.

---

## 6. Konfiguracja po instalacji

### 6.1 — Wyłączenie komunikatu o subskrypcji (opcjonalne)

To tylko kosmetyczna zmiana — wyłącza irytujące okienko przy logowaniu.

Przez SSH lub Shell w panelu webowym (serwer → Shell):
```bash
sed -Ei.bak "s/NotFound/Active/g" /usr/share/javascript/proxmox-widget-toolkit/proxmoxlib.js
systemctl restart pveproxy
```

### 6.2 — Dodanie darmowych repozytoriów

Proxmox domyślnie ma włączone repo enterprise (płatne). Trzeba je podmienić na darmowe.

```bash
# Wyłącz repo enterprise
sed -i 's/^deb/# deb/' /etc/apt/sources.list.d/pve-enterprise.list

# Dodaj darmowe repo
echo "deb http://download.proxmox.com/debian/pve bookworm pve-no-subscription" > /etc/apt/sources.list.d/pve-no-subscription.list

# Dodaj darmowe repo dla Ceph (jeśli plik istnieje)
if [ -f /etc/apt/sources.list.d/ceph.list ]; then
  sed -i 's/^deb/# deb/' /etc/apt/sources.list.d/ceph.list
fi
```

### 6.3 — Aktualizacja systemu

```bash
apt update && apt full-upgrade -y
reboot
```

Po restarcie zaloguj się ponownie do panelu.

---

## 7. Ustawienie stałego IP

Żeby IP komputerka się nie zmieniało po restarcie routera, ustaw **static lease** w routerze:

1. Zaloguj się do panelu routera (zwykle `192.168.1.1` w przeglądarce)
2. Znajdź sekcję DHCP / LAN / Address Reservation
3. Przypisz adres IP do adresu MAC komputerka
   - Adres MAC znajdziesz w Proxmox: serwer → Network → `vmbr0`
4. Zapisz i zrestartuj router

Od teraz komputerek zawsze dostanie ten sam IP.

---

## 8. Tworzenie pierwszego snapshota

To nie dotyczy samego Proxmox (host), ale VM-ek które postawisz. Zasada:

**Przed każdą większą zmianą w VM → zrób snapshot.**

W panelu webowym:
1. Kliknij VM po lewej stronie
2. Zakładka `Snapshots`
3. `Take Snapshot`
4. Nazwij np. `przed-zmiana-zigbee`
5. OK

Cofanie: kliknij snapshot → `Rollback` → potwierdź.

---

## 9. Połączenie SSH z Maca

Po instalacji SSH jest domyślnie włączone. Z terminala Maca:

```bash
ssh root@192.168.1.XXX
```

Wpisz hasło root i jesteś na serwerze.

### Ułatwienie — klucz SSH (żeby nie wpisywać hasła)

Na Macu:
```bash
# Jeśli nie masz jeszcze klucza SSH:
ssh-keygen -t ed25519

# Skopiuj klucz na serwer:
ssh-copy-id root@192.168.1.XXX
```

Od teraz `ssh root@192.168.1.XXX` łączy bez hasła.

### Ułatwienie — alias w SSH config

Dodaj do `~/.ssh/config` na Macu:
```
Host pve
    HostName 192.168.1.XXX
    User root
```

Teraz wystarczy wpisać:
```bash
ssh pve
```

---

## 10. Rozwiązywanie problemów

### Nie mogę wejść na panel webowy
- Sprawdź czy Mac i GMKtec są w tej samej sieci (ten sam router)
- Sprawdź czy wpisujesz `https://` (nie `http://`)
- Sprawdź czy port `:8006` jest w adresie
- Spróbuj `ping 192.168.1.XXX` z Maca

### Komputerek nie bootuje z pendrive'a
- Spróbuj inny klawisz: F2, F7, F10, F12, DEL
- W BIOS-ie wyłącz Secure Boot
- Sprawdź czy pendrive jest poprawnie nagrany (spróbuj nagrać jeszcze raz)

### Nie widzę karty sieciowej podczas instalacji
- GMKtec G3 z N100 powinien być wspierany out-of-the-box
- Upewnij się, że kabel Ethernet jest podłączony

### Zapomniałem hasła root
- Uruchom z pendrive'a instalacyjnego
- Wybierz "Advanced Options" → "Rescue Boot"
- Zamontuj dysk i zresetuj hasło przez `passwd`

---

## Co dalej?

Po ukończeniu tego tutoriala masz działający Proxmox. Następny krok:
→ **Instalacja Home Assistant OS jako VM** (osobny tutorial)
