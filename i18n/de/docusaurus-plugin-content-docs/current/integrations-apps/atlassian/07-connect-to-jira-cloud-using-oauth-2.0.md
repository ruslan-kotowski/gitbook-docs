---
title: Mit Jira Cloud über OAuth 2.0 verbinden
article_id: 8588617184402
translation_id: 12813822263570
locale: de
sidebar_position: 7
created_at: '2023-08-01T10:08:10Z'
updated_at: '2025-10-21T12:18:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Verfügbar für: Jira Cloud einschließlich LDAP-geschützt Preispläne: Starter,
    Business, Enterprise, Education Einrichtung durch: (Enterprise) Unternehmens-Admin
    oder (Alle anderen Pläne) Team-Admin mit Jira-Admin-Berechtigungen'
---

:::warning
Sollten technische Probleme auftreten, lies bitte unseren Artikel über [Mögliche Probleme und wie du sie beheben kannst](https://help.miro.com/hc/articles/360017572654).
:::

:::tip
Erfahre mehr über Jira-Karten in den Artikeln [Häufige Fragen zu Jira-Karten](https://help.miro.com/hc/articles/360013463739)
:::

## Verbindung von Jira und Miro

### Installieren der App

1. Um die Integration zu aktivieren, klicke auf deinem [Dashboard](https://help.miro.com/hc/articles/360017571294-What-is-on-your-dashboard) oben rechts auf dein Avatar > **Apps & Integrationen**:![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)
   *Apps verwalten*
2. Finde "Jira-Karten" in der **Suchzeile** und klicke auf den blauen **Verbinden** Schaltfläche in der rechten unteren Ecke des Popup-Menüs.
3. Du siehst ein Fenster zum **Hinzufügen von „Jira-Karten“**. Hier musst du die Installation bestätigen oder das Team auswählen, in dem du die Integration installieren möchtest (falls du Mitglied in mehreren Teams bist). Klicke auf **Hinzufügen**, um die Integration hinzuzufügen. Am oberen Rand des Dashboards siehst du die Bestätigungsmeldung, dass die **App installiert wurde:**
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)
   *Die Bestätigungsmeldung*

### Dein Jira-Profil verbinden

1. Klicke erneut auf dein Avatar auf dem Dashboard und gehe zu **Einstellungen > Teams >** *Dein Teamname* **> Apps & Integrationen > Jira-Karten** und klicke auf **Verbinden:
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)***Die Integrationseinstellungen*
2. Du wirst zur Jira-Seite geleitet, um die Verbindung zu autorisieren. Melde dich bei Jira an und klicke auf **Akzeptieren**.

### Jira-Instanzen mit deinem Miro-Team verbinden

Mit OAuth 2.0 kannst du jetzt mehrere deiner Jira-Instanzen mit demselben Team und denselben Boards verbinden. Nachdem du die App in den Einstellungen autorisiert hast, siehst du die Option, **eine andere Instanz zu verbinden.**

1. Öffne die Jira-Kartenauswahl über die Erstellungssymbolleiste (du musst die App möglicherweise über die **Weitere Apps +** Schaltfläche hinzufügen).
2. Klicke in der Auswahl auf **Einstellungen**.
3. Du wirst zum Abschnitt **Apps & Integrationen** in deinen Einstellungen geleitet. Such nach der Option **Eine andere Instanz verbinden** und wähle alle zusätzlichen Jira-Instanzen aus, die du verbinden möchtest.![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)*Einstellungen für Jira-Karten in einem Miro-Konto*

Team-Admins können auch alle Instanzen sehen, die die Mitglieder des Teams verbunden haben:

![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)

:::warning
Beachte, dass sich jede Person von den Miro-Boards aus bei jeder verbundenen Jira-Instanz authentifizieren muss, wenn sie mit den Karten der Instanz arbeiten möchte.
:::

> ✍️ Beachte, dass immer nur eine Instanz aktiv sein kann, sodass Personen Karten davon abrufen können. An bestehenden Karten von inaktiven Instanzen kann weiterhin auf den Miro-Boards gearbeitet werden.

### Echtzeit-Updates von Jira einrichten

Um die vollen Vorteile unserer bidirektionalen Synchronisierung in Echtzeit zu nutzen, müssen Sie Webhooks für die hinzugefügten Jira-Instanzen konfigurieren. Dies stellt sicher, dass alle Updates, die Sie in Jira vornehmen, in Miro in Echtzeit übernommen werden.

1. Öffne die Jira-Kartenauswahl über die Erstellungssymbolleiste (du musst die App möglicherweise über den Button **Weitere Apps +** hinzufügen).
2. Klicke in der Auswahl auf **Einstellungen**.
3. Du wirst zum Abschnitt **Apps & Integrationen** in deinen Einstellungen geleitet.
4. Im Abschnitt **Verbundene Instanzen** solltest du eine Liste aller zuvor hinzugefügten Instanzen sehen.
5. Neben jeder Instanz gibt es eine Schaltfläche zum **Webhook hinzufügen**. Ein Klick darauf richtet Echtzeit-Updates von Jira zu Miro für diese Instanz ein.
6. Wenn du in Zukunft Webhooks von dieser Instanz entfernen möchtest, kannst du die obigen Schritte befolgen und die Schaltfläche **Webhook entfernen** neben der verbundenen Instanz klicken, für die du einen Webhook hinzugefügt hast.

:::note
Bitte beachten: Du musst sowohl ein Admin bei Miro *und* Jira sein, um Webhooks zu deinen Instanzen hinzufügen zu können.
:::

Danach bist du fertig! Jetzt kannst du Jira-Aufgaben als Karten auf dem Whiteboard hinzufügen. Alle Änderungen, die in Jira vorgenommen werden, spiegeln sich in den Jira-Karten auf dem Board wider und umgekehrt.

## Deinstallation des Plugins

Gehe zu deinen **Team-Einstellungen > Apps & Integrationen > Jira-Karten** und klicke **Deinstallieren für Team.**

:::tip
Vergiss nicht, dir den Hauptartikel über [die Verwendung von Jira-Karten](https://help.miro.com/hc/articles/360017572434) anzusehen!
:::
