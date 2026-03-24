# Integracja przepisów z Fitatu

---

## Problem
Mam przepisy z Rozkosznego i chcę je śledzić w Fitatu (kalorie, makro), ale nie ma automatycznego importu.

---

## Opcje

### 1. Fitatu Premium — ręczne dodawanie przepisu (najlepsza opcja)
- W apce: **Przepisy → Dodaj przepis**
- Wpisujesz nazwę, liczbę porcji
- Dodajesz składniki jeden po jednym (Fitatu ma bazę produktów)
- Apka oblicza makro automatycznie
- Potem logujesz posiłek jednym kliknięciem: "Zjadłem 1 porcję X"
- **Wysiłek:** ~5 min na przepis, ale robisz to raz

### 2. Fitatu Premium — skan z URL
- Fitatu potrafi zaimportować składniki z linku do przepisu online
- Jeśli przepis z Rozkosznego jest na blogu/stronie — wklej URL
- Apka spróbuje wyciągnąć składniki automatycznie
- Często wymaga korekty, ale oszczędza czas

### 3. Fitatu Premium — skan ze zdjęcia
- Zrób zdjęcie listy składników z książki
- Fitatu rozpoznaje tekst (OCR) i próbuje dopasować produkty
- Dokładność bywa różna

### 4. Skrypt / automatyzacja (zaawansowane)
- Fitatu **nie ma publicznego API** — bezpośredni import niemożliwy
- Alternatywa: użyć bazy **Open Food Facts** (darmowa, open source) do obliczenia makro
- Można napisać skrypt parsujący pliki .md z przepisami → obliczający wartości odżywcze
- Wynik: tabela makro dla każdego przepisu, ale bez integracji z Fitatu

---

## Rekomendacja

**Na start:** Fitatu Premium + ręczne dodawanie przepisów. Robisz to raz na przepis, potem logujesz jednym kliknięciem. Przy 31 przepisach z Rozkosznego to ~2-3h pracy jednorazowej.

**Tip:** Dodawaj przepisy na bieżąco — gdy gotujesz dany przepis, dodaj go przy okazji do Fitatu.

---

## Status

- [ ] Sprawdzić czy Fitatu Premium jest wart ceny
- [ ] Dodać pierwsze 5 przepisów testowo
- [ ] Ocenić czy skan z URL działa z blogiem Rozkosznego
