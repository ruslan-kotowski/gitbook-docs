---
title: Skonfiguruj integracje z Microsoft i Power BI
article_id: 25132703621394
translation_id: 25132703621394
locale: pl-pl
sidebar_position: 3
created_at: '2025-03-06T10:27:14Z'
updated_at: '2025-11-25T15:49:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
availability:
  notes: Aby uzyskać obszerne dokumenty administratora dotyczące integracji Miro z
    Microsoft lub Power BI, w tym szczegółowe diagramy i dodatkowe FAQ, zapoznaj się
    z [dokumentacją administratora Microsoft](https://docs.google.com/document/d/1Gw94z5Pc-elS-pRXKGZVBWKKNEIFR9y9yzAAkbXKwMM/edit?usp=sharing)
    lub [dokumentacją administratora Power BI](https://docs.google.com/document/d/1hMepF163jQF8LI-U8ES8DzHVMW4TltXDr14fJ2KU29k/edit?tab=t.0#heading=h.gu9ng058yy7y).
---

Ten artykuł opisuje, jak skonfigurować integrację Microsoft lub Power BI z Miro.

## Skonfiguruj integrację z Microsoft lub Power BI

Aby skonfigurować integrację z Microsoft lub Power BI, musisz włączyć użytkownikom możliwość autoryzowania własnej zawartości Microsoft lub Power BI w Miro.

### Wymagania wstępne

- Upewnij się, że masz dostęp administratora do Microsoft Entra.
- Administrator firmy zatwierdził Microsoft lub Power BI dla Twojej organizacji w Miro (odnosi się to do polityk zatwierdzania aplikacji po stronie Miro, jeśli Twoja organizacja ogranicza instalację aplikacji).

### Procedura

Te kroki koncentrują się na skonfigurowaniu Microsoft Entra, aby umożliwić integrację z Miro.

1. Zaloguj się do **Entra** jako administrator.
2. Przejdź do **Aplikacje dla przedsiębiorstw** > **Zgoda i uprawnienia**.
3. Dla **Użytkownicy mogą poprosić o zgodę administratora na aplikacje, do których nie mogą udzielić zgody**, wybierz **Tak**.
4. Pod **Kto może przeglądać prośby o zgodę administratora**, wybierz niezbędnych użytkowników, role lub grupy, którym chcesz zezwolić na przeglądanie próśb o zgodę administratora dla aplikacji.

:::note
Następnie administratorzy Entra wyznaczeni w kroku 4 powyżej mogą przejść do **Enterprise Applications > Admin Consent Requests** w Microsoft Entra, aby przejrzeć i zatwierdzić aplikację "Contenthub PowerBI Integratio" (lub podobnie nazwaną) dla organizacji.
:::

## Zwaliduj swoją integrację z Microsoft lub PowerBI

Skopiuj i wklej link do swojej tablicy Miro.

Jeśli aplikacja jest wstępnie zatwierdzona przez administratora firmy, postępuj zgodnie z instrukcjami wyświetlanymi w oknie modalnym. Miro dodaje treści z Twojej aplikacji na tablicę jako iFrame.

Jeśli aplikacja nie jest wstępnie zatwierdzona, otworzy się **Dodaj i włącz** okno modalne, które umożliwia wysłanie prośby do administratora firmy. Wyślij swoją prośbę.

Gdy administrator firmy odpowie, otrzymasz powiadomienie.

**Więcej informacji:** Zobacz [zarządzanie aplikacjami](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).
