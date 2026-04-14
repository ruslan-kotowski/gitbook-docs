---
title: "\xDCbersicht \xFCber Audit-Protokolle von Enterprise Guard"
article_id: 17331872857746
translation_id: 17331872857746
locale: de
sidebar_position: 0
created_at: '2024-02-27T21:08:55Z'
updated_at: '2025-11-25T15:41:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Audit-Protokolle bieten Admins einen umfassenden Eintrag aller Ereignisse im Zusammenhang mit Enterprise Guard. Diese Protokolle sind eine wertvolle Ressource für die effiziente Fehlerbehebung und bieten detaillierte Einblicke in kritische Ereignisse, wie z. B. Aktualisierungen der Papierkorb-Aufbewahrungsrichtlinie und der Berechtigungsrichtlinie für gelöschte Boards, die Erstellung, Aktualisierung oder Löschung von Aufbewahrungsrichtlinien für die Organisation oder die endgültige Löschung eines Boards aus dem Papierkorb. Das systematische Verfolgen dieser Aktivitäten stärkt die Überwachung, Analyse und Wartung und gewährleistet ein sicheres und gut verwaltetes System.

## Ereignisse von Enterprise Guard in Audit-Protokollen

Zusätzlich zu [den bestehenden protokollierten Ereignissen](../../security-integrations/security-management/01-audit-logs.md) enthalten die Audit-Protokolle Datensätze über die folgenden Ereigniskategorien und Ereignisse im Zusammenhang mit Enterprise Guard.

### Papierkorbrichtlinie

In der folgenden Tabelle sind die Ereigniskategorien und -aktionen aufgeführt, die für die Komponente der Papierkorbrichtlinie der Organisation protokolliert werden.

|  |  |
| --- | --- |
| **Ereigniskategorie** | **Ereignisaktion** |
| Verwaltung | Papierkorb-Zeit-zu-leben-Richtlinie für die Organisation geändert |
| Verwaltung | Die Berechtigungsrichtlinie für gelöschte Boards in der Organisation wurde geändert. |

*Tabelle 1: Ereigniskategorien und Ereignisaktionen, die für die Komponente "Organisations-Papierkorb-Richtlinie" protokolliert werden*Weitere Informationen zu Papierkorb-Richtlinien findest du in [unserer Dokumentation](https://help.miro.com/hc/articles/13860817985426-Trash-Policy).

### Aufbewahrungsrichtlinie

Die folgende Tabelle listet die Ereigniskategorien und Ereignisaktionen auf, die für die Komponente "Inhaltsaufbewahrungsrichtlinien" protokolliert werden.

|  |  |
| --- | --- |
| **Ereigniskategorie** | **Ereignisaktion** |
| Verwaltung | Aufbewahrungsrichtlinie für die Organisation erstellt |
| Verwaltung | Aufbewahrungsrichtlinie für die Organisation aktualisiert |
| Verwaltung | Aufbewahrungsrichtlinie für die Organisation gelöscht |

*Tabelle 2: Ereigniskategorien und Ereignisaktionen, die für die Komponente "Inhaltsaufbewahrungsrichtlinien" protokolliert werden.*Weitere Informationen zu Aufbewahrungsrichtlinien findest du in [unserer Dokumentation](https://help.miro.com/hc/articles/16855776325778-Retention-Beta).

### Datenerkennung

Die folgende Tabelle listet die Ereigniskategorien und -aktionen auf, die für die Content Discovery-Komponente protokolliert wurden.

|  |  |
| --- | --- |
| **Ereigniskategorie** | **Ereignisaktion** |
| Verwaltung | Erkennung privater Informationen für die Organisation geändert  (aktiviert/deaktiviert) |
| Verwaltung | Ein Datenerkennungstreffer in der Organisation wurde unterdrückt. |

*Tabelle 3: Ereigniskategorien und Ereignisaktionen, die für die Content Discovery-Komponente protokolliert wurden*

Weitere Informationen zur Datenerkennung findest du in unserer [Dokumentation](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md).

### Intelligente Vorgaben

In der nachstehenden Tabelle sind die Ereigniskategorien und -aktionen aufgeführt, die für die Intelligente Vorgaben-Komponente protokolliert werden.

|  |  |
| --- | --- |
| **Ereigniskategorie** | **Ereignisaktion** |
| Intelligente Vorgaben | Intelligente Vorgaben für ein Board geändert |

*Tabelle 4: Ereigniskategorien und -aktionen, die für die Intelligente Vorgaben-Komponente protokolliert werden*

Weitere Informationen zu den Intelligenten Vorgaben findest du in [unserer Dokumentation](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md).

### eDiscovery

In der nachstehenden Tabelle sind die Ereigniskategorien und -aktionen aufgeführt, die für die eDiscovery-Komponente protokolliert werden.

|  |  |
| --- | --- |
| **Ereigniskategorie** | **Ereignisaktion** |
| Verwaltung | Untersuchung für die Organisation erstellt |
| Verwaltung | Untersuchung für die Organisation abgeschlossen |
| Verwaltung | Aufbewahrungsfrist für die Organisation erstellt |
| Verwaltung | Aufbewahrungsfrist für die Organisation geschlossen |
| Verwaltung | Aufbewahrungsfrist auf das Board angewendet Board aus der Aufbewahrungsfrist freigegeben |

*Tabelle 3: Ereigniskategorien und Ereignisaktionen, die für die eDiscovery-Komponente protokolliert werden*

Weitere Informationen zu eDiscovery findest du in [unserer Dokumentation](https://help.miro.com/hc/sections/22049853357842-eDiscovery-Legal-Hold-Beta).
