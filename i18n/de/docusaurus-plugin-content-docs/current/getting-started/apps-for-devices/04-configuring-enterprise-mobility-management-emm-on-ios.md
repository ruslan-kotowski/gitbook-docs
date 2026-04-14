---
title: Enterprise Mobility Management (EMM) in iOS konfigurieren
article_id: 10183062016274
translation_id: 10183062016274
locale: de
sidebar_position: 4
created_at: '2023-02-20T18:20:46Z'
updated_at: '2025-11-25T15:36:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
availability:
  notes: 'allgemeine: Schritte zur Konfiguration der EMM/MDM-Lösung deines Unternehmens
    anhand von drei Beispielen aus einer bestimmten Software beschrieben: VMWare Workspace
    ONE, Ivanti Neurons (früher MobileIron Cloud) und Intune (Microsoft Endpoint Manager).
    Wenn du eine andere Lösung verwendest, empfehlen wir dir, die Dokumentation deines
    EMM-Anbieters zu konsultieren.'
---

Über das EMM können Unternehmens-Admins Miro zentralisiert und einheitlich konfigurieren und an Nutzer in ihrem Unternehmen verteilen. Miro unterstützt die Bereitstellung der folgenden Einstellungen für die Endgeräte:

- Deaktivierung des Registrierungsvorgangs.
- Beschränkung der unterstützten Authentifizierungsanbieter (z. B. soziale Netzwerke, E-Mail-Anbieter usw.).
- Beschränkung des Nutzernamens auf einen bestimmten Wert oder eine Liste zulässiger E-Mail-Domains.
- Erweiterte SSO-Konfiguration.

## So klappt die Konfiguration

### Füge Miro zum App-Verzeichnis deiner Organisation hinzu

In den meisten Fällen ist es erforderlich, Miro zum App-Katalog deines Unternehmens hinzuzufügen, um mit der EMM-Konfiguration zu starten. Dieser Prozess kann je nach EMM-Anbieter variieren. In der Regel fügst du Miro jedoch direkt vom Apple Store zu deinem App-Katalog hinzu und legst eine Verteilungsrichtlinie fest, die auf Gerätegruppen, Nutzergruppen usw. basiert.

#### Beispiele

**VMware Workspace ONE**

