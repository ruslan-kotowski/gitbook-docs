---
title: "\xDCbersicht \xFCber das Klassifizierungs-Dashboard"
article_id: 26886219054354
translation_id: 26886219054354
locale: de
sidebar_position: 3
created_at: '2025-05-22T11:26:15Z'
updated_at: '2025-08-18T09:36:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Das Klassifizierungs-Dashboard bietet eine zentrale Ansicht für Admins, um die Klassifizierung von Boards in ihrer Organisation zu verfolgen und zu verwalten. Das Dashboard bietet eine klare Aufschlüsselung von klassifizierten und noch nicht klassifizierten Boards, was hilft, eine umfassende Abdeckung sicherzustellen und Bereiche zu identifizieren, die Aufmerksamkeit benötigen.

Admins können auch die verwendete Klassifizierungsmethode überwachen – ob manuell, automatisch oder nicht klassifiziert – um zu verstehen, wie Boards kategorisiert werden. Zusätzlich visualisiert die Klassifizierungsmethode den Verlauf von Änderungen über die Zeit und bietet Einblicke in Trends sowie die Effektivität der laufenden Board-Klassifizierungen.

:::note
Hinweise zu Kennzahlen:

- Alle Kennzahlen in Enterprise Guard schließen Boards von Teams im Papierkorb und Boards unter Aufbewahrungsfrist aus.
- Alle Klassifizierungskennzahlen schließen Vorlagen und Boards im Papierkorb aus.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Titel** | **Beschreibung** | **Domain** | **Erscheint im Übersichts-Dashboard** | **Hat bisherige Kennzahl** |
| Gesamtanzahl der klassifizierten Boards | Anzahl der Boards, denen ein Klassifizierungslabel zugewiesen ist | Klassifizierung | ✅ | ❌ |
| Anzahl der Boards pro Klassifizierung | Anzahl der Boards pro Klassifizierungslabel (Labelname) | Klassifizierung | ✅ | ❌ |
| Anzahl der nicht klassifizierten Boards | Anzahl der Boards, denen kein Klassifizierungslabel zugewiesen ist | Klassifizierung | ✅ | ✅ |
| Anzahl der manuell klassifizierten Boards | Anzahl der Boards, denen manuell ein Klassifizierungslabel zugewiesen ist (nicht durch automatische Klassifizierung) | Klassifizierung | ❌ | ✅ |
| Anzahl der automatisch klassifizierten Boards | Anzahl der Boards mit einem automatisch zugewiesenen Klassifizierungslabel durch die automatische Klassifizierung | Klassifizierung | ❌ | ✅ |

## Fehler, leere Zustände und bisherige Änderungen verstehen

Zum Verständnis der Kennzahlen auf dem Enterprise Guard-Dashboard ist es unerlässlich, zu wissen, wie leere Zustände und Fehlermeldungen zu interpretieren sind.

### Verstehen, wie sich bisherige Daten bei Änderung der Einstellungen verhalten

Wenn eine Funktion, wie die Klassifizierung, deaktiviert wird, nachdem Daten gesammelt wurden, zeigen die bisherigen Kennzahlen weiterhin Werte aus dem aktiven Zeitraum an. Zum Beispiel, wenn du die Klassifizierung im Mai deaktivierst und die Klassifizierung im April aktiv war und 20 Boards klassifiziert wurden:

- April-Werte werden weiterhin auf dem Dashboard angezeigt.
- Die Mai-Grafik wird **keine Daten verfügbar** anzeigen, da die Datenerfassung gestoppt wurde.
