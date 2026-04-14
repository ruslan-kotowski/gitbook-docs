---
title: Dzienniki interakcji z AI (wersja beta)
article_id: 34049604547858
translation_id: 34049604547858
locale: pl-pl
sidebar_position: 1
created_at: '2026-03-15T21:28:41Z'
updated_at: '2026-03-16T09:09:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dzienniki interakcji z AI umożliwiają administratorom z dodatkiem Enterprise Guard zbieranie i przeglądanie zapisów dotyczących korzystania z Miro AI w całej organizacji. Włączając dzienniki interakcji z AI, administratorzy mogą zapewnić zespołom ds. bezpieczeństwa, zgodności i zarządzania większą widoczność sposobu korzystania z funkcji AI oraz tego, jakie informacje są przetwarzane przez systemy AI.

Dzienniki interakcji z AI pomagają organizacjom:

- Monitorować użycie funkcji AI w organizacji
- Wspierać przeglądy zarządzania, zgodności i bezpieczeństwa
- Zapewniać widoczność informacji udostępnianych systemom AI
- Wzmacniać zaufanie i odpowiedzialne przyjmowanie narzędzi AI

Dzienniki interakcji z AI rejestrują zapisy interakcji między użytkownikami a funkcjami opartymi na AI w Miro. Zapisy te pomagają organizacjom przeglądać, jak AI jest używane w organizacji, oraz wspierać procesy audytu wewnętrznego, zgodności i nadzoru.

Gdy dzienniki interakcji z AI są włączone, rejestrują:

- Prompty użytkowników przesyłane do funkcji AI
- Odpowiedzi generowane przez AI zwracane przez system
- Kontekst systemu związany z interakcją

## Zanim zaczniesz

- Musisz być administratorem, aby włączyć lub skonfigurować dzienniki interakcji z AI.
- Wymagany jest dodatek Enterprise Guard, aby używać tej funkcji.
- Dzienniki interakcji z AI muszą być włączone, zanim rozpoczniemy zbieranie danych.
- Tylko interakcje, które wystąpią po włączeniu logowania, zostaną zarejestrowane.

## Włącz dzienniki interakcji z AI

1. Przejdź do **Konsoli administratora**.
2. Wybierz **Bezpieczeństwo**.
3. Kliknij **Dzienniki audytu**.
4. Otwórz kartę **Ustawienia**.
5. W sekcji **Dzienniki interakcji AI**, włącz **Zbieranie dzienników interakcji AI**.
6. Wybierz **okres retencji**.
7. Zapisz zmiany.

Po włączeniu tego ustawienia, Miro zaczyna zbierać dzienniki interakcji AI dla nowych interakcji AI.

## Konfiguracja retencji dzienników

Administratorzy mogą skonfigurować, jak długo dzienniki interakcji z AI są przechowywane.

1. Przejdź do **konsoli administratora > Bezpieczeństwo > Dzienniki audytu**.
2. W sekcji **dzienniki interakcji z AI** wybierz preferowany **okres retencji**.
3. Zapisz zmiany.

Dzienniki są automatycznie usuwane, gdy upływa skonfigurowany okres retencji.

## Dostęp do dzienników interakcji z AI przez API

Dzienniki interakcji z AI można pobierać za pomocą API dzienników interakcji z AI.

To pozwala organizacjom eksportować i analizować dane z interakcji z AI za pomocą istniejących systemów zgodności, zgodności lub monitoringu bezpieczeństwa.

Typowe przypadki użycia obejmują:

- Zarządzanie i nadzór nad AI
- Monitorowanie bezpieczeństwa
- Audyt zgodności
- Wewnętrzne dochodzenia

Aby uzyskać więcej informacji, zobacz [dokumentację dla deweloperów](https://developers.miro.com/reference/enterprise-get-ai-interaction-logs).

## Ograniczenia

Obecne wydanie obejmuje początkową wersję logowania interakcji AI. Występują następujące ograniczenia:

- Przywołania narzędzi z funkcji AI nie są obecnie rejestrowane.
- Interakcje związane z integracjami Miro MCP nie są obecnie rejestrowane.
- Zdarzenia moderacji i blokady wrażliwych promptów nie są obecnie rejestrowane.
- Obrazy nie są uwzględniane w dziennikach interakcji AI.
