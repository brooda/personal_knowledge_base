# Smart Home — Plan uruchomienia

## Architektura docelowa

```
GMKtec G3 (N100)
  └─ Proxmox VE (hypervisor, darmowy)
       ├─ VM: Home Assistant OS  ← główny "mózg" smart home
       │    └─ SONOFF Zigbee Dongle (USB passthrough)
       │         ├─ żarówki Ewelink GU10
       │         └─ rolety Zigbee
       └─ (opcjonalnie inne VM/kontenery w przyszłości)
```

## Po co Proxmox?

Kolega dobrze radzi. Proxmox to darmowy hypervisor (jak VMware, ale open source). Dzięki niemu:
- Stawiasz Home Assistant jako osobną maszynę wirtualną
- Możesz łatwo robić snapshoty/backupy (zepsułeś coś → cofasz w 10 sekund)
- W przyszłości możesz dodać inne usługi (Pi-hole, NAS, monitoring) bez kupowania nowego sprzętu
- N100 spokojnie to udźwignie — jest energooszczędny i wystarczająco mocny

## Kroki — krok po kroku

### Etap 1: Przygotowanie mini PC
- [ ] Zrobić backup danych z Windows jeśli są potrzebne
- [ ] Pobrać Proxmox VE ISO: https://www.proxmox.com/en/downloads
- [ ] Nagrać ISO na pendrive (np. Rufus lub balenaEtcher)
- [ ] Zainstalować Proxmox na GMKtec G3 (zastąpi Windows)
- [ ] Po instalacji wejść na panel webowy Proxmox: `https://<ip-komputerka>:8006`

### Etap 2: Instalacja Home Assistant na Proxmox
- [ ] Pobrać oficjalny skrypt instalacji HA na Proxmox z: https://community-scripts.github.io/ProxmoxVE/
- [ ] Uruchomić skrypt — stworzy VM z Home Assistant OS automatycznie
- [ ] Przekazać SONOFF Zigbee Dongle do VM (USB passthrough w Proxmox)
- [ ] Uruchomić VM i wejść na Home Assistant: `http://<ip-ha>:8123`
- [ ] Przejść kreator pierwszej konfiguracji (konto, lokalizacja, itp.)

### Etap 3: Konfiguracja Zigbee
- [ ] W Home Assistant dodać integrację **ZHA** (Zigbee Home Automation)
- [ ] ZHA powinno wykryć dongle SONOFF automatycznie
- [ ] Sparować żarówki Ewelink GU10 (tryb parowania → dodaj urządzenie w ZHA)
- [ ] Sparować rolety Zigbee (analogicznie)

### Etap 4: Pierwsze automatyzacje
- [ ] Stworzyć dashboard z kontrolą świateł i rolet

#### Pomysły na automatyzacje

1. **Rolety na zachód/wschód słońca**
   Rolety zamykają się automatycznie o zachodzie słońca i otwierają o wschodzie. Home Assistant ma wbudowane dane astronomiczne — wystarczy ustawić lokalizację domu, a HA sam oblicza godziny wschodu i zachodu każdego dnia. Nie trzeba ręcznie zmieniać godzin sezonowo. Można dodać offset, np. zamknij 30 min po zachodzie, żeby jeszcze złapać ostatnie światło dzienne. Trigger: `sun.sun` → state `below_horizon` / `above_horizon`.

2. **Światło powitalne**
   Gdy wracasz do domu, żarówki automatycznie zapalają się ciepłą bielą. Trigger: telefon łączy się z domowym WiFi (Home Assistant wykrywa to przez aplikację mobilną HA Companion — darmowa na iOS/Android). Można ustawić warunek: tylko po zmroku (bo w dzień nie ma sensu zapalać). Można też dodać opóźnienie 1-2 min, żeby światło się zapaliło kiedy już wchodzisz do mieszkania, a nie gdy parkujesz.

3. **Tryb nocny**
   O ustalonej godzinie (np. 23:00) wszystkie światła gasną, rolety się zamykają. Działa jako "wyłącznik generalny" — nie musisz pamiętać czy zgasiłeś wszystko. Można to też powiązać z przyciskiem fizycznym przy łóżku (Zigbee button — do dokupienia) albo z komendą głosową "dobranoc". Warto dodać warunek: jeśli światło w salonie jest jeszcze włączone po 23:30, wyślij powiadomienie na telefon zamiast od razu gasić.

4. **Symulacja obecności (wakacje)**
   Gdy wyjeżdżasz, włączasz tryb "away" w HA. Od tego momentu system losowo włącza i wyłącza światła wieczorem (np. między 18:00 a 23:00), a rolety pracują normalnie jak co dzień. Z zewnątrz wygląda to jakby ktoś był w domu. Losowość jest kluczowa — stały schemat (światło zawsze o 19:00) jest podejrzany. HA ma do tego gotowy blueprint "Presence Simulation". Można aktywować ręcznie lub automatycznie gdy HA wykryje, że wszystkie telefony domowników są poza domem przez X godzin.

5. **Pobudka światłem (sunrise alarm)**
   15-30 minut przed budzikiem żarówki powoli rozjaśniają się od zera do ciepłej bieli, symulując wschód słońca. Rolety zaczynają się otwierać. Ciało zaczyna produkować kortyzol w reakcji na światło, więc budzenie jest łagodniejsze niż nagły alarm. W HA robi się to przez automatyzację z akcją `light.turn_on` z parametrem `transition: 900` (900 sekund = 15 min płynnego rozjaśniania). Trigger: czas, np. 6:15 w dni robocze. Można powiązać z alarmem telefonu przez HA Companion.

6. **Tryb kino**
   Jednym przyciskiem lub komendą głosową: rolety zjeżdżają w dół, światła przyciemniają się do 10% w ciepłym bursztynowym kolorze. Idealne przed filmem. W HA tworzy się to jako "scenę" (Scene) — zapisujesz dokładny stan wszystkich urządzeń i potem odtwarzasz jednym kliknięciem. Żeby wrócić do normalności, robisz drugą scenę "normalny" i przełączasz między nimi. Fajnie działa z pilotem Zigbee (np. IKEA TRADFRI remote) — jeden przycisk = kino, drugi = normalnie.

## Wskazówki

- **Nie resetuj żarówek/rolet z apki Tuya/Ewelink** — jak je sparujesz z ZHA, będą działać lokalnie bez chmury
- **Rób snapshoty w Proxmox** przed każdą większą zmianą
- **Zigbee mesh** — im więcej urządzeń Zigbee (zwłaszcza zasilanych z gniazdka, np. żarówki), tym lepsza sieć — działają jako repeatery
