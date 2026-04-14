---
title: "\xDCbersicht zum Board-Export aus der Admin-Konsole"
article_id: 26259747401362
translation_id: 26259747401362
locale: de
sidebar_position: 0
created_at: '2025-04-24T14:18:00Z'
updated_at: '2025-11-25T15:50:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: discovery-board-export
---

eDiscovery-Admins können jetzt Boards unter Aufbewahrungsfrist direkt aus der Admin-Konsole exportieren.
Diese Funktion ermöglicht es eDiscovery-Admins:

- Initiere den Board-Export von der Admin-Konsole aus.
- Überwache den Fortschritt von Exportaufträgen in Echtzeit über den **Exports**-Tab innerhalb jeder Untersuchung.
- Filtere Exportaufträge nach Status und Creator und sieh, welche Boards enthalten sind.
- Erhalte ein vollständiges Inhaltsprotokoll für jedes exportierte Board.
- Sieh dir eine Liste exportierter Boards und deren Metadaten (Klassifizierung, Eigentümer, Exportstatus) an.
- Exportierte Boards einzeln direkt aus der Admin-Konsole herunterladen.
- Schließe den Export-Workflow ab, ohne auf APIs oder Integrationen zurückzugreifen.
- Abgebrochene Exportaufträge in der Warteschlange oder laufende Aufträge abbrechen.

:::note
Um Boards zu exportieren und Exportaufträge zu verwalten, musst du die [eDiscovery-Admin-Rolle](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Um die Admin-Rolle für sensible Inhalte zu beantragen, wende dich an deinen Unternehmens-Admin.
:::

## **Board-Export-Funktionen**

- Jeder **Exportauftrag** kann bis zu **1.000 Boards** enthalten.
- **Exportlimits** nach Preisplan:

  - **Enterprise Guard:** Bis zu **100** aktive Exportaufträge.
  - **Enterprise:** Bis zu **10** aktive Exportaufträge.
- **Grenzen der parallelen Verarbeitung**:

  - **Enterprise Guard**: Bis zu **5** Exportaufträge gleichzeitig verarbeitet.
  - **Enterprise**: **1** Exportauftrag wird gleichzeitig verarbeitet.
- **Inhaltsprotokolle mit Exportaufträgen:** Exporte können optional ein vollständiges Inhaltsprotokoll für jedes exportierte Board enthalten.
- **Filter für Exportaufträge**: Exportaufträge filtern und sehen, welche Boards enthalten sind.
- **Laufende und wartende Exportaufträge abbrechen**: Export-Bandbreite effizient verwalten.
  > ✏️ Wenn du einen Export abbrichst, werden alle laufenden Boards abgeschlossen und zum Herunterladen bereitgestellt. Alle Boards, die nicht gestartet wurden, werden nicht exportiert.

- **Herunterladezugriff**: Ergebnisse sind für **14 Tage** herunterladbar.
- **Geltungsbereich der Admin-Konsole**: Nur Exporte, die über die Admin-Konsole initiiert wurden, erscheinen im **Tab „Exporte“**. API-basierte Exportaufträge sind nicht in der Liste der Admin-Konsole enthalten.
