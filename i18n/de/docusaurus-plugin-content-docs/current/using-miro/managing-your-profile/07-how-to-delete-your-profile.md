---
title: So löschst du dein Profil
article_id: 360017571354
translation_id: 360017571354
locale: de
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
  notes: 'Einrichtung durch: Profileigentümer'
---

Wenn du dein Profil bei Miro löschst, werden deine Daten aus unserem System entfernt. Bitte beachte, dass ein Profilund ein Team zwei verschiedene Dinge sind.

- Dein Profil enthält die Daten, die mit deiner Registrierungs- und E-Mail-Adresse verbunden sind.
- Ein Team ist ein Bereich, dem du zusammen mit anderen Teammitgliedern angehörst und in dem Mitglieder Inhalte erstellen und Boards speichern können.

Jedes Profil kann mit mehreren Teams verknüpft werden. [Hier](../../administration/team-management/06-delete-and-restore-teams.md) findest du heraus, wie du ein Team entfernen kannst.
:::warning
Das Löschen deines Profils kann **nicht** rückgängig gemacht werden.
:::

:::warning
Hinweis: Durch das Löschen deines Profils werden keine deiner aktiven Abos gekündigt. Wenn du die Verlängerungen stoppen möchtest, [kündige dein Abonnement in den Einstellungen](../../plans-billing/manage-your-subscription-and-plan/06-cancel-your-miro-subscription.md).
:::

### So löschst du dein Profil

1. Öffne deine [Profileinstellungen](https://miro.com/app/settings/user-profile/).

2. Scrolle zum Ende der Seite und wähle **Mein Profil löschen.**

![Delete_profile.png](../../../../../../docs/using-miro/managing-your-profile/images/21017429126546_Delete%20profile.png)
*Löschen deines Profils*

3. An dieser Stelle empfehlen wir, [Backups](../import-and-export/export/05-how-to-save-board-backup.md) zu speichern oder deine Boards zu [exportieren](../import-and-export/export/03-how-to-export-your-board.md), bevor du sie löschst.

![profile_removal_modal.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017429125778_profile%20removal%20modal.jpg)*Nachricht zur Bestätigung der Profilentfernung*

4. Kurze Zeit später erhältst du eine E-Mail mit einem Bestätigungslink. Klicke auf den Link, um den Vorgang abzuschließen. Bitte beachte, dass du in deinem Miro-Profil im Browser angemeldet sein musst, wenn du auf **Profil löschen** klickst, um die Profillöschung erfolgreich abzuschließen.

![Profile_deletion_email.jpg](../../../../../../docs/using-miro/managing-your-profile/images/21017416055186_Profile%20deletion%20email.jpg)
*Bestätigungs-E-Mail zum Löschen des Profils*

### Was mit deinen Inhalten passiert, wenn das Profil gelöscht wurde

Sobald du dein Profil löschst, werden auch deine Boards gelöscht.

Wenn du der einzige Admin für dein Team bist, wird der Inhalt *komplett* entfernt. Die Admin-Rechte werden dem Mitglied gewährt, das zuerst eingeladen wurde.

Gibt es andere Admins in dem Team, in dem du Mitglied bist, werden die Inhalte gelöscht und einem der anderen Admins zugewiesen – das bedeutet, dass der Admin [deine Boards innerhalb von 90 Tagen wiederherstellen](../managing-boards/08-how-to-restore-a-deleted-board.md) kann (Nutzer in einem kostenpflichtigen Preisplan finden sie im Papierkorb, Nutzer in einem kostenlosen Preisplan können sie über den Link wiederherstellen).

### Häufige Fragen

1. *Kann ich mein Profil löschen, wenn ich mich mit [Single Sign-on (SSO)](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) in Miro anmelde?*
   - Ja, das kannst du. Wenn dein Unternehmen jedoch [SCIM](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) verwendet, wird dein Profil sofort neu erstellt, solange deine E-Mail-Adresse über SCIM für Miro bereitgestellt wird.
2. *Wie kann ich meine E-Mail-Adresse ändern, die mit dem Miro Profil verknüpft ist?*
   - Folge dazu dieser Anleitung: [So änderst du deine E-Mail-Adresse](04-how-to-change-your-email.md).
3. *Ich erhalte die E-Mail-Adresse mit dem Bestätigungslink nicht. Was muss ich tun?*
   - Bitte versuche Folgendes:

- Öffne deine Ordner  **Spam, Werbung,****Junk, Social** und **Updates** und sieh nach, ob die Bestätigungs-E-Mail von Miro dort gelandet ist.
- Überprüfe, ob dein Posteingang voll ist, um sicherzustellen, dass du das Speicherlimit deines E-Mail-Postfachs nicht erreicht hast. Wenn er voll ist, musst du eventuell einige bestehende E-Mails löschen, um neue zu erhalten. Wenn du E-Mails gelöscht hast, sende erneut eine Anfrage zur Löschung deines Profils.
- Es kann sein, dass eine Firewall verhindert, dass die E-Mail-Adresse deinen Posteingang erreicht. Bitte deinen *Systemadministrator*, unsere Domains und Subdomains in die Zulassungsliste aufzunehmen: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) und [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Hier ist ein Artikel](../tools/troubleshooting/02-allowlist-miro-mailers.md) mit weiteren Informationen zu den Mailern, die du in deine Zulassungsliste aufnehmen musst.
- Wenn keine der Lösungen hilfreich war, [melde das Problem bitte dem Support von Miro](../tools/troubleshooting/06-contacting-miro-support.md).
