---
title: Jira lokal mit Drittanbieter-Autorisierung über OAuth 2.0 Referenz
article_id: 26726425696530
translation_id: 26751134924818
locale: de
sidebar_position: 11
created_at: '2025-05-16T09:08:59Z'
updated_at: '2025-11-25T15:51:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Verfügbar für: Unternehmens-Admins Preispläne: Unternehmen'
---

Dieser Artikel bietet technische Details zur Verwendung eines Drittanbieter-Autorisierungsservers mit OAuth 2.0, um Jira mit Miro zu integrieren.

Um zu erfahren, wie du eine Verbindung einrichtest, sieh dir [Verbindung zu Jira on-premise mit Drittanbieterauthorisierungsservern über OAuth 2.0 herstellen](https://help.miro.com/hc/articles/25692796700306) an.

## Funktionsweise der Jira-Integration mit Miro unter Verwendung von On-Premise-Autorisierung und OAuth 2.0

Die folgende Grafik zeigt den Kommunikationsfluss zwischen Miro und einem lokalen Jira-Autorisierungsserver.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Miro und Jira-Integration mit einem lokalen Autorisierungsserver über ein API-Gateway*

## Konfigurationsparameter

Um den Autorisierungsablauf zwischen Miro und Jira mithilfe eines Drittanbieter-Autorisierungsservers mit OAuth 2.0 zu konfigurieren, musst du die folgenden Parameter angeben:

- **Autorisierungsserver**
  - Autorisierungsanforderungs-URL
  - Token-Anforderungs-URL
  - Umfang
- **Autorisierungs-App-Konfiguration**
  - Client-ID
  - Geheimer Clientschlüssel
- **Jira-Instanz**
  - Jira-öffentliche URL
  - Jira-Basis-URL; interne URL

:::note
Miro stellt die Umleitungs-URL bereit, die der Autorisierungsserver gegen die registrierte App validiert.
:::

**Weitere Informationen:** Siehe [Verbindung zu Jira on-premise mit Drittanbieter-Autorisierungsservern unter Verwendung von OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Autorisierungsanfragen zwischen Miro und einem lokalen Autorisierungsserver

Für eine Integration zwischen Miro und Jira unter Verwendung eines Autorisierungsservers eines Drittanbieters zeigt das folgende Diagramm den Ablauf der Benutzerautorisierungsanfrage.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Anfrage zur Benutzerautorisierung*

### Autorisierungsanfrage

```
https://{authorization_URL}?
    response_type=code&
    client_id={CLIENT_ID}&
    redirect_uri={Miro Redirect-URI}&
    scope={scope}&
    Status={state}
```

Der Nutzer kann der Autorisierungsanfrage Parameter als Schlüssel-Wert-Paare in der Konfiguration hinzufügen.

### Token-Anfrage

```
curl --request POST \\
    --url '{token request URL}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=authorization_code \
    --data 'client_id={CLIENT_ID}' \
    --data 'client_secret={CLIENT_SECRET}' \
    --data 'code={Erhaltener Autorisierungs-Code}' \
    --data 'redirect_uri={Miro Umleitungs-URI}' \
```

Nachdem Miro den Autorisierungscode erhalten hat, stellt Miro den Status bereit und fordert ein Token-Paar an.

### Aktualisieren der Token-Austausch

```
curl --request POST \
    --url '{Tokenanforderungs-URL}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=refresh_token \
    --data 'client_id={CLIENT_ID}' \
    --data 'refresh_token={aktuelles gültiges Refresh-Token}' \
```

Stelle sicher, dass die Aktualisierung des Tokens aktiviert ist; erlaube den Offline-Zugriff auf APIs.

### Jira-API-Anfragen

```
curl --request GET \\
    --url {Jira Public URL}/rest/api/{apiversion}/... \
    --header 'Autorisierung: Bearer {accessToken}' \
    --header 'content-type: application/json'
```

Jede Anfrage verwendet die angegebene öffentliche Jira-URL als Basis-URL und das Benutzerzugriffstoken als Überbringer-Token.
