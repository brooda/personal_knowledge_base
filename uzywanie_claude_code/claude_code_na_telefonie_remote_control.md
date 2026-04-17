# Claude Code na telefonie — Remote Control

Od lutego 2026 Anthropic ma oficjalną funkcję **Remote Control**, która pozwala przejąć sesję Claude Code z komputera na telefon. Działa z `claude.ai/code` i aplikacją mobilną Claude na iOS i Android.

## Jak to działa

Claude Code nadal działa **lokalnie** na komputerze — pliki, konfiguracja MCP, serwery, wszystko zostaje u mnie. Przez chmurę Anthropic przechodzą tylko wiadomości i wyniki narzędzi. Telefon jest "drugim ekranem" do tej samej sesji.

## Konfiguracja

1. Zainstalować aplikację Claude na telefonie. W aktywnej sesji Claude Code można wpisać `/mobile` — pokaże się kod QR do pobrania aplikacji.
2. W terminalu w aktywnej sesji wpisać `/rc` (lub `/remote-control`, albo uruchomić `claude remote-control`). Pojawi się kod QR.
3. Zeskanować go aplikacją Claude na telefonie — gotowe, pełny dostęp do sesji.

## Rzeczy, o których warto wiedzieć

- **Terminal na komputerze musi pozostać otwarty** — jeśli proces się zamknie, sesja zdalna też. Warto owinąć to w `tmux` albo `screen`, żeby proces przeżył nawet zamknięcie okna terminala.
- Remote Control jest dostępne na wszystkich planach, ale na **Team i Enterprise jest domyślnie wyłączone** — admin musi je włączyć w ustawieniach.
- **Powiadomienia push** (np. gdy długie zadanie się skończy) wymagają Claude Code w wersji **2.1.110 lub nowszej**.
- W aplikacji sesje Remote Control są oznaczone **ikoną komputera z zieloną kropką**, gdy są online.

## Alternatywa bez własnego komputera

Można użyć Claude Code w przeglądarce przez `claude.ai/code`. Wtedy sesja wykonuje się w chmurze Anthropic, więc nie potrzeba lokalnej konfiguracji — ale tracę dostęp do **swoich lokalnych MCP, plików i narzędzi**. Dobre, gdy chcę szybko odpalić coś w repo, którego nie mam sklonowanego, lub uruchomić kilka zadań równolegle.

## Dla mnie (Notion MCP)

Ponieważ pracuję nad połączeniem Claude Code z Notion przez MCP — **opcja z Remote Control jest lepsza**, bo lokalne serwery MCP (w tym Notion) pozostają dostępne w sesji sterowanej z telefonu.
