---
title: Jak skonfigurować webhooks dla Centrum danych Jira
article_id: 360017731113
translation_id: 26964605745170
locale: pl-pl
sidebar_position: 15
created_at: '2025-05-26T12:21:44Z'
updated_at: '2026-01-14T09:25:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Osoby: Administratorzy systemu Jira Abonamenty: Wszystkie abonamenty Miro
    (dla integracji z Jira Server/Data Center przez OAuth 1.0) Platformy: Przeglądarka,
    aplikacja komputerowa (do procedur konfiguracji)'
---

Aby zapewnić, że Twoje [karty Jira](https://help.miro.com/hc/articles/360017572434) na tablicy Miro są zawsze aktualne, Miro musi otrzymywać wiadomości z Jira za każdym razem, gdy dochodzi do zmian danych. Te zdarzenia Jira są przekazywane do Miro za pomocą webhoka.

Ten przewodnik przedstawia dwa sposoby tworzenia webhooków dla Jira Server i Jira Data Center za pomocą OAuth 1.0 i OAuth2.0.

## Automatyczne tworzenie webhoka

Podczas [konfigurowania integracji kart Jira](https://help.miro.com/hc/articles/360019501754), jeśli łączysz się z serwerem Jira lub Jira Data Center, możesz pozostawić opcję **Automatycznie utwórz webhook** włączoną. Jest to zalecana metoda.

:::note
Automatyczne tworzenie webhooków wymaga zalogowania się do Jira jako administrator systemu Jira.
:::

![jira-webhooks-server-config.png](../../../../../../docs/integrations-apps/atlassian/images/21304245707026_jira-webhooks-server-config.png)
*Ustawienia kart Jira, Krok 2: "Automatycznie utwórz webhook**"** jest włączona*

Po automatycznym utworzeniu webhooka dobrą praktyką jest przejście do strony WebHooks w Jira i edycja webhooka, aby nadać mu unikalną nazwę. Jest to szczególnie ważne, jeśli planujesz podłączyć kilka zespołów Miro do swojej instancji Jira.

:::note
W przypadku połączeń OAuth2.0, połączenie po stronie Miro jest ustawiane na poziomie firmy. Jeden webhook jest tworzony dla wszystkich zespołów Miro.
:::

:::note
W przypadku połączeń OAuth 1.0 na poziomie zespołu Miro, webhook jest tworzony dla każdego zespołu. Na poziomie firmy Miro, jeden webhook jest tworzony dla wszystkich zespołów.
:::

## Utwórz webhooka ręcznie

Jeśli wolisz lub potrzebujesz utworzyć webhooka ręcznie, wykonaj te kroki.

**Uzyskaj URL webhooka z Miro**

1. W ustawieniach kart Jira w Miro (Krok 2, podczas łączenia z Jira Server/Data Center) odznacz opcję **Twórz webhook automatycznie**.
2. Skopiuj i wklej **URL Twojej organizacji Jira** i kliknij **Połącz i zapisz ustawienia.**
   ![jira-webhooks-configure-jira-url-cropped.png](../../../../../../docs/integrations-apps/atlassian/images/21304245708818_jira-webhooks-configure-jira-url-cropped.png)
   *Ustawienia kart Jira, Krok 2: "Twórz webhook automatycznie" jest wyłączony*
3. Zezwól na połączenie integracji w Jira, gdy zostaniesz o to poproszony.
4. Po wykonaniu tych kroków Miro dostarczy Ci adres **URL webhooka**:
   ![webhook_URL.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016928565010_webhook%20URL.jpg)*Adres URL webhooka dostarczony przez Miro*

:::note
Jeśli nie jesteś administratorem systemu Jira, skopiuj adres **URL webhooka** dostarczony przez Miro i przekaż go administratorowi systemu Jira, aby mógł utworzyć webhook po stronie Jira, korzystając z poniższych instrukcji.
:::

**Tworzenie webhooka w Jira**

Poniżej znajdują się kroki do utworzenia webhooka w Jira za pomocą URL uzyskanego z Miro. Możesz również odwołać się do oficjalnej dokumentacji Atlassian dla [Jira Server](https://developer.atlassian.com/server/jira/platform/webhooks/) oraz [Jira Cloud](https://developer.atlassian.com/cloud/jira/platform/webhooks/) (choć ten artykuł skupia się na Server/Data Center).

1. Aby przejść do strony **Webhooki** w Jira, wybierz **Zarządzanie Jira** > **System** > **Zaawansowane >** **Webhooki** (dokładna ścieżka może nieznacznie się różnić w zależności od wersji Jira). Alternatywnie możesz często użyć bezpośredniego linku, dodając `/plugins/servlet/webhooks` do URL Twojej instancji Jira (np. `https://TwojaNazwaInstancjiJira/plugins/servlet/webhooks`).
2. Kliknij **Utwórz webhook** w prawym górnym rogu strony Webhooki.
3. Wpisz opisową **nazwę** dla webhooka (np. "Webhook integracji Miro").
4. Ustaw status webhooka na **Włączony**.
5. Wklej skopiowany z ustawień Miro **URL Webhooka** w pole URL.
   ![system_webhooks.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941532050_system%20webhooks.jpg)
   *Konfiguracja systemowa webhooków w Jira*
6. W sekcji **Zdarzenia**, pod **Zadanie**, wybierz zdarzenia **zaktualizowane** i **usunięte**.
7. Kliknij **Utwórz**, aby zapisać webhook.
   ![Jira_Webhook_settings.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941533074_Jira%20Webhook%20settings.jpg)
   *Ustawienia zdarzeń webhooka Jira*
8. Po utworzeniu webhooku w Jira, wróć do **Kroku 2** w ustawieniach kart Jira w Miro, upewnij się, że **URL Jira** jest poprawnie wypełniony, i kliknij **Połącz**.

Teraz webhook jest utworzony i skonfigurowany. Karty Jira na Twoich tablicach Miro będą aktualizowały się automatycznie po dokonaniu zmian w Jira.
