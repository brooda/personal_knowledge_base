# Claude Code — Integracja ze Slackiem

Dwie opcje integracji Claude Code ze Slackiem.

---

## 1. Claude Code w Slacku (oficjalna integracja)

**Jak to dziala:**
Piszesz na Slacku `@Claude zrob refactor auth middleware` — Claude rozpoznaje ze to coding task, tworzy sesje Claude Code na webie (claude.ai/code), i odsyla na Slacka link + statusy.

**Setup:**
1. Admin instaluje appke Claude ze Slack Marketplace
2. Kazdy user laczy swoje konto Claude w zakladce App Home w Slacku
3. Dodajesz Claude'a do kanalow: `/invite @Claude`
4. Wybierasz tryb routingu:
   - **Code only** — wszystkie wzmianki ida do Claude Code
   - **Code + Chat** — Claude sam decyduje czy to coding task (-> Code) czy zwykle pytanie (-> Chat)

**Co potrafi:**
- Zbiera kontekst z watku/kanalu Slacka i przekazuje do sesji
- Posty ze statusami na Slacku (started, in progress, done)
- Przyciski: "View Session", "Create PR", "Change Repo"
- Dziala z repozytoriami GitHub

**Ograniczenia:**
- Wymaga planu Claude Pro/Max/Teams/Enterprise
- Tylko GitHub (nie GitLab/Bitbucket)
- Sesja dziala na webie — nie w lokalnym CLI
- Nie ma dostepu do lokalnego srodowiska (env vars, .env, lokalne pliki)

---

## 2. Slack MCP Server (z poziomu CLI)

**Jak to dziala:**
Konfigurujesz MCP server w Claude Code, ktory daje mu narzedzia do interakcji ze Slackiem. Potem z CLI mozesz mowic np. "wyslij na #dev-updates ze logging jest gotowy".

**Setup:**
1. Tworzysz Slack App w api.slack.com z odpowiednimi OAuth scopes (`chat:write`, `channels:read`, `search:read` itd.)
2. Dostajesz Bot Token (`xoxb-...`)
3. Konfigurujesz MCP server w `.claude/settings.json`:

```json
{
  "mcpServers": {
    "slack": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-slack"],
      "env": {
        "SLACK_BOT_TOKEN": "xoxb-your-token"
      }
    }
  }
}
```

**Co potrafi:**
- Wysylanie wiadomosci na kanaly/DM
- Szukanie w wiadomosciach
- Czytanie historii kanalow
- Zarzadzanie canvasami
- Wszystko z poziomu lokalnego CLI — pelen dostep do repo

**Ograniczenia:**
- Musisz sam skonfigurowac Slack App + permissions
- Token trzymasz lokalnie (bezpieczenstwo na Twojej glowie)
- To community/third-party MCP server — nie oficjalny Anthropic

---

## Kiedy co?

| Scenariusz | Opcja |
|---|---|
| Zlecanie taskow z poziomu Slacka | 1 (oficjalna) |
| Wysylanie notyfikacji/statusow na Slacka z CLI | 2 (MCP Server) |
| Oba naraz | mozna laczyc |

Data notatki: 2026-03-27
