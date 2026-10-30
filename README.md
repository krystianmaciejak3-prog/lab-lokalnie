# Laboratorium lokalnego modelu AI

## Cel projektu
Celem ćwiczenia było uruchomienie lokalnego modelu AI, sprawdzenie jego szybkości, jakości odpowiedzi i zasad ochrony danych.

## Wykorzystane narzędzia
- System: Windows 11
- Program: Ollama
- Model: Qwen2.5 1.5B (`qwen2.5:1.5b`)
- Edytor: Visual Studio Code

## Pomiar szybkości
Model został uruchomiony na moim komputerze przez Ollama.
- Szybkość generowania: 123,10 tokenów/s
- Czas całkowity: 2,31 s
- Liczba wygenerowanych tokenów: 258
- Szybkość przetwarzania promptu: 117,97 tokenów/s

Wyniki pochodzą z jednego pomiaru poleceniem `ollama run qwen2.5:1.5b --verbose`.

## Zauważone błędy
Podczas pierwszego testu model wstawił chińskie znaki do polskiego tekstu i użył niepoprawnego określenia „urządzenie specyficzowe”. Podczas kolejnego testu mieszał język polski z angielskim i nieprecyzyjnie opisał cykl pracy sterownika PLC.

Wniosek: model odpowiadał szybko, ale jego odpowiedzi wymagają sprawdzania.

## Dlaczego wybrałem model lokalny?
Model uruchomiłem lokalnie, aby mieć większą kontrolę nad danymi. Testowane pytania były przetwarzane na moim komputerze, bez konieczności wysyłania ich do chmurowego modelu AI. Nie używałem w testach prawdziwych danych osobowych ani kluczy API.

## Bezpieczeństwo projektu
Przed publikacją sprawdzę pliki i historię Git pod kątem kluczy API, haseł oraz danych osobowych. Przeprowadzę również przegląd skillem `przeglad-bezpieczenstwa` z lekcji 7.

## Wnioski
Lokalny model AI może być przydatny do nauki i eksperymentów. Jego zaletą jest możliwość pracy na własnym komputerze, ale należy sprawdzać poprawność generowanych informacji.