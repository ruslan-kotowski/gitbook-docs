---
title: Zarządzanie usuwaniem i przywracaniem zespołu
article_id: 360017571334
translation_id: 360017571334
locale: pl-pl
sidebar_position: 6
created_at: '2019-02-11T10:08:51Z'
updated_at: '2025-11-25T15:58:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: deleted-teams
availability:
  notes: 'Dostępne dla: administratorów zespołu, administratorów użytkowników i administratorów
    firmy'
---

### Usuwanie zespołu

:::note
Pamiętaj, że [zespół](../../getting-started/start-here/miro-dashboard/01-what-is-on-your-dashboard.md) w Miro i Twój [profil](https://miro.com/app/settings/user-profile/) (dane użytkownika i adres e-mail, z którym połączone są wszystkie zespoły) to nie to samo. Jeśli chcesz usunąć profil, zapoznaj się z [tym artykułem](../../using-miro/managing-your-profile/07-how-to-delete-your-profile.md).
:::

:::warning
Pamiętaj, że w wersji Enterprise administratorzy **nie są proszeni o potwierdzenie** usunięcia, a sugestia zapisania kopii zapasowej to ostatni etap procesu.
:::

Usuwać zespoły mogą administratorzy zespołu i firmy. Usunięcie zespołu spowoduje **usunięcie wszystkich tablic i szablonów**. Aby odzyskać przypadkowo usunięte tablice, zapoznaj się z instrukcjami podanymi w [artykule dotyczącym zarządzania koszem](../../using-miro/managing-boards/09-trash-management.md). Przed usunięciem zespołu dobrze jest [przenieść tablice](../../using-miro/managing-boards/04-how-to-move-a-board.md) do innych zespołów, [zapisać ich kopie zapasowe](../../using-miro/import-and-export/export/05-how-to-save-board-backup.md) lub je [wyeksportować](../../using-miro/import-and-export/export/03-how-to-export-your-board.md) i poprosić uczestników zespołu o to samo.

Aby usunąć zespół:

1. Przejdź do Ustawień profilu Miro (Na tablicy kliknij ikonę **Ustawienia** obok nazwy tablicy. Na pulpicie nawigacyjnym Miro kliknij awatar i wybierz **Ustawienia)**.
2. Na panelu po lewej stronie kliknij **Zespoły**.
3. Kliknij zespół, który chcesz usunąć.
4. Na panelu po lewej stronie kliknij **Profil zespołu**.
5. Kliknij przycisk **Usuń zespół**.![manage_team_deletion_delete_team_option.png](images/21358631043090_manage_team_deletion_delete_team_option.png)*Usuwanie zespołu za pomocą sekcji Profil zespołu*
6. Potwierdź wybór, klikając **Usuń zespół**. Pamiętaj, że wszystkie tablice powiązane z tym zespołem również zostaną usunięte. ![managing_team_deletion_delete_confirmation.png](../../../../../../docs/administration/team-management/images/21019693273234_managing_team_deletion_delete_confirmation.png)*Wiadomość z potwierdzeniem usunięcia zespołu*
7. Jeśli Twoja organizacja obejmuje tylko jeden zespół, otrzymasz wiadomość e-mail z linkiem potwierdzającym, aby zakończyć proces. Kliknij link **Usuń mój zespół**, aby zakończyć.
   ![managing_team_deletion_email_message.png](images/21358673581330_managing_team_deletion_email_message.png)*Wiadomość e-mail z potwierdzeniem usunięcia zespołu*

## Przywracanie lub trwałe usunięcie zespołu

> **Dostępne w wersjach:** Business, Enterprise
> **Kto może to zrobić:** administratorzy użytkowników, administratorzy firmy

Po usunięciu zespołu możesz go odzyskać lub trwale usunąć. Jeśli nic nie zrobisz, zespół zostanie automatycznie usunięty po 90 dniach.

Przywrócenie usuniętego zespołu spowoduje również przywrócenie wszystkich tablic lub szablonów, które zostały usunięte wraz z zespołem.

Trwałe usunięcie zespołu spowoduje również trwałe usunięcie wszystkich tablic lub szablonów utworzonych przez jego uczestników. Tego działania nie można cofnąć.

### Przywracanie usuniętego zespołu

1. W panelu ustawień Firmy kliknij **Zespoły**.
2. W panelu Zespoły kliknij kartę **Usunięte**.
3. Znajdź zespół, który chcesz odzyskać. Możesz przewijać listę lub użyć paska wyszukiwania, aby znaleźć zespół.
4. Kliknij „**…**” obok zespołu i wybierz **Przywróć zespół**.
5. Zespół zostanie przeniesiony z powrotem do karty Aktywne, a wszystkie tablice lub szablony zostaną przywrócone![deleted_teams_restore_team.gif](images/21358673581842_deleted_teams_restore_team.gif)*Przywracanie usuniętego zespołu*

### Trwałe usunięcie zespołu

1. W panelu ustawień Firmy kliknij **Zespoły**.
2. W panelu Zespoły kliknij kartę **Usunięte**.
3. Znajdź zespół, który chcesz usunąć. Możesz przewijać listę lub użyć paska wyszukiwania, aby znaleźć zespół.
4. Kliknij „**…**” obok zespołu i wybierz **Usuń trwale**.
5. Zostanie wyświetlona prośba o potwierdzenie tego wyboru poprzez zaznaczenie pola Usuń „[nazwa zespołu]”, a następnie kliknięcie **Usuń trwale**.*![deleted_teams_delete_permanently.gif](images/21358631048210_deleted_teams_delete_permanently.gif)**Trwałe usunięcie zespołu*

## Usuwanie ostatniego zespołu w wersji Business

Nie można usunąć ostatniego zespołu w ramach subskrypcji Business. Zamiast tego zobaczysz komunikat ostrzegawczy: **Nie można usunąć ostatniego zespołu w organizacji**.

Możesz użyć następującego sposobu w celu obejścia tego problemu:

1. [Anuluj subskrypcję](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md).
2. Gdy zespół wygaśnie z końcem okresu rozliczeniowego, [przejdź na wersję Free](../../plans-billing/manage-your-subscription-and-plan/04-downgrade-your-plan.md).
3. Usuń bezpłatny zespół.

W przypadku wersji Enterprise [skontaktuj się z pomocą techniczną](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).

## Często zadawane pytania

Czy subskrypcja związana z moim zespołem zostanie zakończona w momenie usunięcia zespołu?

Aby upewnić się, że nie będą naliczane żadne dodatkowe opłaty, anuluj subskrypcję w sekcji z ustawieniami rozliczeń: skorzystaj z [tego przewodnika](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md).

Jakiego rodzaju uprawnienia są potrzebne, aby usunąć zespół?

Usunięcie zespołu wymaga uprawnień administratora firmy. Jeśli nie jesteś administratorem firmy, zobaczysz opcję [opuszczenia zespołu](../../using-miro/managing-your-profile/06-how-to-leave-a-team.md).

Po zgłoszeniu prośby o usunięcie zespołu nie przyszła wiadomość e-mail z potwierdzeniem. Jak znaleźć tę wiadomość e-mail?

Otwórz foldery **Spam, Oferty,** **Kosz, Społeczności** oraz **Powiadomienia** i sprawdź, czy nie ma tam wiadomości e-mail z potwierdzeniem.
Może się również zdarzyć, że zapora sieciowa uniemożliwia wiadomości dotarcie do skrzynki odbiorczej. Skontaktuj się z administratorem systemu i poproś o dodanie naszej domeny i subdomen do listy dozwolonych. [Tutaj znajdziesz](../../using-miro/tools/troubleshooting/02-allowlist-miro-mailers.md) więcej informacji na temat dodawania nadawców do listy dozwolonych.

:::note
Jeśli chcesz opuścić zespół, do którego masz zaproszenie, zapoznaj się z artykułem [Jak opuścić zespół](../../using-miro/managing-your-profile/06-how-to-leave-a-team.md).
:::
