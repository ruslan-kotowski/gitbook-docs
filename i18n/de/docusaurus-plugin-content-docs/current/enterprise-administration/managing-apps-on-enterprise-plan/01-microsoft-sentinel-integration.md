---
title: Microsoft Sentinel Integration
article_id: 31325908249362
translation_id: 31325908249362
locale: de
sidebar_position: 1
created_at: '2025-11-24T18:16:15Z'
updated_at: '2025-12-16T15:49:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: audit-logs
---

## Übersicht

Der [Miro](https://miro.com/)-Konnektor importiert Audit-Protokolle und Inhaltsaktivitätsprotokolle aus den [REST-APIs von Miro](https://developers.miro.com/reference/overview) in Microsoft Sentinel über das Codeless Connector Framework (CCF). Dies zentralisiert die Überwachung von Miro-Arbeitsbereichsaktivitäten in Microsoft Sentinel zur Erkennung von Sicherheitsbedrohungen, Untersuchung von Vorfällen und Compliance-Berichterstattung.

## Datenkonnektoren

Diese Lösung umfasst zwei Datenkonnektoren.

| Konnektor | Preisplan-Anforderungen | Erfasste Inhalte | Quellenangaben |
| --- | --- | --- | --- |
| **Miro Audit-Protokolle (Enterprise-Preisplan)** | Enterprise-Preisplan | Unternehmensweite Audit-Ereignisse, darunter Nutzer-Authentifizierung, Inhaltszugriffe, Teamänderungen und administrative Handlungen. | [API-Dokumentation](https://developers.miro.com/reference/enterprise-get-audit-logs) | [Übersicht der Audit-Protokolle](https://developers.miro.com/reference/audit-logs) |
| **Miro Content Logs (Enterprise-Plan + Enterprise Guard)** | Enterprise-Plan + Enterprise Guard Add-on | Verfolgung von Inhaltsaktivitäten einschließlich Erstellung, Aktualisierung und Löschung von Elementen für Compliance und eDiscovery. | [API-Dokumentation](https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch) | [Inhaltsprotokolle Übersicht](https://developers.miro.com/reference/board-content-logs) |

## Voraussetzungen

### Allgemeine Anforderungen

- Aktiver Microsoft Sentinel-Arbeitsbereich.
- Unternehmens-Admin-Rolle in deiner Miro-Organisation.
- Miro OAuth Zugriffstoken (nicht ablaufend).

### Spezifische Anforderungen für den Connector

#### Für Audit-Logs-Connector

- Miro Enterprise-Preisplan.
- OAuth Geltungsbereich: `auditlogs:read`.
- Zugriffstoken.

#### Für Inhalt-Logs-Connector

- Miro Enterprise-Preisplan + Enterprise Guard Add-on.
- OAuth-Geltungsbereich: `contentlogs:export`.
- Zugriffstoken.
- Miro Unternehmens-ID.

## Installation

Es gibt zwei Möglichkeiten, die Miro-Konnektoren einzurichten.

- **Option 1 (empfohlen):** Verwenden Sie Enterprise-Integrationen. Einfachste Einrichtung mit automatischer Token-Generierung.
- **Option 2 (alternativ):** Erstellen Sie eine benutzerdefinierte OAuth-App. Mehr Kontrolle über die Konfiguration der OAuth-App.

**Hinweis:** Bei Verwendung von Option 1 wird die Integration automatisch dem Team mit der größten Anzahl an Nutzern in deiner Organisation zugeordnet. Bei Verwendung von Option 2 kannst du wählen, welchem Team die App installiert werden soll. Die Teamwahl beeinflusst jedoch nicht, welche Protokolle gesammelt werden. Beide Optionen ermöglichen den organisationsweiten Zugriff auf Protokolle. Alle für die Integration relevanten Ereignisse von allen Teams sind in deinen Protokollen enthalten.

### Option 1: Enterprise-Integrationen nutzen (empfohlen)

Dies ist die einfachste Option für die meisten Nutzer. Sie erstellt automatisch eine OAuth-Anwendung und generiert ein Zugriffstoken für dich über die Enterprise-Integrationen von Miro.

#### Für den Audit-Protokoll-Connector

1. Öffne die [Miro Unternehmenseinstellungen](https://miro.com/app/settings/).
2. Erweitere den Abschnitt **Apps und Integrationen**.
3. Klicke auf **Enterprise-Integrationen**.
4. Aktiviere den **SIEM**-Schalter.
5. Kopiere den Wert des **Access Tokens**, der angezeigt wird.
6. Speichere das Token sicher.

#### Für den Content-Logs-Connector

1. Öffne die [Miro-Unternehmenseinstellungen](https://miro.com/app/settings/).
2. Erweitere den Bereich **Apps und Integrationen**.
3. Klicke auf **Enterprise-Integrationen**.
4. Aktiviere den **eDiscovery**-Schalter.
5. Kopiere den angezeigten **Access Token**-Wert.
6. Hole deine **Organisations-ID** aus der Browser-URL:
   - Suche in der Browser-URL nach deiner Organisations-ID.
   - Das URL-Format lautet: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Kopiere deine Organisations-ID aus der URL (den numerischen Wert).
7. Speichere sowohl das Token als auch die Organisations-ID sicher.

### Option 2: Verwendung einer benutzerdefinierten OAuth-App (Alternativ)

Diese Option gibt Ihnen mehr Kontrolle über die Konfiguration der OAuth-App. Verwenden Sie diese, wenn Sie Geltungsbereiche anpassen, mehrere Integrationen verwalten oder die manuelle App-Verwaltung bevorzugen.

#### Schritt 1: Miro OAuth-App erstellen

1. Melde dich in deinem Miro-Konto an.
2. Gehe zu den [Miro-App-Einstellungen](https://miro.com/app/settings/user-profile/apps).
3. Klicke auf **Neue App erstellen**.
4. Wähle die Option **Nicht ablaufendes Zugangstoken** während der App-Erstellung ([mehr über OAuth-Tokens erfahren](https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens)).
5. Aktiviere die erforderlichen OAuth-Geltungsbereiche:
   - `auditlogs:read` für den Audit-Protokoll-Connector.
   - `contentlogs:export` für den Content-Log-Connector (erfordert Enterprise Guard).
6. Klicke auf **App installieren und OAuth-Token erhalten**.
7. Kopiere den **Access Token** und speichere ihn sicher.

Für detaillierte OAuth-Setup-Anweisungen siehe [Erste Schritte mit OAuth](https://developers.miro.com/docs/getting-started-with-oauth).

#### Schritt 2: Holen Sie die Organisations-ID (nur für Inhaltsprotokolle)

1. Gehe zu [Miro Unternehmenseinstellungen](https://miro.com/app/settings/).
2. Schau dir die URL im Browser an, um deine Organisations-ID zu finden:
   - Das URL-Format lautet: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Kopiere deine Organisations-ID aus der URL (den numerischen Wert).

### Lösung in Microsoft Sentinel bereitstellen

1. Navigiere in Microsoft Sentinel zu **Content Hub**.
2. Suche nach **„Miro“** und klicke auf die Lösung.
3. Klicke auf **Installieren** und folge dem Bereitstellungsassistenten.
4. Wähle dein Log Analytics-Arbeitsbereich aus.
5. Schließe die Installation ab.

### Daten-Connectoren konfigurieren

#### Miro Audit-Protokolle-Connector

1. Gehe in Microsoft Sentinel zu **Daten-Connectors**.
2. Finde **Miro Audit-Protokolle (Enterprise Plan)** und klicke auf **Connector-Seite öffnen**.
3. Klicke auf **Verbinden**.
4. Gib dein **Access Token** ein.
5. Klicke auf **Verbinden**, um den Connector zu aktivieren.

#### Miro-Content-Protokolle-Connector

1. Gehe in Microsoft Sentinel zu **Datenverbinder**.
2. Finde **Miro-Inhaltsprotokolle (Enterprise Plan + Enterprise Guard)** und klicke auf **Verbinderseite öffnen**.
3. Klicke auf **Verbinden**.
4. Gib deine **Organisations-ID** ein.
5. Gib deinen **Zugriffstoken** ein.
6. Klicke auf **Verbinden**, um den Verbinder zu aktivieren.

Die Datenaufnahme beginnt 5–10 Minuten nach der Aktivierung des Verbinders.

## Tabellen

### MiroAuditLogs_CL

Audit-Ereignisse auf Organisationsebene umfassen:

- Nutzerauthentifizierung und -zugriff.
- Inhaltsoperationen.
- Änderungen in Teams und Organisationen.
- Änderungen an Nutzerprofilen.
- Administrative Aktionen.

**Wichtige Spalten**

| Spalte | Beschreibung |
| --- | --- |
| `TimeGenerated` | Ereignis-Zeitstempel. |
| `event` | Ereignisname, der die spezifische Aktion oder Aktivität identifiziert. |
| `logType` | Art des Logeintrags. |
| `category` | Ereigniskategorie, die verwandte Ereignisse gruppiert. |
| `createdBy_email` | Nutzer, der das Ereignis ausgelöst hat. |
| `context_ip` | IP-Adresse des Ereignisses. |
| `details` | Zusätzliche, ereignisspezifische Informationen (JSON). |

### MiroContentLogs_CL

Aktivitätsprotokolle auf Inhaltsebene umfassen:

- Elementbezogene Vorgänge mit Nutzerzuordnung und Zeitstempel.
- Zustandsübergänge und -änderungen.
- Aktivitätsüberwachung für Compliance und eDiscovery.

**Wichtige Spalten**

| Spalte | Beschreibung |
| --- | --- |
| `TimeGenerated` | Ereignis-Zeitstempel. |
| `actionType` | Typ der auf den Inhalt ausgeführten Aktion. |
| `actor_email` | Benutzer, der die Aktion ausgeführt hat. |
| `itemType` | Art des betroffenen Inhaltsobjekts. |
| `contentId` | Eindeutiger Bezeichner des Inhalts. |
| `state` | Informationen zum Objektzustand (JSON). |

## Beispielabfragen

### Neueste Auditergebnisse ansehen

```
MiroAuditLogs_CL
| sort by TimeGenerated desc
| project TimeGenerated, event, category, createdBy_email, context_ip
| take 20
```

### Aktivität nach Nutzer und Ereignistyp

```
MiroAuditLogs_CL
| summarize EventCount = count() by createdBy_email, event, category
| order by EventCount desc
```

### Inhaltsänderungen nach Nutzer

```
MiroContentLogs_CL
| where TimeGenerated > ago(7d)
| summarize Changes = count() by actor_email, actionType
| order by Changes desc
```

### Ereignistrends über die Zeit

```
MiroAuditLogs_CL
| summarize count() by event, bin(TimeGenerated, 1h)
| render timechart
```

### Aktivste Nutzer (Inhaltsänderungen)

```
MiroContentLogs_CL
| where TimeGenerated > ago(30d)
| summarize TotalActions = count() by actor_email
| top 10 by TotalActions desc
```

## Fehlerbehebung

### Keine Daten erscheinen

- Überprüfe, ob das Zugriffstoken gültig ist und die richtigen Geltungsbereiche hat.
- Bestätige für Inhaltsprotokolle, dass deine Organisation das Enterprise Guard Add-on hat.
- Vergewissere dich, dass die Organisations-ID korrekt ist (für Inhaltsprotokolle).
- Warte 5–10 Minuten auf die erste Datenaufnahme.
- Überprüfe den Status des Connectors auf der Seite **Daten-Connectors**.

### Authentifizierungsfehler

#### Wenn Option 1 verwendet wird (Enterprise-Integrationen umschalten)

- Gehe zu den [Miro Unternehmenseinstellungen](https://miro.com/app/settings/), erweitere den Abschnitt **Apps und Integrationen** und klicke auf **Enterprise-Integrationen**.
- Stelle sicher, dass der Schalter (SIEM für Audit-Protokolle, eDiscovery für Inhaltsprotokolle) noch aktiviert ist.
- Falls ein anderer Admin den Schalter deaktiviert hat, wird das Token ungültig.
- Aktiviere den Schalter erneut, um ein neues Token zu erstellen, und aktualisiere die Konnektorkonfiguration.
- Stelle sicher, dass du die Rolle des Unternehmens-Admins in Miro hast.

#### Wenn Option 2 (benutzerdefinierte OAuth-App) verwendet wird

- Überprüfe, ob das Token in den [Miro-App-Einstellungen](https://miro.com/app/settings/user-profile/apps) nicht widerrufen wurde.
- Stelle sicher, dass die OAuth-App die erforderlichen Geltungsbereiche aktiviert hat.
- Erneuere das Token bei Bedarf und aktualisiere es in der Konnektorkonfiguration.
- Stelle sicher, dass du die Rolle des Unternehmens-Admins in Miro hast.

### Inhaltsprotokolle funktionieren nicht

- Bestätige, dass dein Miro-Preisplan das **Enterprise Guard** Add-on umfasst (nicht im Basis-Enterprise-Preisplan enthalten).
- Stelle sicher, dass der OAuth-Geltungsbereich `contentlogs:export` aktiviert ist.
- Überprüfe, ob die Organisations-ID korrekt ist.
- Wende dich an deinen Miro-Kontomanager, wenn du ein Upgrade auf Enterprise Guard benötigst.

## Ressourcen

### Ressourcen des Miro-Hilfecenters

- **Miro-Audit-Protokolle:** `../security-integrations/security-management/01-audit-logs.md
- **Miro-Inhaltsprotokolle:** `../canvas-25-admin-features/ediscovery/06-content-logs-overview.md
- **Miro-Sentinel-Integrationsleitfaden:** `01-microsoft-sentinel-integration.md`.

### Miro-Entwicklerdokumentation

- **Erste Schritte mit der Enterprise API:** `https://developers.miro.com/docs/getting-started-with-enterprise-api`.
- **Erste Schritte mit OAuth:** `https://developers.miro.com/docs/getting-started-with-oauth`.
- **OAuth-Token-Authentifizierung:** `https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens`.
- **Audit-Protokolle-API:** `https://developers.miro.com/reference/enterprise-get-audit-logs`.
- **Inhaltsprotokoll-API:** `https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch`.
- **API-Referenz:** `https://developers.miro.com/reference`.

### Microsoft Sentinel

- **Microsoft Sentinel Dokumentation:** `https://docs.microsoft.com/azure/sentinel/`.
