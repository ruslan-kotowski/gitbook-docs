---
title: Zarządzanie licencjami w ramach Programu elastycznych licencji (FLP)
article_id: 360018622159
translation_id: 360018622159
locale: pl-pl
sidebar_position: 5
created_at: '2020-12-29T10:44:01Z'
updated_at: '2026-02-23T18:22:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Odpowiednie dla: Enterprise'
---

Dowiedz się więcej o zarządzaniu licencjami w programie elastycznych licencji (FLP), w tym jakie opcje zarządzania licencjami są dostępne dla nowych użytkowników i jak konwertować istniejące licencje.

:::tip
Jeśli dopiero poznajesz licencjonowanie FLP, zalecamy najpierw przeczytać [program elastycznych licencji](03-flexible-licensing-program-flp.md) oraz [Poziomy dostępu użytkowników w wersji Enterprise](../../user-management/11-user-access-levels-on-enterprise-plan.md), aby zrozumieć, jak nasze modele licencjonowania, rodzaje licencji i role w Miro współpracują ze sobą.
:::

## Przydzielanie licencji nowym użytkownikom

Członkowie Goście Odwiedzający

Na podstawie domyślnych ustawień licencji w Twojej firmie nowi członkowie otrzymują licencję Free lub bezpłatną ograniczoną. Aby ustawić domyślną licencję dla nowych członków w ramach swojej subskrypcji, skontaktuj się z osobą do kontaktu w Miro.

Nowi członkowie otrzymują domyślną licencję:

- gdy są zapraszani przez nie-administratorów
- automatycznie za pośrednictwem [obsługi administracyjnej Just-in-Time](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), [zarządzania domeną](../../canvas-25-admin-features/domain-control/01-domain-control.md) lub [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)

Administratorzy firmy mają również możliwość wyboru licencji dla zapraszanych członków.

- wybierz **darmowy**, jeśli chcesz, aby użytkownicy mieli możliwość edycji (zostaną zaktualizowani do licencji Standard lub Full (legacy) zaraz po edytowaniu lub utworzeniu tablicy, zaproszeni do edycji tablicy, otrzymaniu współwłasności tablicy lub dodaniu do [projektu](../../../using-miro/sharing-boards/16-projects.md) jako edytujący)
- wybierz **Free Restricted**, aby zaprosić użytkownika bez praw do edytowania

Goście zaproszeni do tablicy zawsze otrzymują licencję **damową**. Dowiedz się, jak [zapraszać gości na abonament Enterprise](../../../using-miro/sharing-boards/07-collaboration-with-guests.md).

[Odwiedzający](../../../using-miro/sharing-boards/08-collaboration-with-visitors.md) tablic udostępnionych publicznie są darmowi i nie mają licencji.

## Jak zmienić licencje na wyższą lub niższą wersję

> **Kto może to zrobić:** Administratorzy firmy

Licencje **Free** są automatycznie zmieniane na wyższą wersję (Standard lub Full (legacy)) w momencie, gdy użytkownik utworzy lub edytuje tablicę.

Free Restricted na Standard lub Full (legacy)  Standard lub Full (legacy) na Free Restricted Zbiorcza konwersja licencji

Bezpłatne ograniczone licencje mogą być zaktualizowane do standardowej lub pełnej (legacy) licencji ręcznie przez administratorów firmy lub w ramach [Enterprise workflow automation](../enterprise-workflow-automation/01-enterprise-workflow-automation.md).

Aby zmienić bezpłatną ograniczoną licencję na pełną licencję:

1. Otwórz **Zespoły** lub otwórz **Ustawienia organizacji** > **Użytkownicy** > **Wszyscy użytkownicy** > **Aktywni użytkownicy**.
2. Kliknij ikonę **menu z 3 kropkami** (**...**) obok użytkownika z bezpłatną ograniczoną licencją.
3. Wybierz **Zmień na Standardowego członka**.

Pełne licencje mogą być zmienione na niższą wersję na bezpłatną ograniczoną licencję, jeśli administratorzy firmy chcą ograniczyć dostęp użytkownika i zwolnić dodatkowe pełne licencje.

Pełni członkowie nie mogą być zmieniani na bezpłatną licencję, ponieważ bezpłatne licencje mogą być przydzielane tylko nowym użytkownikom.

Aby dokonać zmiany pełnej licencji na bezpłatną ograniczoną licencję:

1. Otwórz **Zespoły** lub **Ustawienia organizacji** > **Użytkownicy** > **Wszyscy użytkownicy** >**Aktywni użytkownicy**.
2. Kliknij ikonę **menu z 3 kropkami** (**...**) obok użytkownika z pełną licencją.
3. Wybierz **Zmień na bezpłatną ograniczoną licencję**.

Aby przeprowadzić masową zamianę kilku licencji naraz:

1. Otwórz **Ustawienia organizacji** > **Użytkownicy** > **Wszyscy użytkownicy** > **Aktywni użytkownicy**.
2. Indywidualnie wybierz wszystkich użytkowników, których licencje chcesz zmienić, lub zastosuj filtry do wyboru użytkowników. Możesz wybrać do 50 użytkowników
3. Kliknij **Zbiorcze działania** i wybierz nową opcję licencji
