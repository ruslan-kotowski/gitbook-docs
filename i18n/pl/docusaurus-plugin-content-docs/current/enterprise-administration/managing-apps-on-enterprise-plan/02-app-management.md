---
title: "Zarz\u0105dzanie aplikacjami"
article_id: 4404659741458
translation_id: 4404659741458
locale: pl-pl
sidebar_position: 2
created_at: '2021-08-03T15:46:50Z'
updated_at: '2026-01-29T10:00:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: apps-management
---

Dowiedz się, jak zarządzać aplikacjami i uprawnieniami na poziomie organizacyjnym i zespołowym.

> **Dotyczy:** wersja Business, wersja Enterprise
> **Kto może to zrobić:** administratorzy zespołu, administratorzy firmy

### Kto może zarządzać aplikacjami?

Zarządzanie aplikacjami na poziomie organizacyjnym jest dostępne tylko na wersji Enterprise dla administratorów firmy. Zarządzanie aplikacjami na poziomie zespołu jest dostępne w wersji Business i Enterprise dla administratorów zespołu i firmy.

### Dodaj aplikacje dla organizacji lub konkretnych zespołów

Dodawaj i autoryzuj aplikacje dla wszystkich użytkowników w organizacji lub wybranych zespołów w Twojej organizacji z poziomu zarządzania aplikacjami.
Przejdź do **ustawienia** firmy > **aplikacje i integracje** > **aplikacje**. Z tej sekcji administratorzy firmy mogą dodawać aplikacje dla wszystkich lub wybranych zespołów.

![apps-access.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803476626_apps-access.png)*Zarządzanie aplikacjami w ustawieniach firmy*

Wpisz nazwę aplikacji lub ID klienta w pasku wyszukiwania. Wybierz aplikację z listy rozwijanej i kliknij **Dodaj**.

![add-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780909714_add-app.png)*Dodawanie aplikacji w ustawieniach firmy*

Możesz dodać aplikację dla wszystkich zespołów w Twojej organizacji lub wybrać konkretne zespoły. Jeśli aplikacja jest już dodana dla niektórych zespołów, zobaczysz odpowiadający tag. Jeśli ponownie dodasz aplikację dla zespołu, jego członkowie będą musieli ponownie autoryzować aplikację. Kliknij **Dodaj**, aby zakończyć.

![add-apps-where.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780917010_add-apps-where.png)
*Wybieranie, dla kogo zainstalować aplikację Google Drive*

Jeśli dodasz aplikację dla wszystkich zespołów, aplikacja zostanie dodana również dla wszystkich nowo utworzonych zespołów.

### Wstępnie dodane aplikacje

Niektóre aplikacje są już wstępnie dodane dla użytkowników. Mogą wymagać dodatkowej autoryzacji lub indywidualnego logowania. Te wstępnie dodane aplikacje to: [Box](../../integrations-apps/more-integrations/05-box-legacy.md), [Dropbox](../../integrations-apps/more-integrations/06-dropbox.md), [Google Drive](../../integrations-apps/google/05-google-drive.md), [OneDrive](../../integrations-apps/microsoft/06-onedrive.md), [Smartsheet](../../integrations-apps/more-integrations/15-smartsheet-app-for-miro.md), [Azure Cards](../../integrations-apps/microsoft/03-azure-cards.md), [karta Jira](../../integrations-apps/atlassian/03-jira-cards.md),[Brandfetch](https://miro.com/marketplace/brandfetch/), [Google Images](../../integrations-apps/google/06-google-images.md), [Slack](../../integrations-apps/more-integrations/14-slack.md). Te aplikacje nie zostaną dodane, jeśli nie znajdują się na liście zatwierdzonych przez firmę. Możesz zarządzać tą listą, jeśli jesteś administratorem firmy.

### Preautoryzacja aplikacji dla organizacji

Jeśli dodajesz aplikację, możesz również jednocześnie ją preautoryzować. Jeśli aplikacja zostanie dodana i preautoryzowana przez administratora, użytkownicy w organizacji będą mogli zacząć z niej korzystać od razu. Może jednak być wymagane logowanie do zewnętrznych serwisów dla niektórych aplikacji.

Ta funkcja jest dostępna tylko dla aplikacji zbudowanych przy użyciu Miro Web SDK. Miro Web SDK umożliwia rozszerzanie funkcjonalności Miro. To narzędzie do tworzenia zaawansowanych aplikacji, które działają wewnątrz tablicy Miro.

### Zatwierdzanie aplikacji do zarządzania przez użytkowników indywidualnych

Domyślnie użytkownicy mogą dodawać dowolne aplikacje dla swojego zespołu. Administratorzy firmy mogą ograniczyć zarządzanie aplikacjami przez użytkowników, aby pozwolić na dodawanie tylko określonych aplikacji przez ich zespoły.

Administratorzy firmy mogą włączyć lub ograniczyć dodawanie określonych aplikacji dla swoich użytkowników, przechodząc do **ustawienia firmy** > **aplikacje i integracje** > **aplikacje** > **zarządzanie aplikacjami** i włączając opcję **Ogranicz członków do dodawania aplikacji tylko z poniższej listy**.

![manage-apps.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780921490_manage-apps.png)*Ograniczanie dodawania zatwierdzonych aplikacji w abonamencie Enterprise*

Jeśli to ograniczone, tylko te aplikacje, które zostały zatwierdzone, mogą być dodawane przez użytkowników Enterprise. Aby zatwierdzić aplikację dla użytkowników, włącz przełącznik obok niej lub wklej ID klienta w odpowiednim polu, aby zatwierdzić aplikację rozwijaną wewnętrznie.

Aby ograniczyć wcześniej dodaną aplikację, znajdź ją na liście i upewnij się, że przełącznik obok aplikacji jest wyłączony. Należy pamiętać, że użytkownicy z wszystkich zespołów Enterprise nie będą mogli korzystać z aplikacji, jeśli jest ona ograniczona.

Jeśli aplikacja jest ograniczona w twojej organizacji, użytkownicy będą mogli wysyłać [prośby o korzystanie z aplikacji do administratorów firmy](03-app-request-flow.md).

Użytkownicy mogą zobaczyć zatwierdzone aplikacje w Marketplace na tablicach Miro przechowywanych w ramach wersji Enterprise.

### Zezwalanie lub ograniczanie użycia aplikacji w zespołach

Administratorzy zespołów i firmy mogą także zarządzać użyciem aplikacji na poziomie zespołu: mogą zezwalać lub ograniczać członkom zespołu dodawanie nowych aplikacji dla zespołu. Ustawienie jest konfigurowane dla każdego zespołu oddzielnie.

![add-apps-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780928914_add-apps-team.png)*Aplikacje i integracje w ustawieniach zespołu*

Dowiedz się więcej o [aplikacjach i integracjach Miro.](../../integrations-apps/integrations-basics)
