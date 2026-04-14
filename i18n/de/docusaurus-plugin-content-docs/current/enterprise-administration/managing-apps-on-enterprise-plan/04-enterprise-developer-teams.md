---
title: Enterprise-Entwicklerteams
article_id: 4766759572114
translation_id: 4766759572114
locale: de
sidebar_position: 4
created_at: '2022-03-22T14:13:15Z'
updated_at: '2025-04-29T13:25:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: developer-teams
---

Entdecke die Option, Entwicklerteams innerhalb von Enterprise-Abos einzurichten – eine einfache und sichere Möglichkeit, benutzerdefinierte Apps für deinen Enterprise-Preisplan zu erstellen.

> **Verfügbar für**: [Enterprise-Preisplan](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Einrichtung durch:** Unternehmens-Admin
> Nutzer anderer Miro-Preispläne können auf [dieser Seite](https://developers.miro.com/docs/rest-api-build-your-first-hello-world-app#step-1-create-a-developer-team-in-miro) Entwickler-Teams erstellen

### Erstellen eines Entwicklerteams

Um ein Entwicklerteam einzurichten, öffne **Unternehmenseinstellungen** > **Teams** und klicke auf **Neues Team erstellen** in der oberen rechten Ecke.

Gib im nächsten Pop-up-Fenster den Teamnamen ein und [wähle die Stufe der Teamberechtigungen aus: Du kannst die Standardberechtigungseinstellungen festlegen oder ein Team auswählen, um die Teamberechtigungen zu kopieren (weitere Informationen über](../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)Berechtigungen und Standardeinstellungen).  Aktiviere das Kästchen **Entwicklerteam**, bestätige deine Berechtigung und klicke auf **Team erstellen**.

![create-dev-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803173266_create-dev-team.png)
Erstellen eines Entwicklerteams

### Berechtigungen für Enterprise-Entwicklerteams

Im Enterprise-Entwicklerteam kannst du auf sichere Weise Apps entwickeln. Es ist Teil deines Enterprise-Abos und gibt dir Zugriff auf alle Enterprise-Sicherheitsfunktionen.

Das Enterprise-Entwicklerteam verfügt über eine unbegrenzte Anzahl von Boards und eine unbegrenzte Anzahl von Mitgliedern.

Im Team erstellte Boards werden mit einem Wasserzeichen versehen, um sie von anderen Teams in der Organisation zu unterscheiden.

Das Team verfügt über alle Standardeinstellungen zur Konfiguration von Nutzerberechtigungen im Enterprise-Preisplan: Du kannst Teammitgliedern erlauben/verbieten, neue Personen einzuladen, Boards mit dem Team/der Firma/über einen öffentlichen Link teilen, Boards verschieben, erlaubte Domains einschränken usw. Weitere Informationen findest du [in diesem Artikel](../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md).

### Erstellen und Installieren von Apps

> **Einrichtung durch:** Team-Admins
> Wenn du Entwickler einladen möchtest, eine App im Team zu erstellen, musst du [Team-Admin-Berechtigungen erteilen](../../administration/user-management/06-how-to-manage-admin-roles.md)

[Um eine neue Anwendung in deinem Miro-Enterprise mit dem Enterprise-Entwicklerteam zu erstellen, gehe zu](../../using-miro/managing-your-profile/01-profile-settings.md) ****Profileinstellungen** > Deine Apps****, stimme den Bedingungen und Konditionen zu und klicke auf** Neue App erstellen.

![profil-erstelle-neue-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780634770_profile-create-new-app.png)
Deine Apps in den Profileinstellungen

:::tip
Du kannst die Seite auch aufrufen, indem du oben rechts im Dashboard des Developer Teams auf **Build an app** klickst.
:::

![dev-team-build-an-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780641298_dev-team-build-an-app.png)
Die Option zum Erstellen neuer benutzerdefinierter Apps

**Gib den Namen der App ein, wähle dein Entwicklerteam für die Anwendung aus und klicke auf** App erstellen.

create_a_new_app.jpg
Erstellen einer neuen App für das Enterprise-Entwicklerteam

**Scrolle auf der App-Seite nach unten und wähle den Zugriffsbereich aus, den du deiner App gewähren möchtest. Klicke dann auf** App installieren und rufe den OAuth Token ab.

app_permissions.jpg
App-Berechtigungen

Wähle bei der Installation der App ein Team (das sich vom Entwicklerteam unterscheidet) aus deiner Enterprise-Organisation aus und klicke auf **Installieren & autorisieren**. Der Zugriffstoken wird im nächsten Schritt angezeigt.

installing_the_app.jpg
Installieren der App

### Löschen eines Entwicklerteams

Du kannst das Entwicklerteam wie jedes andere Team in deiner Enterprise-Organisation löschen, aber du musst zuerst alle Apps löschen, die unter diesem Team erstellt wurden. Sobald die Apps gelöscht sind, navigiere zu [**Teams**](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md), klicke auf den Namen des Teams, wähle den Tab **Profil** und dann **Team löschen**.

:::warning
Bitte beachte, dass nach dem Löschen des Enterprise-Entwicklerteams alle mit ihm verbundenen Token nicht mehr gültig sind.
:::

![delete-dev-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803181586_delete-dev-team.png)*Das Enterprise Developer Team löschen*
