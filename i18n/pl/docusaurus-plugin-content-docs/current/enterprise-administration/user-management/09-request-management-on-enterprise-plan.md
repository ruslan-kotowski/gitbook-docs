---
title: Zarządzanie prośbami w wersji Enterprise
article_id: 360017237379
translation_id: 360017237379
locale: pl-pl
sidebar_position: 9
created_at: '2020-10-27T12:09:40Z'
updated_at: '2026-02-19T11:00:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: access-request-management
availability:
  notes: 'Dotyczy: Enterprise Plan Kto może to zrobić: administrator firmy'
---

W Miro prośby o licencje, dostęp do zespołu i organizacji oraz pojedyncze logowanie (SSO) są domyślnie wysyłane przez e-mail do administratorów firmy. Dzięki zaawansowanym funkcjom zarządzania prośbami, administratorzy firmy mogą dostosować sposób odbierania i obsługi tych próśb.

### Rodzaj prośby

Prośby dzielą się na cztery kategorie:

- Prośby o dołączenie do organizacji
- Prośby o dołączenie do zespołu
- Prośby o licencję
- Prośby dotyczące problemów z SSO

Dowiedz się o różnych scenariuszach prośby dla abonamentu Enterprise.

### Opcje zarządzania prośbami

Administratorzy firmy mają szereg opcji zarządzania prośbami, które pozwalają im dostosować procesy do rodzaju prośby:

:::note
Opcje wysyłania e-maili do wszystkich administratorów firmy lub do wybranych administratorów firmy obejmują administratorów zespołu.
:::

- Wyślij e-mail do wszystkich administratorów firmy
- Wyślij e-mail do wybranych administratorów firmy
- Utwórz zgłoszenie serwisowe
- Przekieruj na spersonalizowany adres URL

## Konfiguracja zarządzania prośbami

:::note
Aby [zarządzać prośbami licencyjnymi bezpośrednio w Miro](04-license-requests-on-enterprise-plan.md), wybierz opcję **Wyślij e-mail do wszystkich administratorów firmy** lub **Wyślij e-mail do konkretnych administratorów**. Otrzymasz wszystkie przyszłe prośby licencyjne w swoich ustawieniach prośb licencyjnych.
:::

### Wyślij e-mail do wszystkich administratorów firmy

Wszyscy administratorzy firmy otrzymają powiadomienie e-mail, gdy użytkownik złoży prośbę o dostęp.

1. W **Ustawieniach firmy** przejdź do **Użytkownicy** > **Prośby o dostęp** > **Zarządzanie prośbami**.
2. Kliknij na **Typ prośby** , który chcesz zarządzać.
3. Otworzy się okno pop-up. Kliknij na rozwijane menu i wybierz **E-mail dla wszystkich administratorów firmy**.

:::note
Opcje wysyłania e-maila do wszystkich administratorów firmy, lub do konkretnych administratorów firmy, obejmują również administratorów zespołów.
:::

### Wyślij e-mail do wybranych administratorów firmy

Administratorzy firmy mogą określić do 5 adresów e-mail. Tylko wskazane e-maile otrzymają prośbę. E-maile nie muszą należeć do użytkowników Miro.

1. Przejdź do **ustawień** firmy > **Użytkownicy** > **Prośby o dostęp** > **Zarządzanie prośbami**.
2. Kliknij na **Typ prośby**, który chcesz zarządzać.
3. Otworzy się wyskakujące okienko. Kliknij na rozwijane menu i wybierz **Wyślij e-mail do konkretnych administratorów firmy**.
4. Dodaj do 5 e-maili. Kliknij **Dodaj** za każdym razem, gdy wpiszesz adres e-mail w polu e-mail.

:::note
Opcje wysyłania e-maili do wszystkich administratorów firmy lub konkretnych administratorów firmy obejmują także administratorów zespołów.
:::

### Utwórz zgłoszenie w serwisie

Automatycznie twórz zgłoszenie serwisowe za każdym razem, gdy użytkownik składa prośbę o dostęp. Ta funkcja jest obecnie obsługiwana przez **ServiceNow** oraz **Jira Service Management**.

ServiceNow Jira Service Management

1. Skonfiguruj ustawienia e-mail dla ServiceNow. Utwórz element katalogu dla Miro w ServiceNow. Otwórz ServiceNow, przejdź do **Właściwości systemowe** > **Właściwości e-mail** i włącz odbieranie przychodzących e-maili

