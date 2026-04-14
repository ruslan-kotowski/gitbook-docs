---
title: "Miro Connector f\xFCr Okta-Workflows"
article_id: 8264504421394
translation_id: 8264504421394
locale: de
sidebar_position: 1
created_at: '2022-10-25T14:04:07Z'
updated_at: '2025-02-26T12:20:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Konfiguriere den Miro Connector für Okta-Workflows, um den Miro-Admin-Konnektor von deinem Okta-Workflow-Dashboard zu verwenden.

[Lies mehr über den Administrator-Konnektor und Nutzer-Konnektor in Einrichten der Workflow-Automatisierung für Okta-Workflows.](03-set-up-miro-connectors-for-okta-workflows.md)

> **Erhältlich für:** Enterprise-Preisplan
> **Verfügbar für:** Unternehmens-Admin

## Konfigurieren der Einstellungen auf Miro

### Ein Zugriffstoken generieren

1. Gehe auf deiner Miro Enterprise-Einstellungsseite zu **Apps und Integrationen** > **Enterprise Integrationen** und scrolle dann nach unten zu **Okta Workflows**.

2. 2. Um **Okta-Workflows** zu aktivieren, klicke auf die entsprechende Umschaltfläche.

![okta-workflows-turn-on.pngOkta](images/24938313826706_okta-workflows-turn-on.png)
*Workflows in Miro Enterprise Integrationen Einstellungen*

3. 3. Um das Zugriffstoken zu kopieren, klicke auf **Kopieren**.

4. 4. Um ein neues Zugriffstoken zu generieren, klicke auf **Neues Token generieren**.

![okta-workflows-enablement.pngZugangstoken](images/24938321779090_okta-workflows-enablement.png)

:::warning
Wenn die Umschaltfläche bereits von einem anderen Unternehmens-Admin aktiviert wurde, kannst du das Token nicht kopieren. Du kannst nur die Integration deaktivieren.
:::

:::warning
Die Integration wird mit dem Team mit der größten Anzahl von Nutzern verbunden. Es ist nicht möglich, ein anderes Team auszuwählen. Die Integration funktioniert jedoch für alle Teams innerhalb deines Enterprise-Preisplans, und die integrationsrelevanten Ereignisse werden für den gesamten Preisplan in deinen Audit-Protokollen angezeigt.
:::

## Konfigurieren der Einstellungen in Okta-Workflows

### Eine neue Verbindung erstellen

1. 1. Gehe auf deinem Okta-Workflows-Dashboard zu **Verbindungen**.

2. 2. Klicke auf die Schaltfläche **+ neue Verbindung**.

3. 3. Wähle im Dialog **Neue Verbindung** den Konnektor **Miro-Admin** aus.

![Miro-Administrator-connection.pngMiro](images/16976216641682_Miro-Administrator-connection.png)
*Administration Connector*

4. 4. Füge deine **Organisations-ID** und dein **Zugriffstoken** in die entsprechenden Eingabefelder des Dialogs ein.

5. **Klicke auf** Erstellen.

![Paste-org-ID-and-access-token-click-create.pngErstellen](images/16976235895826_Paste-org-ID-and-access-token-click-create.png)
*eines neuen Connectors*

6. Nachdem du die neu erstellte Verbindung eingerichtet hast, kannst du mit der Erstellung von Okta-Workflows beginnen.
