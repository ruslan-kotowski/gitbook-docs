---
title: Verbindung zu Jira mit OAuth 1.0 (Aktualisiert)
article_id: 27689156602514
translation_id: 27689181505554
locale: de
sidebar_position: 12
created_at: '2025-06-27T13:20:10Z'
updated_at: '2025-11-25T15:52:25Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Wer kann es tun: Unternehmens-Admins, Team-Admins Welche Preispläne: Starter,
    Business, Enterprise, Education Welche Plattformen: Browser, Desktop'
---

Organisationen, die noch nicht bereit sind, auf OAuth 2.0 zu migrieren, können das folgende Verfahren verwenden, um Miro mit Jira über OAuth 1.0 zu verbinden.

Atlassian hat [OAuth 1.0 als veraltet erklärt](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively), und die in diesem Artikel bereitgestellte Methode ist eine Übergangslösung. Um Probleme zu vermeiden und um den besten Praktiken für Sicherheit und Kompatibilität zu entsprechen, empfiehlt Miro dringend, so bald wie möglich auf OAuth 2.0 zu migrieren.

:::note
Die vorherige OAuth 1.0-Authentifizierungsmethode [ist veraltet](https://help.miro.com/hc/articles/360019501754-Set-up-and-disable-Jira-Cards-OAuth-1-0) und wird am 31. Juli 2025 entfernt.
:::

Dieser Artikel erklärt auch die Verwendung einer Jira-Instanz für mehrere Miro-Teams und wie Jira-Karten auf Organisations- und Teamebene deaktiviert werden.

## Voraussetzungen

- Vergewissere dich, dass du die folgenden Berechtigungen hast:
  - (Business, Enterprise) Miro Unternehmens-Admin
    (Starter, Education) Miro Team-Admin
  - Jira-System-Admin

    > ✏️ Um das Verfahren abzuschließen, musst du in der Lage sein, einen Anwendungslink in Jira zu erstellen.
- Entferne in Jira alle bestehenden Anwendungslinks zu Miro.

## Vorgehensweise

Um eine Verbindung zu Jira über OAuth 1.0 herzustellen, gehe wie folgt vor:

1. Klicke in deinem Miro-Dashboard auf deinen Avatar oben rechts und wähle **Admin-Konsole** aus.
2. Gehe in der linken Seitenleiste zu **Apps und Integrationen** > **Apps** > **Apps verwalten**-Tab.
3. Vergewissere dich, dass **Nur Apps aus der Liste unten zulassen** aktiviert ist.
4. Wähle in der **App**-Spalte für **Jira-Karten** **Einstellungen** aus.
5. Wähle im **Standard-Einstellungen**-Tab **Neue Verbindung hinzufügen** aus.
6. Wähle unter **Jira-Setup** entweder **Jira Cloud** oder **Jira Data Center** aus.
7. Unter **Authentifizierungsmethode** wähle **OAuth 1.0x (Aktualisiert)**.
8. Unter **Jira-URL** gib die URL deiner Jira-Instanz ein.
9. (Optional) Um diese Verbindung zur Standardverbindung für alle Teams in deiner Organisation zu machen, wähle **Als Standard festlegen** aus.
10. Unter **Setup-Anweisungen** stelle sicher, dass du über die folgenden Eigenschaften verfügst:
    - URL
    - Verbraucherschlüssel
    - Verbrauchername
    - Öffentlicher Schlüssel
11. Erstelle in Jira einen Anwendungslink.
    1. (Cloud) Gehe zu **Einstellungen** > **Produkte** > **Anwendungslinks**.
       (Data Center) Gehe in den Jira-Admin-Einstellungen zu **Produkte** > **Anwendungslinks**.
    2. Klicke auf **Link erstellen**.
    3. (Cloud) Wähle bei **Anwendungstyp** **Direkte Anwendung**.
       (Data Center) Wähle bei **Anwendungstyp** **Atlassian-Produkt**.
    4. Bei **Anwendungs-URL**, füge die URL aus den Miro-Einrichtungsanweisungen ein. Siehe Schritt 10.
    5. Klicke auf **Weiter**.
    6. Für **Anwendungsname** benenne deine App.

       > **⚠️** Gib keine Daten in andere Felder ein. Du wirst die Miro-Daten in einem späteren Schritt eingeben.
    7. Setze einen Haken bei **Link zum Empfang erstellen**.
    8. Klicke auf **Weiter**.
    9. Kopiere und füge deinen Consumer Key, Consumer Name und Public Key aus den Miro-Setup-Anweisungen ein. Siehe Schritt 10.
    10. Klicke auf **Weiter**.
        Du hast deinen Anwendung-Link erstellt.
12. In Miro klicke auf **Verbinden**.
    Du hast Miro mit Jira über OAuth 1.0 verbunden.

## Was kommt als Nächstes?

Sie haben Ihre Jira-Integration mit Miro mittels Jira OAuth1.0 konfiguriert und verbunden. Wenn ein Nutzer das erste Mal eine Jira-bezogene Aktion in Miro ausführt, wird er dazu aufgefordert, sich zu authentifizieren.

**Weitere Informationen:** Siehe [Wie man Jira-Karten verwendet](https://help.miro.com/hc/articles/360017572434).

## Eine Jira-Instanz für mehrere Miro-Teams

Sie können Jira-Karten auf Organisationsebene oder Teamebene installieren. Wenn Sie mehrere Teams haben, können Sie Organisationseinstellungen festlegen, um eine wiederholte Einrichtung für jedes Team zu vermeiden. Der bestehende Anwendungslink wird dann für alle Teams genutzt.

:::note
Die Verbindung mehrerer Jira-Instanzen mit einem Miro-Team wird nicht unterstützt.
:::

Für Aktualisierungsanforderungen wird nach der Verbindung Ihrer Organisation oder Ihres Teams mit einer Jira-Instanz ein Webhook zu den Jira-Webhooks für diese Miro-Organisation oder dieses Team hinzugefügt.

:::tip
Geben Sie jedem Webhook pro Team einen eindeutigen Namen. Gehen Sie zur Jira-WebHooks-Seite und bearbeiten Sie jeden neu erstellten Webhook.
:::

Wenn Sie organisationale Einstellungen angeben, behalten Teams, die bereits über eigene Teameinstellungen verfügen, ihre Konfiguration. Jedes Team mit eigener Konfiguration kann jederzeit zu den organisationale Einstellungen wechseln.

Umgekehrt kann jedes Team die organisationale Einstellungen überschreiben, um sich mit einer separaten Jira-Instanz zu verbinden.

## Jira-Karten deaktivieren

### Organisationsebene

Um Jira-Karten auf Organisationsebene zu deaktivieren, gehe wie folgt vor:

1. Klicke in deinem Miro-Dashboard auf deinen Avatar oben rechts und wähle **Admin-Konsole**.
2. Gehe zu **Apps und Integration** > **Apps verwalten**.
3. Suche **Jira-Karten**.
4. Schalte bei Jira-Karten die Option **Erlaubt** auf die Aus-Position.

:::warning
Wenn du die Jira-Karten für die Organisation deaktivierst, können Mitglieder in allen Enterprise-Teams keine Jira-Karten verwenden. Erfahre mehr über die App-Verwaltung unter [App-Verwaltung](https://help.miro.com/hc/articles/4404659741458).
:::

### Teamebene

Um Jira-Karten auf Teamebene zu deaktivieren, gehe wie folgt vor:

1. Klicke in deinem Miro-Dashboard auf deinen Avatar oben rechts und wähle **Admin-Konsole** aus.
2. Gehe zu **Teams**.
3. Klicke auf die Zeile für das Team, das du verwalten möchtest.
   Das Team-Einstellungsfeld wird geöffnet.
4. Klicke auf den **Apps**-Tab.
5. Finde und klicke auf **Jira-Karten**.
6. Klicke auf **Für Team entfernen**.
