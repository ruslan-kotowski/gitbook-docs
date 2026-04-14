---
title: Miro-Boards in Microsoft Teams einbetten
article_id: 360017572514
translation_id: 360017572514
locale: de
sidebar_position: 5
created_at: '2019-02-11T10:13:30Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
---

Integriere Miro-Boards in Microsoft Teams-Kanäle, um sie nahtlos mit Teammitgliedern zu teilen. Dadurch stehen deine Miro-Boards stets bereit und du kannst sicher sein, dass dein gesamtes Team denselben Wissensstand hat und abgestimmt ist.

:::note
Überprüfe, wie du Miro-Boards in Microsoft Teams Meetings einbetten kannst: [Miro für Microsoft Teams Meetings (Admin-Anleitung)](01-miro-for-microsoft-teams-admin-guide.md), [Miro für Microsoft Teams Meetings (Nutzer-Anleitung)](02-miro-for-microsoft-teams-user-guide.md).
:::

> **Erhältlich für:** alle Miro-Preispläne

### Plugin-Installation

Zunächst musst du **Miro** im **Microsoft Teams Store** finden. Du kannst auch einfach dem [direkten Link](https://teams.microsoft.com/l/app/8216e453-3db5-48ee-a3d6-5122f505c8a3) folgen.

:::warning
Bitte beachte, dass dein Mandanten-Admin auf der Microsoft Teams-Seite die Miro-App in deinem Drittanbieter-App-Katalog für Teams aktivieren sollte. Wenn Miro nicht genehmigt ist, wird es auch nicht unter den Apps im Microsoft Teams Store aufgeführt.
:::

Klicke auf **Hinzufügen**, um das Plugin zu installieren.

![Miro_plugin_installation.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790725266_Miro%20plugin%20installation.jpg)
Installation des Miro-Plugins

Wenn du das Miro-Plugin installiert hast, wirst du zum Chat weitergeleitet, wo du den Erhalt von Miro-Benachrichtigungen konfigurieren kannst. Weitere Informationen findest du in [diesem Artikel](10-miro-notifications-in-microsoft-teams.md).

Zu diesem Zeitpunkt kannst du aber bereits mit der Integration von Miro-Whiteboards in einen Microsoft Teams-Kanal beginnen, ohne dass weitere Konfigurationsschritte notwendig wären.

### Whiteboards in Microsoft Teams-Kanäle integrieren

> **Einrichtung durch:** [Board-Eigentümer](../../../using-miro/sharing-boards/01-board-access-rights.md) und [Board-Bearbeiter](../../../using-miro/sharing-boards/01-board-access-rights.md), die Mitglieder des Teams sind, in dem sich das Board befindet

Du kannst deine Boards in Microsoft Teams-Kanäle einbetten, indem du einen neuen Tab erstellst. Klicke auf das Plus-Symbol. Es wird eine Auswahl verschiedener Apps angezeigt. Wähle Miro aus der Liste der Apps aus. Wenn du nicht in Miro im gleichen Browser oder in der Desktop-App autorisiert bist, musst du dich anmelden. Klicke auf **Erste Schritte** und melde dich an oder [registriere dich bei Miro](../../../getting-started/start-here/02-how-to-register-with-miro.md).

![embed_in_MS_teams.gif](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734975122_embed%20in%20MS%20teams.gif)
Das Dialogfeld, in dem du aufgefordert wirst, dein Miro-Profil zu autorisieren

Nach der Autorisierung wird eine Auswahl von Miro-Boards angezeigt. Hier findest du nur die Boards, auf die du vonseiten Miro Zugriff hast. Bitte beachten: Du kannst in Miro und in Microsoft Teams unter verschiedenen E-Mail-Adressen autorisiert sein.

Wähle ein Board, das du deinem Microsoft Teams-Kanal hinzufügen möchtest.

![MS_teams_embed_picker.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734978322_MS%20teams%20embed%20picker.jpg)
Die Board-Auswahl von Miro

Beachte, dass nur Board-Eigentümer und Board-Bearbeiter, die Team-Mitglieder sind, Miro-Boards einbetten können. Wenn du ein Whiteboard wählst, für das du nicht die erforderliche Zugriffsberechtigung hast, wird eine Warnmeldung angezeigt.

![unable_to_embed_boards.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790732690_unable%20to%20embed%20boards.jpg)
Die Warnmeldung, dass deine Zugriffsebene dir nicht gestattet, ein Board zu integrieren

Du kannst als Nächstes Berechtigungen für die restlichen Meeting-Teilnehmer festlegen und ihnen Zugriff auf das Board gewähren oder diesen beschränken. Du hast die Wahl unter folgenden Berechtigungen:

- **Alle können bearbeiten** (keine Anmeldung erforderlich)
- **Alle können kommentieren** (keine Anmeldung erforderlich)
- **Alle können anzeigen** (keine Anmeldung erforderlich)
- **Privat**

![sharing_level.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019790733586_sharing%20level.jpg)
*Zugriffseinstellungen für ein eingebettetes Board*

:::note
Beachte, dass die Freigabeeinstellungen, die für ein Board in Miro festgelegt werden, auch den Zugriff auf das Board innerhalb von Microsoft Teams bestimmen können. Wenn das Board in Miro öffentlich freigegeben wird, ist es für jeden in Microsoft Teams verfügbar, auch wenn du das Board als **Privat** eingebettet hast. Wenn dein Board jedoch ein [privat](../../../using-miro/sharing-boards/15-make-a-miro-board-private.md) auf der Miro-Seite ist und du es mit **Anyone can view/comment/edit** access einbettest , wird der Zugriff auf das Board in Miro nicht beeinträchtigt. [Mehr erfahren](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).
:::

:::note
Für [Enterprise-Preisplan](../../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md) Miro-Nutzer folgen deine Zugriffseinstellungen den organisationsweiten Zugriffskontrollen, was bedeuten kann, dass einige Freigabeoptionen eingeschränkt sind. Mehr erfährst du unter [Verwalten der Freigaberichtlinie bei Enterprise-Preisplänen für die Einbettungsintegrationen](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

:::warning
Die Option " **Jeder kann kommentieren"** wird nicht unterstützt, wenn du ein Board einbettest, das sich in einem [freien Team](../../../plans-billing/miro-plans/09-free-plan.md) befindet.
:::

Sobald das Board eingebettet wurde, kannst du damit arbeiten.

![Miro_embed_in_MS_teams.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734972562_Miro%20embed%20in%20MS%20teams.jpg)
In einen Microsoft Teams-Kanal eingebettetes Board

:::note
Nutzer von Microsoft Teams, die Miro in der mobilen App von Microsoft Teams verwenden, können Boards *ansehen und kommentieren*, je nach den festgelegten Berechtigungen. Für die Bearbeitung von Boards empfehlen wir Nutzern dringend, unsere native [mobile App](../../../getting-started/apps-for-devices/08-mobile-app.md) zu installieren, für die wir die Benutzeroberfläche optimiert haben.
:::

![Miro_in_MS_Team_on_mobile.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21019734976146_Miro%20in%20MS%20Team%20on%20mobile.jpg)
*Miro-Board in MS Teams auf einem Mobiltelefon – Tippe auf **In der App öffnen**, um die native mobile App von Miro zu installieren*

### Häufige Fragen

1. *Muss jedes Teammitglied ein Miro-Profil haben, um eingebettete Boards in Microsoft Teams ansehen zu können?*
   - Wenn du beim Einbetten des Boards die Option **Alle können das Board ansehen/kommentieren/bearbeiten** wählst, können auch nicht registrierte Nutzer das Board ansehen/kommentieren. Wenn das Board außerdem auf der Miro-Seite [öffentlich freigegeben](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) wird, ist es für alle in Microsoft Teams verfügbar.
2. **Wer kann nach dem Einbetten eines Boards den Zugriff auf das Board in MS Teams ändern (z. B. von "Jeder kann es ansehen" auf "Privat")?**
   - Niemand kann den Zugriff auf das angehängte Board ändern, nicht einmal derjenige, der es angehängt hat. Jeder kann jedoch auf dem Tab  auf **Einstellungen** klicken und dann ein anderes (oder dasselbe) Board für denselben Tab auswählen und eine andere Zugriffsebene für das gewählte Board wählen.
3. **Ich bin mit zwei E-Mails bei Miro registriert und möchte ein Miro-Board von meinem zweiten Profil einbetten. Wie kann ich das Profil von Miro wechseln?**
   - Der Picker zeigt Boards des Nutzers, mit dem du in Miro berechtigt bist, im selben Browser an. Öffne Miro in einem anderen Tab deines Browsers, melde dich ab und melde dich bei deinem zweiten Profil in Miro an.
   Wenn du die Microsoft Teams Desktop-App verwendest, melde dich von der App ab – damit meldest du dich auch von Miro innerhalb der App ab. Melde dich dann in der App an und versuche, [ein Board einzubetten](#h_5af20ae6-78c0-4e6c-ab20-e4968c89c97f). Du wirst aufgefordert, dich bei Miro anzumelden und kannst dich dann bei einem anderen Miro-Profil anmelden.
