# Prywatna baza wiedzy na plikach Markdown

## Problem
Szukam narzędzia do prywatnej knowledge base opartej na plikach `.md`, z dobrą apką mobilną.

## Narzędzia — pliki MD + mobile

### Obsidian
- Najpopularniejsze, darmowe do użytku prywatnego
- Pliki `.md` w folderze, linkowanie `[[link]]`, graf powiązań
- Sync między urządzeniami: płatny (Obsidian Sync) lub za darmo przez Git/iCloud/Dropbox
- Plugin **Remotely Save** — sync przez OneDrive/S3/WebDAV za darmo
- **Apka mobilna** — działa, ale toporна i mało dopracowana

### Joplin
- Open source, pliki Markdown, szyfrowane
- Sync przez Dropbox/OneDrive/WebDAV (za darmo)
- Apka mobilna na iOS i Android — OK, nie piękna ale funkcjonalna
- **Najlepszy kompromis** jeśli priorytet to pliki MD + dobry mobile

### Foam
- Rozszerzenie do VS Code, wiki w Markdown z linkami i grafem
- Darmowe, open source
- Brak natywnej apki mobilnej

### Logseq
- Podobne do Obsidian, bardziej "outliner" (jak Roam)
- Oparte na plikach `.md`

## Narzędzia — dobry mobile, ale nie surowe MD

### Notion
- Świetna apka mobilna
- Pliki w chmurze Notion (eksport do MD możliwy, ale nie natywne pliki)
- Darmowe do użytku prywatnego

### Craft
- Bardzo dopracowana apka na iOS/Mac
- Eksport do MD, ale natywny format to nie MD

### Anytype
- Ładna apka mobilna, offline-first
- Własny format (nie surowe MD)

## Generatory stron z MD (do repo Git)
- **MkDocs** — generuje stronę z `.md`, trzymasz w repo
- **Docusaurus** — jak MkDocs, ale w React
- **mdBook** — lekki generator od Rusta

## GitHub Wiki
- Prywatne wiki **niedostępne** na darmowym planie GitHub (tylko publiczne repo lub plan płatny)
- Alternatywa: katalog `docs/` w repo

## Podsumowanie
- Priorytet mobile → **Joplin** lub **Notion**
- Priorytet pliki MD + ekosystem pluginów → **Obsidian**
- Już używasz VS Code → **Foam**
