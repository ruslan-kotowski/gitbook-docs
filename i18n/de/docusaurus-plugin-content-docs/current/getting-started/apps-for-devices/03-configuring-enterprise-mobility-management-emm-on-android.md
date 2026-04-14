---
title: Enterprise Mobility Management (EMM) für Android konfigurieren
article_id: 13888848676498
translation_id: 13888848676498
locale: de
sidebar_position: 3
created_at: '2023-09-21T14:45:02Z'
updated_at: '2025-11-25T15:38:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
availability:
  notes: 'allgemeine: Schritte zur Konfiguration der EMM/MDM-Lösung deines Unternehmens
    anhand von drei Beispielen aus einer bestimmten Software beschrieben: VMWare (Workspace
    ONE), Ivanti Neurons (ehemals MobileIron Cloud) und Intune (Microsoft Endpoint
    Manager). Wenn du eine andere Lösung verwendest, empfehlen wir dir, die Dokumentation
    deines EMM-Anbieters zu konsultieren.'
---

Über das EMM können Unternehmens-Admins Miro zentralisiert und einheitlich konfigurieren und an Nutzer in ihrem Unternehmen verteilen. Miro unterstützt die Bereitstellung der folgenden Einstellungen für die Endgeräte:

- Deaktivierung des Registrierungsvorgangs.
- Beschränkung der unterstützten Authentifizierungsanbieter (z. B. soziale Netzwerke, E-Mail-Anbieter usw.).
- Beschränkung des Nutzernamens auf einen bestimmten Wert oder eine Liste zulässiger E-Mail-Domains.
- Erweiterte SSO-Konfiguration.

## So klappt die Konfiguration

### Füge Miro zum App-Verzeichnis deiner Organisation hinzu

In den meisten Fällen ist es erforderlich, Miro zunächst zum App-Katalog deines Unternehmens hinzuzufügen, bevor die EMM-Konfiguration gestartet werden kann.  Dieser Prozess kann je nach EMM-Anbieter variieren. In der Regel fügst du Miro jedoch direkt vom Google Play Store zu deinem App-Katalog hinzu und legst eine Verteilungsrichtlinie fest, die auf Gerätegruppen, Nutzergruppen usw. basiert.

#### Beispiele

**VMware Workspace ONE**

Einen allgemeinen Leitfaden zur Bereitstellung von VMware Workspace ONE findest du [hier](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Klicke auf **Hinzufügen** und dann auf **Öffentliche App.**
2. Wähle in dem Dropdown-Menü der Plattform **Android** aus und **App Store durchsuchen** für die Quelle.
3. Gib „**Miro**“ in das **Textfeld „Name“** ein und klicke anschließend auf „Weiter“.
4. Wähle die Miro-App aus und tippe auf **Genehmigen**, wenn du dazu aufgefordert wirst.
5. Veröffentliche die App, indem du auf **Speichern und zuweisen** klickst.
6. Konfiguriere die Zuweisungen und Verteilungseinstellungen entsprechend den Präferenzen deines Unternehmens.

**Ivanti Neurons**

Einen allgemeinen Leitfaden zur Bereitstellung von Ivanti Neurons findest du [hier](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/92/all/Managing_Google_Play_apps.htm).

- 1. Gehe zu **Apps > App-Katalog** und klicke auf **Hinzufügen.**
  2. Wähle als Quelle den „**Google Play Store**“ und dein Land aus.
  3. Suche nach "**Miro**" und wähle "**Miro: Online-Whiteboard**" aus der Liste der verfügbaren Apps.
  4. Konfiguriere die Verteilungseinstellungen und -richtlinien gemäß den Präferenzen deines Unternehmens.

**Intune (Microsoft Endpoint Manager)**

Einen allgemeinen Leitfaden zur Bereitstellung von Intune von MS findest du[hier](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-android).

1. Gehe zu **Apps > Alle Apps** und klicke auf **Hinzufügen**.
2. Wähle **App speichern > Android-App** (als **App-Typ**).
3. Trage auf der Seite „**App-Informationen**“ die Angaben ein, die du in dem [Miro-Eintrag des Google Play Stores](https://play.google.com/store/apps/details?id=com.realtimeboard) findest.
4. Konfiguriere die Verteilungseinstellungen und -richtlinien gemäß den Präferenzen deines Unternehmens.

Konfiguriere die Verteilungseinstellungen und -richtlinien gemäß den Präferenzen deines Unternehmens.

### App-Einstellungen vorausfüllen

Miro verwendet als einheitliche Methode zur Konfiguration und Sicherung von Kundendaten [AppConfig](https://www.appconfig.org/), da es eine einfache Konfiguration mobiler Unternehmens-Apps ermöglicht. Viele EMM-Lösungen unterstützen das AppConfig-Format oder sie akzeptieren es im „Kompatibilitätsmodus“. Die genauen Einschränkungen, die in deinem Fall gelten, findest du in der Dokumentation deines EMM-Anbieters.

#### Beispiele

**VMWare Workspace ONE**

Einen allgemeinen Leitfaden zur Bereitstellung von VMware Workspace ONE findest du [hier](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications).

1. Gehe zu **Ressourcen > Apps**.
2. Klicke auf **zuweisen** im Fenster **Status installieren** in der Spalte **Miro: Online-Whiteboard** app row.
3. Lege den **Namen, die Zuweisungsgruppen** und die **App-Auslieferungsmethode** der Verteilung fest.
4. Aktiviere **Verwalteter Zugriff** und **Konfiguration senden**.
5. Die App-Konfiguration definieren

**Ivanti Neurons**

Einen allgemeinen Leitfaden zur Bereitstellung von Ivanti Neurons findest du [hier](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/92/all/Using_the_Android_enterprise_App_Configuration.htm).

1. Gehe zu **Apps > App-Katalog**.
2. Navigiere zu "**Miro: Online-Whiteboard**" Einstellungen.
3. Gehe zu **App-Konfigurationen > Verwaltete Konfigurationen für Android**.
4. Klicke auf **Hinzufügen**, um **App-Einschränkungen** zu erstellen.
5. Definiere die **Erforderlichen Berechtigungen** und die **Laufzeitberechtigungen**.
6. Wähle im **Abschnitt** Diese App-Konfiguration verteilen das Verteilungsprofil aus.

**Intune (Microsoft Endpoint Manager)**

Einen allgemeinen Leitfaden zur Bereitstellung von Intune von MS findest du[hier](https://learn.microsoft.com/mem/intune/apps/app-configuration-policies-use-android).

1. Um eine neue App-Konfiguration zu erstellen, gehe zu **Apps > App-Konfigurationsrichtlinien > Hinzufügen > Verwaltete Geräte**.
2. Gib deinem Konfigurationsprofil einen Namen.
3. Wähle als **Plattform** **Android Enterprise** aus.
4. Wähle **Miro: Online-Whiteboard** als die **Ziel-App** durch Klicken auf **App auswählen**.
5. Wähle **Konfigurationsdesigner** als **Konfigurationseinstellungen verwenden** aus.
6. App-Konfiguration definieren
7. Wähle das Verteilungsprofil für die Konfiguration aus.

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