Einen allgemeinen Leitfaden zur Bereitstellung von VMware Workspace ONE findest du [hier](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Klicke auf **Hinzufügen** und dann auf **Öffentliche App.**
2. Wähle in dem Dropdown-Menü der Plattform **Android** aus und **App Store durchsuchen** für die Quelle.
3. Gib „**Miro**“ in das **Textfeld „Name“** ein und klicke anschließend auf „Weiter“.
4. Wähle die Miro-App aus und tippe auf **Genehmigen**, wenn du dazu aufgefordert wirst.
5. Veröffentliche die App, indem du auf **Speichern und zuweisen** klickst.
6. Konfiguriere die Zuweisungen und Verteilungseinstellungen entsprechend den Präferenzen deines Unternehmens.

Ivanti Neurons

1. Gehe zu **Apps > App-Katalog** und klicke auf **Hinzufügen.**
2. Wähle den „**App Store**“ (iOS) und dein Land als Ursprung aus.
3. Suche nach "**Miro**" und wähle "**Miro: Online-Whiteboard**" aus der Liste der verfügbaren Apps.
4. Konfiguriere die Verteilungseinstellungen und -richtlinien gemäß den Präferenzen deines Unternehmens.

Intune (Microsoft Endpoint Manager)

[Einen allgemeinen Leitfaden zur Bereitstellung von Intune von MS findest du](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-ios-ipados)hier.

1. Gehe zu **Apps > iOS/iPadOS** und klicke auf **Hinzufügen**.
2. Wähle **App speichern > iOS-App speichern** als **App-Typ** aus.
3. Klicke auf **Im App Store suchen**.
4. Wähle das Land des Stores aus, den du verwenden möchtest.
5. Suche "**Miro**" und wähle "**Miro: Online-Whiteboard**" aus der Liste der verfügbaren Apps.
6. Konfiguriere die Verteilungseinstellungen und -richtlinien gemäß den Präferenzen deines Unternehmens.

### App-Einstellungen vorausfüllen

Miro nutzt „AppConfig“ als einheitliche Methode zur Konfiguration und Sicherung der Kundendaten. Viele EMM-Lösungen unterstützen das AppConfig-Format oder sie akzeptieren es im „Kompatibilitätsmodus“. Die genauen Einschränkungen, die in deinem Fall gelten, findest du in der Dokumentation deines EMM-Anbieters.

#### Beispiele

**VMWare Workspace ONE**

Einen allgemeinen Leitfaden zur Bereitstellung von VMware Workspace ONE findest du [hier](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Gehe zu **Ressourcen > Apps**.
2. Klicke auf **zuweisen** im Fenster **Status installieren** in der Spalte **Miro: Online-Whiteboard** app row.
3. Lege den **Namen, die Zuweisungsgruppen** und die **App-Auslieferungsmethode** der Verteilung fest.
4. Aktiviere **Verwalteter Zugriff** und **Konfiguration senden**.
5. Die App-Konfiguration definieren

Ivanti Neurons

1. 1. Gehe zu **Apps > App-Katalog**.
   2. Navigiere zu "**Miro: Online-Whiteboard**" Einstellungen.
   3. Gehe zu **App-Konfigurationen > Apple Managed App-Konfiguration**.
   4. Klicke auf **Hinzufügen**, um ein neues Verteilungsprofil zu erstellen.
   5. Gib deinem Konfigurationsprofil einen Namen.
   6. Definiere **Apple Managed App-Einstellungen**
   7. Wähle das Verteilungsprofil im Abschnitt **Diese App-Konfiguration verteilen** aus.

Intune (Microsoft Endpoint Manager)

[Einen allgemeinen Leitfaden zur Bereitstellung von Intune von MS findest du](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-ios-ipados)hier.

1. 1. Gehe zu **Apps > App-Konfigurationsrichtlinien**.
   2. Klicke auf **Hinzufügen > Gerät verwalten**, um eine neue App-Konfiguration zu erstellen.
   3. Gib deinem Konfigurationsprofil einen Namen.
   4. Wähle **iOS/iPadOS** als **Plattform** aus.
   5. Wähle **Miro: Online-Whiteboard** als **Ziel-App**, indem du auf **App auswählen** klickst.
   6. Wähle **Konfigurationsdesigner** als **Konfigurationseinstellungen** verwenden aus.
   7. App-Konfiguration definieren
   8. Wähle das Verteilungsprofil für die Konfiguration aus.

## Komplette Liste der unterstützten Einstellungen

### Beschränkung der Optionen „Anmelden mit …“ / „Anmelden“

Wenn die Option „Registrieren“ aktiviert ist, wirken sich alle Einstellungen für „Anmelden mit …“ auf den Anmeldevorgang aus.

:::warning
Jeder Schlüssel, der nicht explizit auf „wahr“ gesetzt ist (oder nicht vorhanden ist), gilt als auf „falsch“ gesetzt. Daher ist die Authentifizierungsoption verfügbar (Standardverhalten).
:::

| Schlüssel | Typ | Erlaubte Werte |
| --- | --- | --- |
| **Facebook** miro.authentication.facebookRestricted | Boolean | wahr/falsch |
| **Google** miro.authentication.googleRestricted | wahr/falsch |
| **Microsoft Office 365** miro.authentication.office365Restricted | wahr/falsch |
| **Slack**   miro.authentication.slackRestricted | wahr/falsch |
| **AppleID** miro.authentication.appleIdRestricted | wahr/falsch *Nur auf Apple-Geräten verfügbar |
| Registrieren miro.authentication.signUpRestricted | wahr/falsch |
| **Anmeldung mit Magic Link** miro.authentication.magicLinkRestricted | wahr/falsch |
| Unternehmensarbeitsbereich miro.authentication.enterpriseWorksSpaceDisabled | wahr/falsch |

### Einschränkungen beim Nutzernamen

Kundinnen und Kunden, die die Sicherheit verbessern und gleichzeitig eine einfache Passwortauthentifizierung beibehalten möchten, können folgende Optionen nutzen.

| Schlüssel | Wert | Beschreibung |
| --- | --- | --- |
| **Vordefinierter Nutzername** miro.policy.authentication.username | **Wert-Typ:** String | Das Feld ist gesperrt und kann von Personen nicht geändert werden |
| **Domains auf der Whitelist** miro.policy.authentication.allowedDomains | **Wert-Typ:** Array  **Wert:** @miro.com, @yourdomain.com  *Einige Anbieter unterstützen keine **Array**-Datentypen.  Sollte das der Fall sein, verwende bitte den Typ **string** und JSON array als Wert. ["@miro.com", "@Ihredomain.com"] | Es sind nur E-Mail-Adressen erlaubt, die einer der aufgeführten Domains entsprechen. |

### SSO-Konfiguration

Um die Sicherheit des Unternehmens zu verbessern und den Authentifizierungsprozess zu vereinfachen, können Unternehmens-Admins die SSO-Richtlinie anhand des folgenden Beispiels konfigurieren.

:::warning
Vergewissere dich, dass die SSO-Richtlinie in der App-Konfiguration mit den SSO-Einstellungen der Miro-Organisation übereinstimmt. Wenn diese Richtlinien nicht miteinander übereinstimmen, können sich die Personen möglicherweise nicht anmelden und werden gesperrt. Miro kann die Einstellungen nicht validieren, bevor sie auf den Zielgeräten erzwungen werden.
:::

|  |  |
| --- | --- |
| Konfigurationsschlüssel | miro.policy.sso |
| Art des Konfigurationswerts | String |
| Richtlinienobjekt | \{ "authenticationRestricted" : false, "email": "user@domain.com", "allowDomains": ["domain1.com", "domain2.com"], "forceSsoLogin": true \} |

| Attribute der Richtlinienobjekte | | | |
| --- | --- | --- | --- |
| Parameter | Typ | Beschreibung | Merkzettel |
| authenticationRestricted | Boolean | Ob die Schaltfläche „Mit SSO anmelden“ auf der Hauptseite aktiviert ist. | **Der Schlüssel wird ignoriert, wenn andere Konfigurationsoptionen bereitgestellt werden.** |
| E-Mail-Adresse | String | E-Mail-Adresse, die für das SSO-Login vordefiniert ist. | Das Feld ist gesperrt und kann nicht geändert werden |
| allowDomains | Boolean | Behalte SSO als einzige verfügbare Methode für die Authentifizierung. | Die Person wird umgehend zur Seite „Mit SSO anmelden“ weitergeleitet. Alle anderen Optionen außer **email** und **allowedDomains** werden ignoriert. Es stehen keine anderen Authentifizierungsmethoden zur Verfügung. |
