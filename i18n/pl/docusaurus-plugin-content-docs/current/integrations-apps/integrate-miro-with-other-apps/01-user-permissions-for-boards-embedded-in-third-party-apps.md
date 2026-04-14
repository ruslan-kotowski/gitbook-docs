---
title: Uprawnienia użytkowników do tablic osadzonych w aplikacjach zewnętrznych
article_id: 4411883577618
translation_id: 4411883577618
locale: pl-pl
sidebar_position: 1
created_at: '2021-12-08T10:13:42Z'
updated_at: '2025-11-25T16:07:55Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'Lista osób: Właściciele tablic, współwłaściciele tablic Wersje: Wszystkie
    wersje Platformy: Przeglądarka, aplikacja komputerowa'
---

Miro oferuje kilka integracji, które umożliwiają łatwą współpracę z tablicami w środowiskach zewnętrznych, takich jak [Microsoft Teams](../microsoft), [Confluence](../atlassian/01-miro-for-confluence.md), Notion i Google Meet. Możesz odkryć inne obsługiwane aplikacje w [Miro Marketplace](https://miro.com/marketplace/category/embed-miro/). Podczas osadzania tablic możesz ustawić różne poziomy dostępu użytkowników i zarządzać tymi uprawnieniami w Miro.

## Zrozumienie dostępu do osadzeń

Udostępniając tablicę w aplikacji zewnętrznej, możesz zapewnić użytkownikom tej aplikacji jednorazową współpracę poprzez dostęp do wyświetlania, komentowania lub edycji, niezależnie od ich dostępu w Miro. Ci użytkownicy nie będą potrzebowali profilu Miro, aby uzyskać dostęp do tablicy w aplikacji. To pozwala na ustawienie specyficznych praw dostępu do tablicy dla użytkowników aplikacji, którzy nie są zarejestrowani w Miro, bez publicznego udostępniania tablicy.

Dla maksymalnego bezpieczeństwa odradzamy stosowanie tej metody poza jednorazową współpracą (taką jak warsztaty) i zalecamy, aby Twoja organizacja przydzielała dostęp do Miro odpowiednio tym, którzy tego potrzebują.

![embed_Miro_in_Zoom.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020254296722_embed%20Miro%20in%20Zoom.gif) *Konfiguracja praw dostępu do osadzenia tablicy*

Tablica staje się dostępna tylko w aplikacji, w której została osadzona. Poziom dostępu, który ustawisz dla osadzenia tablicy w aplikacji, nie wpływa na ustawienia udostępniania tablicy poza aplikacją. Na przykład, jeśli [prywatna tablica](../../using-miro/sharing-boards/15-make-a-miro-board-private.md) jest osadzona w kanale Microsoft Teams z dostępem "Każdy może wyświetlać", użytkownicy w tym kanale Microsoft Teams mogą oglądać tablicę bez logowania się do Miro. Jeśli ci sami użytkownicy spróbują uzyskać dostęp do tablicy poza kanałem Microsoft Teams, korzystając z linku do tablicy, nie będą mieli dostępu.

Jednak ustawienia udostępniania tablicy po stronie Miro mają pierwszeństwo przed poziomem dostępu ustawionym w aplikacji zewnętrznej. Na przykład, jeśli tablica jest [udostępniana publicznie po stronie Miro](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), będzie dostępna dla wszystkich w Microsoft Teams, nawet jeśli osadziłeś tablicę jako prywatną.

## Zarządzaj i cofnij dostęp do osadzeń

Możesz łatwo śledzić, zarządzać i cofać dostęp do tablic osadzonych w obsługiwanych aplikacjach zewnętrznych.

Aby zarządzać i cofać dostęp do osadzonych tablic:

1. Kliknij przycisk **Udostępnij**, aby otworzyć ustawienia udostępniania tablicy Miro.
2. Wybierz **Ustawienia udostępniania**.
3. Otwórz kartę **Osadzenia**.
4. Zobaczysz zewnętrzne aplikacje, w których tablica jest osadzona, w tym nazwę integracji, kiedy i przez kogo została osadzona oraz ustawienia dostępu do tablicy w aplikacji.
5. Aby cofnąć dostęp do tablicy w aplikacji, kliknij **Cofnij dostęp** obok aplikacji. Pamiętaj, że tej akcji nie można cofnąć.

ol

![remove_an_access_link.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020265344914_remove%20an%20access%20link.gif)
*Usuwanie linku dostępu*

Po cofnięciu dostępu do osadzenia, dostęp do tablicy w aplikacji zostanie ograniczony. Pamiętaj, że tablica może nadal być dostępna w aplikacji, jeśli jest udostępniana po stronie Miro. Na przykład:

- Jeśli ktokolwiek może **edytować** tablicę w aplikacji, a ta sama tablica jest [publicznie udostępniona](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) do **wyświetlania** po stronie Miro, to każdy nadal będzie mógł **wyświetlać** tablicę w aplikacji.
- Jeśli tablica jest prywatna i udostępniana tylko [innym użytkownikom za pośrednictwem e-maila](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), osadzona tablica będzie wymagała **logowania** w celu uzyskania do niej dostępu w aplikacji.

## Zasady i ograniczenia osadzania

Zwróć uwagę na następujące zasady i ograniczenia podczas osadzania tablic:

- Nie możesz osadzić tablicy, jeśli jest [nieaktywna](../../using-miro/tools/troubleshooting/15-the-board-is-locked.md) lub masz do niej dostęp tylko do odczytu.
- Tablice przechowywane w [darmowych zespołach](../../plans-billing/miro-plans/09-free-plan.md) nie mogą być osadzone z uprawnieniami do komentowania.
- Dla użytkowników [wersji Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) ustawienia dostępu będą zgodne z kontrolą dostępu obowiązującą w całej organizacji, co może oznaczać, że niektóre opcje udostępniania mogą być ograniczone. Dowiedz się więcej: [Zarządzanie zasadami udostępniania Enterprise dla integracji osadzania](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- Dla niektórych starych linków zobaczysz tylko poziom dostępu i aplikację, ale nie dowiesz się, kto stworzył tablicę ani kiedy została osadzona.
- Jeśli chcesz ograniczyć możliwość osadzania tablic Miro w zewnętrznych aplikacjach dla swojej organizacji Enterprise, zobacz [Zarządzanie zasadami udostępniania Enterprise dla integracji osadzania](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
- Zarządzanie linkami dostępu do osadzonych tablic nie jest jeszcze obsługiwane na urządzeniach mobilnych i tabletach.

Dowiedz się więcej o [dostępie do osadzonych tablic dla użytkowników z bezpłatnymi ograniczonymi licencjami](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
