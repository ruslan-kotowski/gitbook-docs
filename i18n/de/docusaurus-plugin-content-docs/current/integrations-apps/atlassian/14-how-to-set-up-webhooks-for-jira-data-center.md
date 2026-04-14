---
title: So richtest du Webhooks für Jira Data Center ein
article_id: 360017731113
translation_id: 8531848266898
locale: de
sidebar_position: 15
created_at: '2022-11-11T17:31:53Z'
updated_at: '2026-01-14T09:25:35Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Personen: Jira Systemadministratoren Preispläne: Alle Miro-Preispläne (für
    die Integration von Jira Server/Data Center über OAuth 1.0) Plattformen: Browser,
    Desktop-App (für die Einrichtungsschritte)'
---

Um sicherzustellen, dass Ihre [Jira-Karten](https://help.miro.com/hc/articles/360017572434) auf einem Miro-Board aktuell bleiben, muss Miro Nachrichten von Jira erhalten, wann immer Datenänderungen auftreten. Diese Jira-Ereignisse werden in Miro über ein Webhook übertragen.

Diese Anleitung bietet zwei Möglichkeiten, Webhooks für Jira Server und Jira Data Center unter Verwendung von OAuth 1.0 und OAuth2.0 zu erstellen.

## Webhook automatisch erstellen

Beim [Einrichten deiner Jira-Karten-Integration](https://help.miro.com/hc/articles/360019501754), wenn du eine Verbindung zu Jira Server oder Jira Data Center herstellst, kannst du die Option **Webhook automatisch erstellen** aktiviert lassen. Dies ist die empfohlene Methode.

:::note
Für die automatische Webhook-Erstellung musst du bei Jira als Admin angemeldet sein.
:::

![jira-webhooks-server-config.png](../../../../../../docs/integrations-apps/atlassian/images/21304245707026_jira-webhooks-server-config.png)
*Jira-Karteneinstellungen, Schritt 2: „Webhook automatisch erstellen**“** ist aktiviert*

Nachdem der Webhook automatisch erstellt wurde, ist es ratsam, auf die WebHooks-Seite in Jira zu gehen und den Webhook zu bearbeiten, um ihm einen eindeutigen Namen zu geben. Dies ist besonders wichtig, wenn du vorhast, mehrere Miro-Teams mit deiner Jira-Instanz zu verbinden.

:::note
Bei OAuth2.0-Verbindungen wird die Verbindung auf der Miro-Seite unternehmensebene eingerichtet. Ein Webhook wird für alle Miro-Teams erstellt.
:::

:::note
Bei OAuth 1.0-Verbindungen auf Team-Ebene wird pro Miro-Team ein Webhook erstellt. Auf Unternehmensebene wird ein Webhook für alle Teams erstellt.
:::

## Webhook manuell erstellen

Wenn du den Webhook lieber manuell erstellen möchtest oder musst, gehe wie folgt vor.

**Erhalte die Webhook-URL von Miro**

1. Deaktiviere in den Jira-Karten-Einstellungen in Miro (Schritt 2, beim Verbinden mit dem Jira Server/Data Center) die Option **Webhook automatisch erstellen**.
2. Kopiere und füge die **Jira-URL** deiner Organisation ein und klicke auf **Verbinden und Einstellungen speichern.**
   ![jira-webhooks-configure-jira-url-cropped.png](../../../../../../docs/integrations-apps/atlassian/images/21304245708818_jira-webhooks-configure-jira-url-cropped.png)
   *Jira-Karten-Einstellungen, Schritt 2: "Webhook automatisch erstellen" ist deaktiviert*
3. Erlaube der Integration, in Jira eine Verbindung herzustellen, wenn du dazu aufgefordert wirst.
4. Nach diesen Schritten stellt Miro dir die **Webhook-URL** zur Verfügung:
   ![webhook_URL.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016928565010_webhook%20URL.jpg)*Vom Miro bereitgestellte Webhook-URL*

:::note
Wenn du kein Jira-Admin bist, kopiere bitte die von Miro bereitgestellte **Webhook-URL** und sende sie an deinen Jira-Admin, damit er den Webhook auf der Jira-Seite gemäß den unten stehenden Anweisungen erstellen kann.
:::

**Webhook in Jira erstellen**

Unten findest du die Schritte zur Erstellung eines Webhooks in Jira unter Verwendung der von Miro erhaltenen URL. Du kannst dich auch auf die offizielle Atlassian-Dokumentation für [Jira Server](https://developer.atlassian.com/server/jira/platform/webhooks/) und für [Jira Cloud](https://developer.atlassian.com/cloud/jira/platform/webhooks/) beziehen (obwohl sich dieser Artikel auf Server/Data Center konzentriert).

1. Um zur Seite **WebHooks** in Jira zu navigieren, gehe zu **Jira-Verwaltung** > **System** > **Erweitert >** **WebHooks** (der genaue Pfad kann je nach Jira-Version leicht variieren). Alternativ kannst du oft einen direkten Link verwenden, indem du `/plugins/servlet/webhooks` an die URL deiner Jira-Instanz anhängst (z. B. `https://YourJiraInstanceName/plugins/servlet/webhooks`).
2. Klicke oben rechts auf der WebHooks-Seite auf **Webhook erstellen**.
3. Gib einen beschreibenden **Namen** für den WebHook ein (z. B. "Miro Integration Webhook").
4. Setze den WebHook-Status auf **Aktiviert**.
5. Füge die aus den Miro-Einstellungen kopierte **WebHook-URL** in das URL-Feld ein.
   ![system_webhooks.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941532050_system%20webhooks.jpg)
   *System-WebHooks-Konfiguration in Jira*
6. Wähle im Abschnitt **Ereignisse** unter **Vorgang** die Ereignisse **aktualisiert** und **gelöscht** aus.
7. Klicke auf **Erstellen**, um den Webhook zu speichern.
   ![Jira_Webhook_settings.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016941533074_Jira%20Webhook%20settings.jpg)
   *Jira-WebHook-Ereigniseinstellungen*
8. Nachdem der Webhook in Jira erstellt wurde, kehre zu **Schritt 2** in den Jira-Karteneinstellungen in Miro zurück. Stelle sicher, dass deine **Jira-URL** korrekt eingetragen ist, und klicke auf **Verbinden**.

Der Webhook ist nun erstellt und konfiguriert. Jira-Karten auf deinen Miro-Boards werden automatisch aktualisiert, wenn Änderungen in Jira vorgenommen werden.
