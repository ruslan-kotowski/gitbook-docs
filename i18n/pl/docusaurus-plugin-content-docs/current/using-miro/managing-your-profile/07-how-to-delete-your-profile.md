---
title: Jak usunąć profil
article_id: 360017571354
translation_id: 360017571354
locale: pl-pl
sidebar_position: 7
created_at: '2019-02-11T10:08:54Z'
updated_at: '2026-01-07T13:30:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
availability:
  notes: 'Konfiguracja: właściciel profilu'
---

Usunięcie profilu w Miro spowoduje usunięcie Twoich informacji z naszego systemu. Pamiętaj, że profil izespół to dwie różne rzeczy.

- Twój profil reprezentuje dane połączone z Twoją rejestracją i adresem e-mail.
- Zespół to przestrzeń, do której należysz, wraz z innymi uczestnikami zespołu, w której uczestnicy mogą tworzyć treści i przechowywać swoje tablice.

Każdy profil może być powiązany z kilkoma zespołami. Jeśli chcesz usunąć zespół, dowiedz się, jak to zrobić [tutaj](../../administration/team-management/06-delete-and-restore-teams.md).
:::warning
Usunięcia profilu **nie** można cofnąć.
:::

:::warning
Pamiętaj, że usunięcie profilu nie anuluje aktywnych subskrypcji. Aby zatrzymać dalsze odnawianie, [anuluj subskrypcję w ustawieniach](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md).
:::

### Jak usunąć profil

1. Otwórz [ustawienia profilu](https://miro.com/app/settings/user-profile/).

2. Przewiń na dół strony i wybierz **Usuń mój profil.**

![Delete_profile.png](../../../../../../docs/using-miro/managing-your-profile/images/21017429126546_Delete%20profile.png)
*Usuwanie profilu*

3. W tym momencie sugerujemy zapisanie [kopii](../import-and-export/export/05-how-to-save-board-backup.md) zapasowych lub [eksportowanie](../import-and-export/export/03-how-to-export-your-board.md) tablic przed ich usunięciem.

![profile_removal_modal.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017429125778_profile%20removal%20modal.jpg)*Wiadomość potwierdzająca usunięcie profilu*

4. Wkrótce potem otrzymasz wiadomość e-mail z linkiem potwierdzającym. Kliknij link, aby zakończyć. Pamiętaj, że musisz być zalogowany do swojego profilu Miro w przeglądarce po kliknięciu **Usuń** profil, aby pomyślnie zakończyć usunięcie profilu.

![Profile_deletion_email.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017416055186_Profile%20deletion%20email.jpg)
*Wiadomość e-mail z potwierdzeniem służąca do usunięcia profilu*

### Co stanie się z treściami po usunięciu profilu

Po usunięciu profilu tablice zostaną usunięte.

Jeśli jesteś jedynym administratorem zespołu, zawartość zostanie *całkowicie* usunięta. Uprawnienia administratorów będą przyznawane uczestnikowi, który został najpierw zaproszony chronologicznie.

Jeśli w zespole są inni administratorzy, których jesteś członkiem, treści zostaną usunięte i ponownie przypisane do jednego z administratorów. Oznacza to, że administrator będzie mógł [przywrócić tablice w ciągu 90 dni](../managing-boards/08-how-to-restore-a-deleted-board.md) (płatni użytkownicy znajdą je w Koszu, użytkownicy bezpłatni będą mogli przywrócić je przez link).

### Często zadawane pytania

1. *Czy mogę usunąć mój profil, jeśli zaloguję się do Miro za pomocą [pojedynczego logowania (SSO)](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)?*
   - Tak, możesz. Jeśli jednak Twoja organizacja używa [SCIM](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md), Twój profil zostanie natychmiast ponownie utworzony, dopóki Twój adres e-mail zostanie przekazany do Miro za pośrednictwem SCIM.
2. *Jak zmienić adres e-mail połączony z profilem Miro?*
   - Skorzystaj z tego przewodnika: [Jak zmienić adres e-mail](04-how-to-change-your-email.md).
3. *Nie otrzymuję wiadomości e-mail z linkiem potwierdzającym. Co mam zrobić?*
   - Wykonaj następujące czynności:

- Otwórz foldery **Spam, Promocje,** **Wiadomości, Społeczności** i **Aktualizacje,** i sprawdź, czy jest tam wiadomość e-mail z potwierdzeniem Miro.
- Sprawdź, czy skrzynka odbiorcza jest pełna, aby upewnić się, że nie osiągnięto limitu pamięci za pomocą skrzynki odbiorczej. Jeśli jest pełna, może być konieczne usunięcie niektórych istniejących wiadomości e-mail, aby otrzymywać nowe. Po usunięciu wiadomości e-mail ponownie poproś o usunięcie profilu
- Może się okazać, że zapora sieciowa uniemożliwia dotarcie wiadomości e-mail do skrzynki odbiorczej. Skontaktuj się z *administratorem systemu* i poproś o dodanie dozwolonych domen i subdomen: [miro.com*,](http://miro.com/) *.miro.com, [mirostatic.com,](http://mirostatic.com/) [*.mirostatic.com](http://mirostatic.com/) i realtimeboard.com*, *.realtimeboard.com. [Tutaj znajduje się artykuł](../tools/troubleshooting/02-allowlist-miro-mailers.md) zawierający więcej informacji na temat listy dozwolonych adresów.
- Jeśli żadne z rozwiązań nie [pomoże,zgłoś problem do pomocy technicznej Miro](../tools/troubleshooting/06-contacting-miro-support.md)
