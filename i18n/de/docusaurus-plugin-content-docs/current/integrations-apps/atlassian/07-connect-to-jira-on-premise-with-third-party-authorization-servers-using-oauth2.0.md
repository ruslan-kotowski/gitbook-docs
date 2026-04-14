---
title: Verbinde dich mit Jira lokal über Drittanbieter-Autorisierungsserver, die OAuth2.0
  verwenden.
article_id: 25692796700306
translation_id: 26751280409746
locale: de
sidebar_position: 9
created_at: '2025-05-16T09:13:18Z'
updated_at: '2025-11-25T15:50:34Z'
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

> *✏️* Das Verbinden von Jira über einen Autorisierungsserver ist nur auf Organisationsebene aktiviert.

Dieser Artikel beschreibt die Schritte zur Verbindung von Miro mit Jira über einen Drittanbieter-Server vor Ort mithilfe eines OAuth2.0-Autorisierungsservers.

Um die technischen Details zu dieser Konfiguration zu erfahren, siehe den Artikel über [Jira On-Premise mit Drittanbieter-Autorisierung über OAuth 2.0](https://help.miro.com/hc/articles/26726425696530).

## Voraussetzungen

- Vergewissere dich, dass du die folgenden Berechtigungen hast:
  - Miro Unternehmens-Admin
  - (Optional) Jira-Systemadministrator, wenn du automatische Webhooks verwenden möchtest.
- Erstelle in deinem Autorisierungsserver eine OAuth 2.0-App.
- Konfiguriere die Weiterleitungs-URL in deiner OAuth 2.0-App auf die folgende URL:
  https://integrations.miro.com/api/external-auth/oauth2/callback
- Stelle sicher, dass du die folgenden Details aus deiner OAuth 2.0-App bereit hast, um sie in Miro einzurichten:
  - Autorisierungs-URL
  - Token-URL
  - Client-ID
  - Geheimer Clientschlüssel
  - Geltungsbereich

## Mit Jira on-premise über Drittanbieter-Server unter Verwendung von OAuth 2.0 verbinden

1. Wähle in deinem Miro-Dashboard deinen Avatar in der oberen rechten Ecke aus und gehe zu **Admin-Konsole**| **Einstellungen**.
2. Gehe zu **Apps und Integrationen ![icon-plug.svg](../../../../../../docs/integrations-apps/atlassian/images/26513589065106_icon-plug.svg)**> **Apps** > **Apps verwalten**-Tab.
3. Stelle sicher, dass **nur Apps aus der Liste unten zulassen** aktiviert ist.
4. Unter der **App**-Spalte wähle für **Jira-Karten** die **Einstellungen** aus.
5. Klicke auf **neue Verbindung hinzufügen**.
6. Unter **Jira-Einrichtung** klick auf **Jira-Rechenzentrum**.
7. Unter **Authentifizierungsmethode** wähle **OAuth2.0 über einen Drittanbieter-Autorisierungsserver** aus.
8. Unter **Jira-URL** gib deine Jira-Instanz-URL ein.
   > *✏️* Du kannst deine externe Jira-Basis-URL oder deine interne Jira-URL hinzufügen. Wenn du eine interne Jira-URL verwendest, musst du im Schritt 10 deine externe API-Gateway-URL angeben.

   > *✏️* Im Allgemeinen ermöglicht die Verwendung einer internen URL, die Navigation zur Quelle anzupassen.
9. Um diese Verbindung zur Standardverbindung für alle Teams in deiner Organisation zu machen, aktiviere **Als Standard festlegen**.
10. (Optional) Wenn du ein API-Gateway verwendest, um Anfragen an Jira zu stellen, gib für **Jira API Gateway Basis-URL** deine externe API-Gateway-URL ein.
11. Gib die folgenden Details aus deiner OAuth 2.0-App ein:
    - Autorisierungs-URL
    - Token-URL
    - Client-ID
    - Geheimer Clientschlüssel
    - Umfang
12. (Optional) Um Echtzeit-Updates von Jira in Miro zu erhalten, aktiviere **Webhook automatisch erstellen**.
    > *✏️ Du kannst den Webhook später manuell hinzufügen.*
13. Klicke auf **Verbinden**.
14. Befolge den Authentifizierungsablauf für deinen Autorisierungsserver. Wenn du dazu aufgefordert wirst, melde dich in deiner Umgebung an.
    Wenn die Verbindung abgeschlossen ist, wird deine Jira-Instanz unter **Verbundenen Instanzen** mit dem folgenden Tag aufgeführt: **Authentifizierungsserver**.

## Stelle sicher, dass dein Team sich authentifizieren kann

Jetzt, da du deine Jira-Instanz auf Organisationsebene verbunden hast, kannst du Jira auf Teamebene nutzen.

1. Wähle in deinem Miro-Dashboard rechts oben deinen Avatar aus und gehe zur **Admin-Konsole**.
2. Wähle **Teams** > **Dein Team** aus.
   Der **Slider für dein Team** öffnet sich.
3. Wähle den **Apps**-Tab aus.
4. Wähle aus der App-Liste **Jira-Karten** aus.
5. Unter **Admin-Einstellungen** überprüfe, ob deine Jira-Konfiguration das Label **GLOBAL CONNECTION** anzeigt und die korrekte Jira-Instanz-URL anzeigt. Führe dann eine der folgenden Aktionen aus:
   - Wenn ja, hast du diese Prozedur abgeschlossen. Du kannst zu [Was nun?](https://help.miro.com/hc/articles/25699264170386) springen.
   - Wenn nein, wähle **Konfiguration ändern** > **Globale Unternehmenseinstellungen** > **deine Jira-Instanz**.
6. Wähle **Einstellungen speichern**.

## Was kommt als Nächstes?

Jedes Teammitglied muss sein Benutzerkonto autorisieren. Um sicherzustellen, dass jeder Nutzer Zugriff und Aktualisierungs-Tokens erhält, werden die Teammitglieder bei einem Jira-bezogenen Vorgang auf einem Miro-Board aufgefordert, ihr Konto zu autorisieren.

## Häufige Fragen

**Welche Autorisierungsserver kann ich verwenden?**

Du kannst jeden Autorisierungsserver verwenden, der Standard-OAuth 2.0-Protokolle für lokale Umgebungen unterstützt. Zum Beispiel Azure Active Directory (Entra ID) und Okta.

**Kann ich denselben Autorisierungsserver für mehrere Organisationen verwenden?**

Ja, aber du musst den Server manuell zu jeder Organisation hinzufügen.

**Kann ich das Client-Geheimnis für einen Autorisierungsserver aktualisieren?**

Nein. Wenn du den Client Secret ändern musst, musst du deine Instanz trennen und wieder verbinden.

**Können Organisations- und Team-Admins in Jira weiterhin die native Autorisierung verwenden?**

Ja. Je nach ausgewählter Konfiguration können Admins den nativen Autorisierungsablauf in Jira weiterhin nutzen.

**Was passiert, wenn ein Team bereits mit einer anderen Jira-Instanz verbunden ist?**

Du kannst Teams auf die Standard-Jira-Einstellungen deiner Organisation aktualisieren [Standard-Jira-Einstellungen](https://help.miro.com/hc/articles/26438407676434).

**Steuert Miro die Zuordnung zwischen autorisierten und Jira-Nutzern?**

Nein. Die Zuordnung zwischen autorisierten Nutzern und Jira-Nutzern fällt in die Verantwortung der Kundenumgebung über deren API-Gateway. Miro kontrolliert dieses Gateway nicht.

**Wie erkenne ich, ob OAuth 2.0 über einen Drittanbieter-Autorisierungsserver die richtige Lösung für meine Organisation ist?**

Wenn alle der folgenden Punkte zutreffen, ist OAuth 2.0 über einen Autorisierungsserver eines Drittanbieters eine gute Lösung:

- Deine Jira-Instanz wird lokal gehostet.
- Externer Zugriff auf Jira ist nur mit einem API-Gateway möglich.
- Das API-Gateway erzwingt die Autorisierung mittels eines benutzerdefinierten Autorisierungsservers.
- Du musst Miro mit Jira verbinden, ohne die öffentliche Basis-URL von Jira offenzulegen.

**Welches Problem löst diese Lösung?**

Diese Lösung ist für Organisationen konzipiert, die Jira lokal hosten und externen API-Datenverkehr über ein API-Gateway leiten. In dieser Konfiguration ist Jira nicht öffentlich zugänglich, und der Zugriff wird über einen benutzerdefinierten Autorisierungsserver gesteuert. Anstatt eine öffentliche Basis-URL für Jira zu haben, ermöglicht diese Lösung, deine lokalen Jira-Instanzen zu verbinden, indem du Miro so konfigurierst, dass die Authentifizierung über deinen eigenen Autorisierungsserver erfolgt.
