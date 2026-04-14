---
title: "Board Export API \xDCbersicht"
article_id: 17774560667794
translation_id: 17774560667794
locale: de
sidebar_position: 12
created_at: '2024-03-19T12:52:09Z'
updated_at: '2025-07-09T17:32:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

[eDiscovery-APIs](https://developers.miro.com/reference/enterprise-create-board-export) ermöglichen es Kunden des Enterprise-Preisplans, Board-Daten aus Miro zu exportieren, um sie manuell zu überprüfen oder in eigens entwickelte Tools für Rechts-, Compliance- und Sicherheitszwecke einzupflegen.

Die Board-Export-API liefert eine ZIP-Datei mit einem Snapshot der Board-Daten zum Zeitpunkt der Ausführung des Jobs, einschließlich des Exports des Board-Inhalts in einem bestimmten Format (SVG, PDF oder HTML), eine JSON-Datei mit einer Aufzeichnung aller Kommentare, eine JSON-Datei mit einer Liste aller Nutzer, die das Board angesehen oder geändert haben, ggf. Videoaufzeichnungen von TalkTrack-Webcam-Aufnahmen, die mit dem Board verbunden sind, und eine JSON-Datei mit Board-Matadaten. Bei großen Boards erzeugt der Export im PDF-Format mehrere PDF-Dateien, die das gesamte Board abbilden.

Das asynchrone API-Design umfasst Endpunkte zum Abrufen von Informationen über einen Board-Exportauftrag, wie z. B. den Status.

:::note
Wenn du den Enterprise-Preisplan nutzt, kannst du immer nur einen Board-Exportauftrag ausführen. Als Enterprise Guard-Kunde kannst du bis zu fünf Boards gleichzeitig exportieren, und das mit einer deutlich höheren Exportgeschwindigkeit.
:::

## Anwendungsfälle

Einige der häufigsten Anwendungsbeispiele für eDiscovery sind:

- **eDiscovery (Electronic Discovery):** Der Prozess der Identifizierung, Sammlung, Aufbewahrung und Überprüfung elektronisch gespeicherter Informationen zur Verwendung in einer Rechtsangelegenheit.
- **Informationsarchiv:** Eine Praxis, bei der Organisationen Daten außerhalb des ursprünglichen Systems für die langfristige Speicherung und Aufbewahrung aufbewahren. Die Inhalte und Metadaten helfen den Kunden, das Archiv zu indizieren und zu durchsuchen und proaktiv auf Compliance-Probleme zu achten.
