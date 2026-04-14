---
title: "Przegl\u0105d moderacji AI (wersja beta)"
article_id: 29491049430674
translation_id: 29491049430674
locale: pl-pl
sidebar_position: 2
created_at: '2025-09-15T16:27:59Z'
updated_at: '2026-01-12T11:21:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dzięki moderacji Miro AI, administratorzy firmy mogą dostosować poziomy filtrowania promptów, które mogą zawierać potencjalnie szkodliwy lub nieodpowiedni tekst. Możesz ustawić organizacyjny poziom czułości na moderację Miro AI, aby filtrować treści, takie jak mowa nienawiści, treści seksualne, przemoc i samookaleczenia. Pomaga to dostosować użycie Miro AI do wymagań, zasad i poziomu tolerancji ryzyka twojej organizacji.

:::note
*Jeśli twoja organizacja łączy własnego dostawcę LLM (na przykład bezpośrednią integrację z OpenAI), selektor moderacji jest wyłączony, a wszelkie wcześniej wybrane poziomy są ignorowane dla tej integracji.*
:::

## Poziomy moderacji

Zarządzaj treściami Miro AI w całej organizacji za pomocą moderacji Miro AI. Ustaw poziom filtrowania na Ścisłe, Domyślne lub Minimalne, aby określić, które komunikaty są blokowane. Przejrzyj poniższą tabelę, aby szybko porównać poziomy, a następnie zapoznaj się z szczegółowymi sekcjami, aby uzyskać więcej wskazówek.

| Poziom | Działanie | Najlepsze dla | Kompromisy |
| --- | --- | --- | --- |
| Ścisły | Blokuje Domyślne + treści o niskim do umiarkowanego poziomie ryzyka. | Silnie regulowane organizacje, edukacja. | Więcej fałszywie pozytywnych; możliwość nadmiernego filtrowania. |
| Domyślny (zalecany) | Blokuje umiarkowanie do poważnie szkodliwe treści. | Większość zastosowań biznesowych. | Niektóre treści graniczne mogą przechodzić. |
| Minimalny | Blokuje tylko poważnie szkodliwe treści. | Konteksty kreatywne, gamingowe, medialne. | Większa ekspozycja na niskiej do średniej szkodliwości treści. |

:::note
*Domyślny jest zalecany dla większości organizacji. Filtruje treści, które większość osób uważa za nieodpowiednie lub szkodliwe, zachowując przy tym szeroką użyteczność.*
:::

## Poziom restrykcyjny

### Co filtruje

Wszystko w poziomie domyślnym plus treści niosące niskie lub umiarkowane ryzyko (na przykład subtelne lub zakodowane mowy nienawiści, treści o podtekstach seksualnych, niewłamana przemoc, czy niejawne wzmianki o samookaleczeniach).

### Kiedy używać

- Branże regulowane lub polityki organizacji unikających ryzyka
- Programy edukacyjne lub skierowane do młodzieży
- Projekty pilotażowe z niską tolerancją ryzyka

### Kompromisy

- Więcej fałszywych alarmów i zablokowanych granicznych prób
- Wymaga wskazówek w celu zredukowania trudności użytkowników

## Poziom domyślny (zalecany)

### Co filtruje

Treści umiarkowanie do bardzo szkodliwe (jawna mowa nienawiści, jawne treści seksualne, brutalna przemoc, zachęcanie do samookaleczeń).

### Kiedy używać

- Większość organizacji poszukujących równowagi między bezpieczeństwem a użytecznością

### Wady

- Kontekstowe/graniczne prompty mogą przechodzić

## Minimalny poziom

### Co filtruje

Tylko bardzo szkodliwe treści.

### Kiedy używać

- Zespoły twórcze, które potrzebują szerszej swobody wyrazu (gry, media)
- Wewnętrzna ideacja z jasnymi ścieżkami eskalacji

### Wady

- Większa ekspozycja na treści od nisko do umiarkowanie szkodliwych w wynikach

## Audyt i zgodność

Zmiany poziomu moderacji są rejestrowane w dzienniku audytu organizacji, łącznie z poprzednią wartością, nową wartością, osobą, która dokonała zmiany, oraz czasem jej dokonania. Aby uzyskać więcej informacji, zapoznaj się z dokumentacją na temat [dzienników audytu](../security-management/01-audit-logs.md).

## Najlepsze praktyki

- Zacznij od ustawienia domyślnego, następnie dostosuj na podstawie opinii z pilotażu i przeglądów eskalacyjnych.
- Sparuj tryb Ścisły z jasnymi wytycznymi wewnętrznymi dotyczącymi akceptowalnych promptów, aby zredukować liczbę fałszywych alarmów.
- Jeżeli potrzebujesz trybu Minimalnego, zdefiniuj, kiedy zespoły powinny eskalować lub zgłaszać problematyczne wyniki.
- Przejrzyj swoje ustawienia po dużych aktualizacjach zasad lub regulacyjnych.

- Przegląd moderacji AI
- Poziomy moderacji
- Poziom restrykcyjny
- Poziom domyślny (zalecany)
- Poziom minimalny
- Audyt i zgodność
- Najlepsze praktyki
