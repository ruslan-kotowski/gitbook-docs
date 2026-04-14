---
title: App-Verwaltung
article_id: 4404659741458
translation_id: 4404659741458
locale: de
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

Erfahre, wie du Apps und Berechtigungen auf Organisations- und Teamebene verwaltest.

> **Relevant für:** Business-Preisplan, Enterprise-Preisplan
> **Wer kann das:** Team-Admin, Unternehmens-Admin

### Wer kann Apps verwalten?

Die App-Verwaltung auf Organisationsebene ist nur im Enterprise-Preisplan für Unternehmens-Admins verfügbar. Die App-Verwaltung auf Team-Ebene ist in Business- und Enterprise-Preisplänen für Team- und Unternehmens-Admins verfügbar.

### Hinzufügen von Apps für eine Organisation oder bestimmte Teams

Installiere und autorisiere Apps für alle Nutzer in einer Organisation oder bestimmten Teams in deiner Organisation über die App-Verwaltung.
Gehe zu **Unternehmenseinstellungen** > **Apps und Integrationen** > **Apps**. In diesem Abschnitt können Unternehmens-Admins Apps für alle oder bestimmte Teams hinzufügen.

![apps-access.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803476626_apps-access.png)*Managementsteuerung der Apps in den Unternehmenseinstellungen*

Gib einen App-Namen oder eine Client-ID in die Suchleiste ein. Wähle eine App aus der Dropdownliste aus und klicke auf **Hinzufügen**.

![add-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780909714_add-app.png)*Hinzufügen einer App über die Unternehmenseinstellungen*

Du kannst die App für alle Teams in deiner Organisation hinzufügen oder bestimmte Teams auswählen. Wenn eine App bereits für einige Teams hinzugefügt wurde, siehst du das entsprechende Tag. Wenn du die App für ein Team erneut hinzufügst, müssen Teammitglieder die App erneut autorisieren. Klicke auf **Hinzufügen**, um abzuschließen.

![add-apps-where.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780917010_add-apps-where.png)
*Auswählen, für wen die Google Drive-App installiert werden soll*

Wenn du eine App für alle Teams hinzufügst, wird die App auch für alle neu erstellten Teams hinzugefügt.

### Vorinstallierte Apps

Einige Apps sind für Nutzer bereits vorinstalliert. Es kann eine zusätzliche Genehmigung oder Anmeldung erforderlich sein. Diese vorinstallierten Apps sind: [Box](../../integrations-apps/more-integrations/05-box-legacy.md), [Dropbox](../../integrations-apps/more-integrations/06-dropbox.md), [Google Drive](../../integrations-apps/google/05-google-drive.md), [OneDrive](../../integrations-apps/microsoft/06-onedrive.md), [Smartsheet](../../integrations-apps/more-integrations/15-smartsheet-app-for-miro.md), [Azure Cards](../../integrations-apps/microsoft/03-azure-cards.md), [Jira Cards](../../integrations-apps/atlassian/03-jira-cards.md),[Brandfetch](https://miro.com/marketplace/brandfetch/), [Google Bilder](../../integrations-apps/google/06-google-images.md), [Slack](../../integrations-apps/more-integrations/14-slack.md). Diese Apps werden nicht vorab hinzugefügt, wenn sie sich nicht auf der vom Unternehmen genehmigten Liste befinden. Du kannst diese Liste verwalten, wenn du ein Unternehmens-Admin bist.

### Vorautorisierung von Apps für eine Organisation

Wenn du eine App hinzufügst, kannst du sie auch gleichzeitig vorautorisieren. Wenn eine App vorab hinzugefügt und von einem Admin vorautorisiert wurde, können die Nutzer in der Organisation sie sofort nutzen. Für bestimmte Apps kann weiterhin eine individuelle Anmeldung bei einem Drittanbieterdienst erforderlich sein.

Diese Funktion ist nur für Apps verfügbar, die mit dem Miro Web SDK erstellt wurden. Das Miro Web SDK ermöglicht die Erweiterung der Miro-Funktionalität. Es handelt sich um eine Toolbox zum Erstellen leistungsstarker Apps, die auf einem Miro-Board laufen.

### Apps für die individuelle Nutzerverwaltung genehmigen

Standardmäßig können Nutzer jede beliebige App für ihr Team hinzufügen. Unternehmens-Admins können die App-Verwaltung durch Nutzer einschränken, sodass nur bestimmte Apps von ihren Teams hinzugefügt werden können.

Unternehmens-Admins können das Hinzufügen bestimmter Apps für ihre Nutzer aktivieren oder einschränken, indem sie zu **Unternehmenseinstellungen** > **Apps und Integrationen** > **Apps** > **Apps verwalten** gehen und die Option **Mitgliedern nur das Hinzufügen von Apps aus der Liste unten erlauben** aktivieren.

![manage-apps.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780921490_manage-apps.png)*Hinzufügen genehmigter Apps im Enterprise-Preisplan einschränken*

Wenn dies eingeschränkt ist, können Enterprise-Nutzer nur die Apps hinzufügen, die genehmigt wurden. Um eine App für Nutzer freizugeben, aktiviere die Umschaltfunktion daneben oder füge eine Client-ID in das entsprechende Feld ein, um eine intern entwickelte App zu genehmigen.

Um eine zuvor hinzugefügte App einzuschränken, suche die App in der Liste und stelle sicher, dass die Umschalttaste neben der App deaktiviert ist. Bitte beachte, dass Nutzer aus allen Enterprise-Teams die App nicht nutzen können, wenn sie nicht zugelassen ist.

Wenn eine App in deiner Organisation eingeschränkt ist, können die Nutzer [Anfragen für die App-Nutzung an Unternehmens-Admins](03-app-request-flow.md) senden.

Nutzer können genehmigte Apps im Marketplace innerhalb der Miro-Boards sehen, die im Enterprise-Preisplan gespeichert sind.

### App-Nutzung in Teams erlauben oder einschränken

Team- und Unternehmens-Admins können die Verwendung von Apps auch auf Teamebene verwalten: Sie können Teammitgliedern erlauben oder verbieten, neue Apps für das Team hinzuzufügen. Die Einstellung ist für jedes Team separat konfiguriert.

![add-apps-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780928914_add-apps-team.png)*Apps & Integrationen in den Teameinstellungen*

Erfahre mehr über [Miro-Apps und Integrationen.](../../integrations-apps/integrations-basics)
