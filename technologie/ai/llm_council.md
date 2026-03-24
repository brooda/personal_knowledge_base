# LLM Council — ewaluacja AI przez panel modeli

---

## Co to jest?

**LLM Council** to podejście, w którym **kilka różnych modeli LLM wspólnie ocenia** jakość odpowiedzi — zamiast polegania na jednym modelu jako sędzia. Agregacja wielu opinii redukuje biasy i daje oceny lepiej korelujące z ludzkimi preferencjami.

---

## Popularne platformy i narzędzia

### Publiczne leaderboardy i areny

| Platforma | URL | Opis |
|-----------|-----|------|
| **Chatbot Arena (LMSYS)** | chat.lmsys.org | Użytkownicy porównują modele w ślepym teście A/B. Ranking Elo. Złoty standard |
| **Open LLM Leaderboard** | HuggingFace | Automatyczne benchmarki dla modeli open source |
| **AlpacaEval** | tatsu-lab.github.io/alpaca_eval | LLM-as-a-judge z kontrolą długości odpowiedzi |
| **WildBench** | HuggingFace (Allen AI) | Trudne, realistyczne zapytania oceniane przez LLM |
| **MT-Bench** | Część FastChat (LMSYS) | 80 pytań wieloturowych, GPT-4 jako sędzia |
| **Artificial Analysis** | artificialanalysis.ai | Porównania jakości, szybkości i ceny modeli |

### Narzędzia open source (GitHub)

| Projekt | Opis |
|---------|------|
| **llm-council** | Framework do uruchamiania panelu LLM jako sędziów |
| **FastChat (LMSYS)** | Infrastruktura Chatbot Arena + moduł `llm_judge` |
| **DeepEval** | Framework do ewaluacji LLM z metrykami (faithfulness, hallucination) |
| **RAGAS** | Standard do ewaluacji pipeline'ów RAG |
| **Prometheus / Prometheus-2** | Open-source model wytrenowany specjalnie jako sędzia |
| **OpenAI Evals** | Framework od OpenAI z szablonami model-graded evaluations |

### Platformy komercyjne

| Platforma | Opis |
|-----------|------|
| **Patronus AI** | Enterprise — automatyczni sędziowie na halucynacje, toksyczność |
| **Braintrust** | Dev platform z LLM-as-a-judge scoring |
| **LangSmith (LangChain)** | Tracing + ewaluacja w ekosystemie LangChain |
| **Arize Phoenix** | Open-source observability + ewaluacja LLM |

---

## Kluczowe problemy i biasy

- **Position bias** — modele preferują pierwszą lub ostatnią odpowiedź. Rozwiązanie: testuj obie kolejności
- **Self-enhancement bias** — modele oceniają własne odpowiedzi wyżej. Rozwiązanie: panel z różnych modeli
- **Verbosity bias** — dłuższa odpowiedź = wyższa ocena. Rozwiązanie: kontrola długości (AlpacaEval 2.0)

---

## Ważne prace badawcze

| Paper | Rok | Wkład |
|-------|-----|-------|
| *Judging LLM-as-a-Judge (MT-Bench)* | 2023 | Fundamentalna praca — GPT-4 zgadza się z ludźmi w >80% |
| *LLM Council: Benchmarking with a Council of Judges* | 2024 | Panel różnych LLM zamiast jednego sędziego |
| *Prometheus / Prometheus 2* | 2023/24 | Open-source model sędziowski, niezależny od API |
| *Chatbot Arena* | 2024 | System Elo z 200K+ ludzkich głosów |

---

> **Moje przemyślenia:**
> *(tu wpisuj swoje notatki i obserwacje)*
