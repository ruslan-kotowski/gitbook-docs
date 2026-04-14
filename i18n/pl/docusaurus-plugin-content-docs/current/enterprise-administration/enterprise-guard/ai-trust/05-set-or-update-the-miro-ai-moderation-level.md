---
title: Ustawienie lub aktualizacja poziomu moderacji w Miro AI (wersja beta)
article_id: 30613174297618
translation_id: 30613174297618
locale: pl-pl
sidebar_position: 3
created_at: '2025-10-29T01:15:35Z'
updated_at: '2026-01-12T11:22:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dzięki moderacji Miro AI, administratorzy firmy mogą dostosować poziomy filtrowania promptów, które mogą prowadzić do potencjalnie szkodliwych lub nieodpowiednich wyników. Możesz kontrolować czułość moderacji Miro AI w całej swojej organizacji i filtrować w kategoriach takich jak nienawiść, treści seksualne, przemoc i samookaleczenia. Pomaga to dopasować korzystanie z Miro AI do wymagań, zasad i tolerancji ryzyka Twojej organizacji.

**Uwaga**: Jeśli Twoja organizacja łączy się z własnym dostawcą LLM (na przykład bezpośrednią integracją OpenAI), selektor moderacji jest wyłączony i wszelkie wcześniej wybrane poziomy są ignorowane dla tej integracji.

## Wymagania wstępne

- Upewnij się, że masz dodatek Enterprise Guard.
- Upewnij się, że jesteś **Administratorem Firmy** dla organizacji, którą chcesz skonfigurować.
- Przejrzyj swoje wymagania dotyczące zarządzania i zasad, aby wybrać odpowiedni początkowy poziom. Domyślny jest zalecany dla większości organizacji.

## Ustaw lub zaktualizuj poziom moderacji Miro AI

1. Otwórz **Ustawienia** swojej organizacji w Miro.
2. Przejdź do **Miro AI** › **Moderacja**.
3. Wybierz poziom moderacji:
   - **Surowy:** Blokuje wszystko, co w poziomie Domyślnym, plus zawartość o niskim do umiarkowanego ryzyka (na przykład subtelna lub zakodowana nienawiść, treści o sugestywnym charakterze seksualnym, niegraficzna przemoc, niejawne wzmianki o samookaleczeniach).
   - **Domyślny (zalecany):** Blokuje treści umiarkowanie do poważnie szkodliwych (na przykład jawna nienawiść, jawne treści seksualne, drastyczna przemoc, zachęcanie do samookaleczeń).
   - **Minimalny:** Blokuje jedynie poważnie szkodliwe treści.
4. Kliknij **Potwierdź**.
   Zmiana zostanie natychmiast zastosowana dla wszystkich w organizacji i zostanie zapisana w dzienniku audytu.

## Zatwierdź poziom moderacji (opcjonalnie)

- Poproś grupę pilotażową o testowanie typowych promptów i zgłaszanie nadmiernej lub niedostatecznej filtracji.
- Monitoruj kanały pomocy lub eskalacji w celu wykrycia fałszywych pozytywów lub pominiętych szkód w pierwszym tygodniu po zmianie.

## Wskazówki i najlepsze praktyki

- Rozpocznij od **Default**, a następnie dostosuj na podstawie opinii pilotów i przeglądów eskalacji.
- Jeśli użytkownicy zgłaszają zbyt wiele zablokowanych promptów, spróbuj **Default** (z Strict) lub **Minimal** (z Default) i opublikuj przykłady akceptowalnych promptów.
- Jeśli graniczne treści prześlizgują się, przejdź do **Strict** i dodaj wewnętrzne wskazówki, aby zmniejszyć tarcia.
- Ponownie przemyśl poziom po zmianach w zasadach, regulacjach lub przypadkach użycia.

## Rozwiązywanie problemów

**Kontrola moderacji jest wyłączona**
Połączona jest niestandardowa integracja LLM. Odłącz ją, aby ponownie włączyć selektor. Gdy jest połączona, każdy wcześniej wybrany poziom jest ignorowany dla tej integracji.

**Zbyt wiele fałszywych alarmów**
Rozważ zmianę **z Surowe na Domyślne** i udostępnij przykłady akceptowalnego użycia. Przejrzyj dziennik audytu, aby potwierdzić czas wprowadzenia zmian.

**Ekspozycja na szkodliwe treści**
Upewnij się, że poziom nie jest **Minimalny**. Rozważ **Domyślny** lub **Surowy**, w zależności od tolerancji na ryzyko.

**Użytkownicy nie wiedzą, dlaczego prompty są blokowane**
Opublikuj wewnętrzne wytyczne dotyczące wybranego poziomu, przykładowych promptów i ścieżek eskalacji.
