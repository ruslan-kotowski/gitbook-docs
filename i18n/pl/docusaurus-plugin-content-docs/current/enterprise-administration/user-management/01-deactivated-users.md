---
title: "Dezaktywowani u\u017Cytkownicy"
article_id: 360025025894
translation_id: 360025025894
locale: pl-pl
sidebar_position: 1
created_at: '2019-06-19T22:16:18Z'
updated_at: '2026-02-19T10:44:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-deactivation
---

Zaawansowane zarządzanie użytkownikami w Miro pozwala administratorom firmy na dezaktywowanie użytkowników zamiast ich usuwania. Dezaktywowani użytkownicy pozostają w katalogu abonamentu i mogą być reaktywowani w dowolnym momencie.

> **Dostępne dla**: [Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Ustawiane przez:** administratorów firmy

## Zasady

- Dezaktywowani użytkownicy nie będą mieli dostępu do Twojego konta Enterprise i jego funkcji.
- Jeśli włączyłeś ustawienie [Blokuj dezaktywowanych użytkowników](02-block-deactivated-users.md), dezaktywacja zarządzanego użytkownika zablokuje jego możliwość logowania się do Miro.
- Dezaktywowani użytkownicy nie będą już mogli używać opcji pojedynczego logowania Twojej firmy do logowania, powracając do standardowych metod uwierzytelniania.
- Udostępnione tablice i przestrzenie stworzone przez dezaktywowanych użytkowników *nie* są przypisywane nikomu innemu i nadal są dostępne dla współpracowników (chyba że podczas dezaktywacji usuniesz użytkownika z jego zespołu. W takim przypadku tablice są przypisywane do administratora zespołu. Jest to zazwyczaj istotne dla operacji [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)).
- Wszystkie [powiadomienia](../../using-miro/managing-your-profile/02-miro-notifications.md) do dezaktywowanych użytkowników są blokowane.
- Inni użytkownicy nie mogą udostępniać tablic i przestrzeni dezaktywowanym użytkownikom.
- Dezaktywowani użytkownicy nie mogą być dodawani do zespołów w ramach Twojej subskrypcji Enterprise. Administratorzy firmy mogą reaktywować dezaktywowanych użytkowników, zapraszając ich jako członków, [dowiedz się więcej](05-manage-user-invitations-on-enterprise-plan.md).
- Dezaktywowani użytkownicy nie są rozliczani. Ich licencje są zwalniane i mogą być przypisane innemu aktywnemu użytkownikowi.
- Następujące atrybuty nie mogą być aktualizowane dla dezaktywowanych użytkowników:

|  |
| --- |
| `nazwaUżytkownika` |
| `typUżytkownika` |
| `role.wartość` |

## Dezaktywuj użytkownika

Możesz dezaktywować użytkownika w dowolnym momencie. Kiedy dezaktywujesz użytkownika, jego stan zmienia się z **Aktywny** na **Dezaktywowany** i przestaje korzystać z licencji. Zmiana ta jest także widoczna na listach Aktywnych i Dezaktywowanych użytkowników w ustawieniach **Użytkowników**.

Aby dezaktywować użytkownika:

1. Otwórz **ustawienia firmy**.
2. Wybierz **Wszyscy użytkownicy** z menu **Użytkownicy****.**
3. Kliknij **menu z 3 kropkami** (**...**) po prawej stronie użytkownika, którego chcesz dezaktywować.
4. Kliknij **Dezaktywuj**.
   ![deactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781594002_deactivate-users.png)
   *Opcja dezaktywacji użytkownika w abonamencie Enterprise*

   Możesz również dezaktywować użytkowników zbiorczo. Wybierz kilku użytkowników, zaznaczając pola po lewej stronie, lub zastosuj filtry i wybierz jednocześnie do 50 przefiltrowanych użytkowników, a następnie wybierz **Dezaktywuj** w sekcji **Akcje zbiorcze**.
5. Zaznacz pole **Przypisz zawartość użytkownika** jeśli chcesz przenieść tablice użytkownika, [szablony](../../getting-started/start-here/your-first-board/02-custom-templates.md) oraz [przestrzenie](../../using-miro/spaces/01-spaces.md). Nowy właściciel musi zostać wybrany dla każdego zespołu, w którym wybrany użytkownik posiadał zawartość. Przypisanie zawartości użytkowników nie może zostać cofnięte.
   ![deactivate-reassign-content.png](../../../../../../docs/enterprise-administration/user-management/images/23921804187154_deactivate-reassign-content.png)
   *Opcja przypisania zawartości użytkownika podczas jego dezaktywacji*
6. Wybierz **Dezaktywuj.**

Dezaktywacja użytkowników nie usuwa ich danych w Miro. Uprawnienia, które posiadają, będą zachowane i zostaną przywrócone po ponownej aktywacji użytkowników.

:::note
Uwaga: aby dezaktywować administratora firmy, musisz najpierw cofnąć jego uprawnienia administratora firmy.
:::

:::note
Jeśli widzisz powiadomienie **Zespół musi mieć co najmniej jednego administratora** podczas próby dezaktywacji użytkownika, oznacza to, że użytkownik jest *jedynym* administratorem w zespole lub zespołach typu Enterprise. Aby to naprawić, [zaprosisz siebie do tych zespołów](05-manage-user-invitations-on-enterprise-plan.md) i [przyznasz sobie uprawnienia administratora zespołu](../../administration/user-management/06-how-to-manage-admin-roles.md). Kliknij liczbę zespołów danego użytkownika, aby dowiedzieć się, do których zespołów należy.
:::

:::note
Jeżeli Twoja firma korzysta z rozwiązania [SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md), możesz również dezaktywować użytkowników za pośrednictwem swojego dostawcy tożsamości. Kiedy użytkownik zostanie dezaktywowany przez SCIM, jego zawartość nie jest przypisywana ponownie — opcja przypisania jest wspierana tylko w interfejsie użytkownika dla tego scenariusza.
:::

### Automatyczna dezaktywacja gości

Dla gości (użytkowników pierwotnie zaproszonych do Twoich tablic przez e-mail) możesz włączyć [automatyczną dezaktywację](03-invitation-settings-on-enterprise-plan.md).

## Ponowna aktywacja użytkownika

Aby ponownie aktywować użytkownika:

1. Otwórz **ustawienia Firmy**.
2. Wybierz **Wszyscy użytkownicy** z menu Użytkownicy, a następnie zakładkę **Dezaktywowani użytkownicy****.**
3. Kliknij ikonę **menu z 3 kropkami** (...) po prawej stronie użytkownika, którego chcesz reaktywować.
4. Wybierz **Reaktywuj**.
5. Dodaj użytkownika do zespołów, jeśli to konieczne.
6. Potwierdź **Reaktywuj**.

![reactivate-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921804191762_reactivate-users.png)
*Reaktywacja użytkownika*

Kiedy przywracasz użytkownika:

- Użytkownicy mogą zalogować się od razu
- Będą mieli dostęp do udostępnionych tablic, tablic zespołowych i tablic, które utworzyli przed dezaktywacją (chyba że tablice zostały przekazane innym osobom)

:::note
Uwaga: tylko administratorzy firmy mogą ponownie aktywować zdezaktualizowanych użytkowników.
:::

### Trwałe usuwanie użytkownika

Aby trwale usunąć dezaktywowanego użytkownika:

1. Otwórz swoje **Ustawienia firmy**.
2. W menu kliknij **Użytkownicy** > **Wszyscy użytkownicy**.
3. Wybierz kartę **Dezaktywowani użytkownicy**.
4. Kliknij ikonę **menu z 3 kropkami** **(...)** po prawej stronie użytkownika, którego chcesz usunąć.
5. Wybierz **Usuń**.
   ![delete-users.png](../../../../../../docs/enterprise-administration/user-management/images/23921781612562_delete-users.png)
   *Usuwanie dezaktywowanego użytkownika*
6. Wybierz, czy chcesz przypisać zawartość użytkownika do nowego właściciela, czy usunąć ją — wybierz nowego właściciela i kliknij **Usuń użytkownika** lub wybierz **Usuń użytkownika i zawartość**.

Możesz również usuwać użytkowników za pomocą akcji zbiorczych:

1. Na karcie Dezaktywowani użytkownicy zaznacz pole wyboru obok użytkowników, których chcesz usunąć.
2. Kliknij przycisk **Usuń z firmy** u góry.

:::note
Notatka: po usunięciu użytkownicy mogą zostać ponownie zaproszeni do Twojego abonamentu jako członkowie lub na tablicę jako goście przez każdą osobę posiadającą uprawnienia do [dodawania nowych użytkowników](05-manage-user-invitations-on-enterprise-plan.md).
:::
