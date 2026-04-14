---
title: KI-Interaktionsprotokolle (Betaversion)
article_id: 34049604547858
translation_id: 34049604547858
locale: de
sidebar_position: 1
created_at: '2026-03-15T21:28:41Z'
updated_at: '2026-03-16T09:09:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

KI-Interaktionsprotokolle ermöglichen es Admins mit dem Enterprise Guard Add-on, Aufzeichnungen über die Nutzung von Miro AI in ihrer Organisation zu sammeln und zu überprüfen. Durch die Aktivierung von KI-Interaktionsprotokollen können Admins Sicherheits-, Compliance- und Governance-Teams mehr Einblick darüber geben, wie KI-Funktionen genutzt werden und welche Informationen von KI-Systemen verarbeitet werden.

KI-Interaktionsprotokolle unterstützen Organisationen dabei:

- Zu überwachen, wie KI-Funktionen in der Organisation genutzt werden
- Governance-, Compliance- und Sicherheitsüberprüfungen zu unterstützen
- Einblick in die mit KI-Systemen geteilten Informationen zu gewähren
- Vertrauen zu stärken und die verantwortungsvolle Einführung von KI-Tools zu fördern

KI-Interaktionsprotokolle erfassen Aufzeichnungen von Interaktionen zwischen Nutzern und KI-gesteuerten Funktionen in Miro. Diese Aufzeichnungen helfen Organisationen dabei, die Nutzung von KI in der gesamten Organisation zu überprüfen und interne Prüfungs-, Governance- und Compliance-Prozesse zu unterstützen.

Wenn aktiviert, erfassen KI-Interaktionsprotokolle:

- Von Nutzern eingereichte Prompts an KI-Funktionen
- Vom System zurückgegebene KI-generierte Antworten
- Systemkontext im Zusammenhang mit der Interaktion

## Bevor Sie beginnen

- Du musst Admin sein, um KI-Interaktionsprotokolle zu aktivieren oder zu konfigurieren.
- Das Enterprise Guard Add-on ist erforderlich, um diese Funktion zu nutzen.
- Bevor mit der Datenerfassung begonnen wird, müssen KI-Interaktionsprotokolle aktiviert werden.
- Nur Interaktionen, die nach der Aktivierung der Protokollierung stattfinden, werden aufgezeichnet.

## KI-Interaktionsprotokolle aktivieren

1. Gehe zur **Admin-Konsole**.
2. Wähle **Sicherheit** aus.
3. Klicke auf **Prüfprotokolle**.
4. Öffne den **Einstellungen**-Tab.
5. Aktiviere im Bereich **KI-Interaktionsprotokolle** die Option **KI-Interaktionsprotokolle sammeln**.
6. Wähle die **Protokoll-Aufbewahrungsfrist** aus.
7. Speichere deine Änderungen.

Nachdem du diese Einstellung aktiviert hast, beginnt Miro damit, KI-Interaktionsprotokolle für neue KI-Interaktionen zu sammeln.

## Protokoll-Aufbewahrung konfigurieren

Admins können konfigurieren, wie lange KI-Interaktionsprotokolle gespeichert werden.

1. Gehe zu **Admin-Konsole > Sicherheit > Audit-Protokolle**.
2. Wähle im Bereich **KI-Interaktionsprotokolle** die gewünschte **Aufbewahrungsfrist**.
3. Speichere deine Änderungen.

Protokolle werden automatisch gelöscht, wenn die konfigurierte Aufbewahrungsfrist abläuft.

## Zugriff auf KI-Interaktionsprotokolle über APIs

KI-Interaktionsprotokolle können über die KI-Interaktionsprotokoll-API abgerufen werden.

Dies ermöglicht es Organisationen, KI-Interaktionsdaten mit ihren bestehenden Governance-, Compliance- oder Sicherheitsüberwachungssystemen zu exportieren und zu analysieren.

Häufige Anwendungsbeispiele umfassen:

- KI-Governance und Aufsicht
- Sicherheitsüberwachung
- Compliance-Prüfung
- Interne Untersuchungen

Weitere Informationen finden Sie in der [Entwicklerdokumentation](https://developers.miro.com/reference/enterprise-get-ai-interaction-logs).

## Einschränkungen

Die aktuelle Version umfasst die erste Version des KI-Interaktionsprotokolls. Die folgenden Einschränkungen gelten:

- Werkzeugaufrufe aus KI-Funktionen werden derzeit nicht protokolliert.
- Interaktionen im Zusammenhang mit Miro MCP-Integrationen werden derzeit nicht protokolliert.
- Moderationsereignisse und sensible Eingabeaufforderungen werden derzeit nicht protokolliert.
- Bilder sind in KI-Interaktionsprotokollen nicht enthalten.
