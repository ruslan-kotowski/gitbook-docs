---
title: Inhaltsprotokolle
article_id: 17774729839378
translation_id: 17774729839378
locale: de
sidebar_position: 5
created_at: '2024-03-19T13:00:06Z'
updated_at: '2026-03-15T21:32:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
availability:
  notes: 'Eingerichtet von: Unternehmens-Admins, Sicherheits-Admins'
---

Inhaltsprotokolle ermöglichen es Unternehmenskunden, detaillierte Aufzeichnungen über Nutzeraktivitäten auf Boards zu sammeln und sie für Untersuchungen oder regulatorische Archivierung zu nutzen.

Inhaltsprotokolle können in verschiedene speziell entwickelte Tools für rechtliche, Compliance- und Sicherheitszwecke aufgenommen werden. Durch die Bereitstellung einer Lösung zum großflächigen Exportieren von Nutzerdaten verringert Miro das Risiko für Kunden und eröffnet Wissensarbeitern in Unternehmen die Möglichkeit, die kollaborative Kraft von Miro zu erleben, während sie strenge Sicherheits- und Compliance-Anforderungen beachten.

## Inhaltsprotokolldaten

Wenn ein Nutzer ein Widget auf dem Board aktualisiert, wird ein Protokolleintrag erstellt, der Informationen wie die Zeit der Nutzeraktion, Nutzerdetails, die Art der Aktion (erstellen, aktualisieren, löschen), Board- und Widget-IDs sowie andere relevante Informationen über den Zustand des Widgets infolge der Nutzeraktionen enthält. Inhaltsprotokolle *zeichnen* jedoch keine Aktualisierungen in Bezug auf Position, Größe oder Drehung des Widgets auf.

## Inhaltsprotokolle sammeln

Die Ereignisse werden ab dem Moment protokolliert, in dem ein Admin die Sammlung von Inhaltsprotokollen aktiviert. Gesammelte Ereignisse werden standardmäßig 30 Tage lang gespeichert.

Um die Sammlung von Inhaltsprotokollen zu aktivieren, führe folgende Schritte aus:

1. Gehe zu den Unternehmenseinstellungen.
2. Klicke im linken Feld auf **Sicherheit** > **Prüfungsprotokolle**.
3. Klicke unter **Prüfungsprotokolle** auf den **Einstellungen**-Tab.
4. Klicke im Bereich **Inhaltsprotokolle** auf die Umschaltfläche, um **Inhaltsprotokolle zu sammeln**.
   ![content_logs.png](images/24936983713298_content_logs.png)
   *Aktivieren der Sammlung von Inhaltsprotokollen*

## Zugriff auf Inhaltsprotokolle über die API

Admins können die [Content Logs API](https://developers.miro.com/reference/board-content-logs) verwenden, um programmatisch auf Daten der Inhaltsprotokolle innerhalb ihrer Organisation zuzugreifen. Admins können auch Integrationen wie Smarsh oder Theta Lake nutzen, um Inhaltsprotokolldaten zu sammeln.

Um den Zugriff auf die API zu authentifizieren, können Admins aus den folgenden Optionen wählen:

- eDiscovery-Umschalter in den Enterprise Integrations aktivieren.
- Eine Plattform-App erstellen und ihr Zugriff auf den Geltungsbereich Content log:read geben.
- Eine der eDiscovery-Integrationen aus dem Marketplace installieren und autorisieren.

## Löschen von Inhaltsprotokollen

Admins können eine Aufbewahrungsrichtlinie für Inhaltsprotokolle festlegen, und zwischen 30, 90, 180 oder 365 Tagen wählen. Standardmäßig ist der Aufbewahrungszeitraum auf 30 Tage gesetzt.

:::note
Sobald Inhaltsprotokolle gelöscht sind, können sie nicht wiederhergestellt werden.
:::

Um eine Löschfrist festzulegen, führe die folgenden Schritte aus:

1. Gehe zu den Unternehmenseinstellungen.
2. Klicke im linken Feld auf **Sicherheit** > **Audit-Protokolle**.
3. Klicke unter **Audit-Protokolle** auf den Tab **Einstellungen**.
4. Wähle unter **Inhaltsprotokolle** eine Option aus der Dropdown-Liste aus. Du wirst aufgefordert, deine Wahl zu bestätigen.
   ![content_logs_duration.png](images/24936983717778_content_logs_duration.png)
   *Aufbewahrungsrichtlinie für Inhaltsprotokolle festlegen*
