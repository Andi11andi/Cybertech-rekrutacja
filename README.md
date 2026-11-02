# Cybertech LLM Zadania Rekrutacyjne

Repozytorium zawiera rozwiązania zadań rekrutacyjnych z zakresu dużych modeli językowych (LLM), przygotowane w ramach rekrutacji do koła naukowego Cybertech na Politechnice Wrocławskiej.

## Zadanie 1: Wpływ parametru Temperature na generowanie tekstu

Eksperyment bada wpływ wartości parametru `temperature` na odpowiedzi modelu językowego.

- Model: `Qwen/Qwen3.5-2B`
- Framework: MS Swift
- Środowisko: Kaggle Notebook
- GPU: NVIDIA Tesla T4

Szczegółowy opis eksperymentu, kod oraz wyniki znajdują się w pliku `Cyber_rek_Zadanie1.ipynb`.

## Zadanie 2: Fine-tuning modelu z użyciem LoRA

Zadanie obejmuje dostrojenie modelu językowego z wykorzystaniem techniki LoRA oraz ocenę jakości odpowiedzi przed i po fine-tuningu.

- Model: `Qwen/Qwen3.5-2B`
- Dataset: `medalpaca/medical_meadow_wikidoc_patient_information`
- Framework: MS Swift
- Metoda dostrajania: LoRA
- Środowisko: Kaggle Notebook
- GPU: NVIDIA Tesla T4

Model został oceniony na tym samym zbiorze testowym przed i po dostrojeniu. Do porównania wykorzystano metryki ROUGE-1, ROUGE-2, ROUGE-L, BLEU oraz średnią długość generowanych odpowiedzi.

Szczegółowy opis eksperymentu, implementacja, analiza wyników oraz przykłady odpowiedzi znajdują się w pliku `Cyber_rek_Zadanie2.ipynb`.
