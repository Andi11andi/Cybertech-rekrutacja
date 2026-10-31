# Cybertech LLM Zadania Rekrutacyjne

Repository zawiera rozwiązania zadań rekrutacyjnych z zakresu modeli LLM (Inference oraz Fine-tuning) dla koła naukowego Cybertech na Politechnice Wrocławskiej.

---

## Zadanie 1: Wpływ parametru Temperature na generowanie tekstu (Inference)

### 1. Wybór modelu
Do eksperymentu wybrano **`Qwen/Qwen2.5-3B-Instruct`**. Jako że oficjalna linia Qwen 2.5 nie posiada wariantu dokładnie 2.0B, model 3B stanowi najlepszą reprezentację klasy 2B, działając wydajnie w ramach pamięci VRAM GPU NVIDIA Tesla T4 w Google Colab (~6 GB VRAM).

### 2. Wyniki eksperymentu
Przetestowano zachowanie modelu dla czterech wartości temperatury ($T$):

| Temperatura ($T$) | Tryb dekodowania | Obserwowane zachowanie modelu |
| :--- | :--- | :--- |
| **0.0** | Greedy Search | **Precyzyjny i deterministyczny**: Najwyższa zgodność logiczna i brak losowości. |
| **1.0** | Standard Sampling | **Naturalny i konwersacyjny**: Płynna odpowiedź, przypominająca ludzki styl. |
| **10.0** | High-Entropy | **Szum i błędy**: Złamanie spójności, utykanie w powtórzeniach pod-słów. |
| **1000.0** | Uniform Limit | **Absurdalna struktura**: Losowy wybór poprawnych słów ze słownika ($P \approx 1/|V|$). |

---

## Zadanie 2: Fine-tuning z użyciem PEFT / LoRA

*(Sekcja zostanie uzupełniona po przeprowadzeniu procesu doedukowania modelu)*# Cybertech-rekrutacja