2. [Utwórz akcję przychodzącego e-maila](https://docs.servicenow.com/bundle/tokyo-servicenow-platform/page/administer/notification/task/t_CreatingAnInboundEmailAction.html). W polu **Od**pole poniżej linii **Ten wewnętrzny akcja będzie wyzwalana tylko przez e-maile od tego nadawcy**, wpisz [notification@miro.com](mailto:notification@miro.com).

3. [Ustaw wartości pól z treści e-maila](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/notification/reference/r_SetFieldValsFromTheEmailBody.html) w celu skonfigurowania dodatkowych ustawień i ustawienia procesu konwersji e-maila od Miro na bilet w ServiceNow. Na przykład, możesz przypisać nowo utworzony bilet do konkretnej osoby.

4. Przejdź do Miro, otwórz **Ustawienia** firmy > **Użytkownicy** > **Prośby o dostęp** > **Zarządzanie prośbami**, i wybierz **Utwórz zgłoszenie w ServiceNow**. W polu e-mail wpisz swój adres e-mail do ServiceNow.

1. Skonfiguruj ustawienia e-mail dla Jira Service Management. Wybierz **Ustawienia projektu** > **Prośby e-mail** w swoim projekcie serwisowym. [Wybierz swojego dostawcę usług e-mail i postępuj zgodnie z instrukcjami, aby połączyć Miro](https://support.atlassian.com/jira-service-management-cloud/docs/receive-requests-from-an-email-address/).

2. Przejdź do Miro, otwórz **Ustawienia firmy** > **Zarządzanie użytkownikami**> **Prośby o dostęp** > **Zarządzanie prośbami**, i wybierz **Utwórz zgłoszenie w Jira Service Management**. W polu e-mail wprowadź adres e-mail Jira Service Management.

### Przekieruj na spersonalizowany adres URL

Osoba składająca prośbę zostanie przekierowana na wybrany adres URL w celu podjęcia następnych kroków.

1. W sekcji **Ustawienia firmy** przejdź do **Użytkownicy** > **Prośby o dostęp** > **Zarządzanie prośbami**.
2. Kliknij na **Rodzaj prośby**którą chcesz zarządzać.
3. Pojawi się wyskakujące okno. Kliknij listę rozwijaną i wybierz **Przekieruj na spersonalizowany adres URL**.
4. Wpisz link przekierowania w polu **spersonalizowany adres URL**.

## Scenariusze zgłoszeń

Poniższe scenariusze pokazują, jak różne prośby są wyzwalane w Miro. Przejrzyj scenariusze, aby zdecydować, jak chcesz zarządzać każdym typem zgłoszenia.

|  |  |
| --- | --- |
| **Prośby o dołączenie do organizacji** | - Gdy nowy użytkownik prosi o dołączenie do zespołu, który ma subskrypcję zarządzaną przez firmę z [zarządzaniem domeną](../canvas-25-admin-features/domain-control/01-domain-control.md) (chyba że zarządzanie domeną jest ustawione na pozyskiwanie nowych użytkowników). |
| **Prośby o licencję** | - Kiedy [użytkownik z bezpłatnym ograniczeniem](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) prosi o Standardową lub Pełną (przestarzałą) licencję. - Gdy członek prosi o standardową lub pełną (starszą) licencję dla użytkownika z bezpłatną ograniczoną licencją, o ile członkowie nie są uprawnieni do zapraszania nowych użytkowników do subskrypcji w [ustawieniach zaproszeń](03-invitation-settings-on-enterprise-plan.md). - Gdy użytkownik z pełną (starszą) lub standardową licencją prosi o zaawansowaną licencję. - Gdy członek próbuje zaprosić lub nadać uprawnienia do edycji użytkownikowi z bezpłatną ograniczoną licencją. |
| **Prośby o dołączenie do zespołu** | - Kiedy użytkownik, który nie jest administratorem, próbuje udostępnić tablicę użytkownikowi, który *nie* jest członkiem zespołu, zaproszenia dla gości są wyłączone w [ustawieniach zaproszeń](03-invitation-settings-on-enterprise-plan.md), a tylko administratorzy mogą zapraszać nowych członków do zespołu. - Gdy członek zespołu, który nie ma pozwolenia na zapraszanie nowych członków, próbuje nadać rolę właściciela lub [współwłaściciela](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) na określonej tablicy użytkownikowi, który nie jest członkiem zespołu. - Gdy użytkownik Enterprise prosi o dołączenie do zespołu [dostępnego do odkrywania w jego organizacji](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md). - Kiedy [gość](../../using-miro/sharing-boards/07-collaboration-with-guests.md) zaproszony do określonych tablic w zespole prosi o dołączenie do zespołu |
| **Prośby dotyczące problemów z SSO** | - Kiedy użytkownik nie otrzymał dostępu do Miro od dostawcy tożsamości i ma problemy z logowaniem się przez SSO. |

## Często zadawane pytania

**Dlaczego nadal otrzymuję e-maile, mimo że skonfigurowałem swoje ustawienia do tworzenia zgłoszeń?**

Jeśli administratorzy zespołu mogą zapraszać nowych użytkowników do zespołu w [ustawieniach zaproszeń](03-invitation-settings-on-enterprise-plan.md), otrzymają prośby o zaproszenie związane z tym zespołem za pośrednictwem e-maila, nawet jeśli ustawienia zarządzania prośbami są skonfigurowane inaczej. Administratorzy firmy, którzy są również administratorami zespołu, także nadal otrzymują te e-maile.

**Skąd administratorzy zespołu wiedzą o prośbie dołączenia do ich zespołu?**

Jeśli mają uprawnienia do zapraszania użytkowników do swoich zespołów, administratorzy zespołu otrzymają e-mail dotyczący próśb niezależnie od ustawień zarządzania prośbami.
