---
title: Jira OAuth 1.0 wycofany w Miro
article_id: 28738797627538
translation_id: 28739475088274
locale: pl-pl
sidebar_position: 13
created_at: '2025-08-13T12:34:21Z'
updated_at: '2025-10-20T14:48:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Osoby: administratorzy firmy Plany: Starter, Business, Enterprise, Education
    Platformy: przeglądarka, komputery biurkowe'
---

Autoryzacja Jira OAuth 1.0 jest wycofana od sierpnia 2025 r.

Jeśli Twoja organizacja już zaktualizowała się do Jira OAuth 2.0, możesz zignorować ten artykuł. Nie są wymagane działania od Twojego administratora firmy. Możesz zweryfikować ze swoim administratorem firmy, czy Wasza organizacja korzysta z OAuth 2.0.

:::warning
Jeśli Twoja organizacja nie zaktualizowała się do OAuth 2.0, wtedy może dojść do zakłóceń integracji Jira z Miro, w tym Jira Cloud, Server i Data Center.
:::

Tylko administratorzy firmy mogą zmieniać wersje zespołów w swojej organizacji.

W przypadku zakłócenia synchronizacja między Miro a Jira zostaje zatrzymana, aż Twoja organizacja zaktualizuje się do uwierzytelniania OAuth 2.0. Istniejące karty Jira pozostaną na Twoich tablicach Miro.

Zakłócenie oznacza, że import jest niedostępny i karty nie są aktualizowane, nie można załadować szczegółów, a tworzenie i aktualizowanie planera jest niedostępne.

Aby uniknąć zakłóceń, Miro zaleca, aby administrator(zy) firmy natychmiast zaktualizowali się do Jira OAuth 2.0.

:::tip
Administratorzy mogą sprawdzić swoją wersję OAuth.
:::

## Dlaczego OAuth 1.0 jest wycofany?

Atlassian wycofał protokół uwierzytelniania OAuth 1.0 i nie zapewnia dla niego wsparcia.

**Więcej informacji:** Zobacz (zewnętrzny) [OAuth 1.0a dla REST API (wycofany)](https://developer.atlassian.com/cloud/jira/platform/jira-rest-api-oauth-authentication/).

## Sprawdź swoją wersję OAuth

Jako administrator zespołu Enterprise lub administrator abonamentu Starter lub Business możesz sprawdzić, czy Twój zespół używa OAuth 1.0 czy OAuth 2.0.

Wykonaj te kroki:

1. Na pulpicie Miro kliknij swój awatar w prawym górnym rogu i wybierz **Konsola administracyjna**.
2. Przejdź do **Zespoły** > **[Nazwa zespołu]**.
3. Kliknij **Aplikacje**.
4. Znajdź i kliknij **Karty Jira**.
5. Przejdź do **Ustawienia administracyjne** > **Konfiguracja Jira**.
   Konfiguracja wskazuje, której wersji OAuth używa Twój zespół.
6. (Opcjonalnie) Powtórz kroki 1-5 dla innych zespołów, które chcesz zweryfikować.
7. Poinformuj swojego(-ich) administratora(-ów) firmy o zespołach niekorzystających z OAuth 2.0.

## Znajdź swojego administratora firmy

Aby zidentyfikować swoich administratorów firmy, wykonaj te kroki:

:::note
(Enterprise) Jeśli włączono ochronę prywatności zespołu, osobom nie będącym administratorami firmy wyświetlanie list członków nie jest możliwe.
:::

1. Przejdź do **Ustawień profilu zespołu** w Miro.
2. Otwórz stronę **Członkowie**.
3. Kliknij **Dodatkowe role**.
4. Znajdź użytkowników z rolą **administrator firmy**.

:::tip
Aby upewnić się, że twój zespół przechodzi na OAuth 2.0 i unika potencjalnych zakłóceń, udostępnij ten artykuł swojemu administratorowi firmy.
:::

## Zmiana na wyższą wersję OAuth 2.0 dla administratorów firmy

Jako administrator firmy masz następujące zasoby, które pomogą Ci zmienić organizację na OAuth 2.0:

- [Łączenie z Jira Cloud przy użyciu OAuth 2.0](https://help.miro.com/hc/articles/8588617184402)
- [Łączenie z Jira Data Center przy użyciu OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
- [Łączenie zespołów w organizacji z domyślnymi ustawieniami Jira](https://help.miro.com/hc/articles/26438407676434)

## Tymczasowe rozwiązanie

Jeśli OAuth 2.0 nie jest obecnie możliwy do wdrożenia w Twojej organizacji, Miro oferuje [tymczasowe rozwiązanie z wykorzystaniem OAuth 1.0](https://help.miro.com/hc/articles/27689156602514).

Jednak Miro rekomenduje zmianę na OAuth 2.0 jako najbardziej bezpieczną i przyszłościową metodę uwierzytelniania, zgodną z obecnymi standardami Atlassian.

## Dodatkowa pomoc

Jeśli Ty lub Twój administrator firmy macie pytania, skontaktujcie się z [pomocą Miro](https://help.miro.com/hc/articles/360020185799).
