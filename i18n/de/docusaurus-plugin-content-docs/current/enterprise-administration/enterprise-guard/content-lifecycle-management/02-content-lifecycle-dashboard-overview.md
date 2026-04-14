---
title: "Content Lifecycle-Dashboard im \xDCberblick"
article_id: 26894063726482
translation_id: 26894063726482
locale: de
sidebar_position: 2
created_at: '2025-05-22T16:02:58Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

Das Content Lifecycle-Dashboard bietet Admins eine zentrale Ansicht, um den gesamten Lifecycle von Boards zu überwachen und zu verwalten – von der Erstellung bis zur Löschung – und gleichzeitig mit den Aufbewahrungsrichtlinien der Organisation in Einklang zu bleiben. Es bietet Einblick in die aktuelle Lebenszyklusphase jedes Boards und hilft dabei, eine angemessene Handhabung der Inhalte sicherzustellen.

Admins können auch Boards verfolgen, die durch Aufbewahrungs- und Löschungsrichtlinien geregelt sind, und historische Trends bei der Richtlinienanwendung ansehen. Das Dashboard enthält eine Prognose zur Löschung, die proaktive Planung für kommende automatisierte Lebenszyklusaktionen ermöglicht. Dies ermöglicht eine konsistente, richtliniengesteuerte Inhaltsverwaltung in der gesamten Organisation.

:::note
Alle Kennzahlen im Enterprise Guard schließen Boards von gelöschten Teams und Boards unter Aufbewahrungsfrist aus.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Titel** | **Beschreibung** | **Domain** | **Erscheint im Übersichts-Dashboard** | **Hat bisherige Kennzahl** |
| Gesamtanzahl der Boards | Gesamtzahl der Boards in allen Stadien des Lebenszyklus (aktiv, Papierkorb, in der Aufbewahrung) | Inhaltslebenszyklus-Management | ✅ | ❌ |
| Anzahl aktiver Boards. Beachte, dass dies NICHT die Aktivität der Boards ist, sondern Boards, die sich im aktiven Lebenszyklusstadium befinden. | Gesamtanzahl der Boards im aktiven Lebenszyklusstadium | Inhaltslebenszyklus-Management | ✅ | ✅ |
| Anzahl der Boards im Papierkorb | Gesamtanzahl der Boards im Lebenszyklusstadium „im Papierkorb“ | Content Lifecycle Management | ✅ | ✅ |
| Anzahl der Boards in Aufbewahrung | Gesamtzahl der Boards im Lebenszyklusstadium „in Aufbewahrung“ | Inhaltslebenszyklus-Management | ✅ | ✅ |
| Anzahl der Boards zur Aufbewahrung | Gesamtanzahl der Boards, denen mindestens eine nicht abgelaufene Aufbewahrungsrichtlinie zugewiesen ist | Content Lifecycle Management | ❌ | ✅ |
| Anzahl der Boards zur Löschung | Gesamtanzahl der Boards, denen mindestens eine nicht abgelaufene Löschungsrichtlinie zugewiesen ist | Inhaltslebenszyklus-Management | ❌ | ❌ |
| Anzahl der Boards gemäß einer Aufbewahrungsrichtlinie, gruppiert nach Richtlinien | Anzahl der Boards in einem beliebigen Lebenszyklusstadium, denen mindestens eine Aufbewahrungsrichtlinie zugewiesen ist, pro Richtlinie | Inhaltslebenszyklus-Management | ✅ | ❌ |
| Anzahl der Boards gemäß einer Löschungsrichtlinie gruppiert nach Richtlinien | Anzahl der Boards in jedem Lebenszyklusstadium, denen pro Richtlinie mindestens eine Löschungsrichtlinie zugewiesen wurde | Content Lifecycle Management | ✅ | ❌ |
| Anzahl der erstellten Boards an diesem Tag/in dieser Woche/in diesem Monat | Anzahl der in dieser Woche erstellten Boards | Content Lifecycle Management | ❌ | ✅ |
| Anzahl der Boards, die an diesem Tag/in dieser Woche/in diesem Monat gelöscht (in den Papierkorb verschoben) wurden | Anzahl der in dieser Woche gelöschten (in den Papierkorb verschobenen) Boards | Content Lifecycle Management | ❌ | ✅ |
| Anzahl der Boards unter Löschungsrichtlinien, gruppiert nach effektivem Löschungsrichtliniendatum pro Monat |  | Inhaltslebenszyklus-Management | ❌ | ❌ |

## Fehler, leere Zustände und bisherige Änderungen verstehen

Zum Verständnis der Kennzahlen auf dem Enterprise Guard-Dashboard ist es unerlässlich, zu wissen, wie leere Zustände und Fehlermeldungen zu interpretieren sind.

### Verstehen, wie sich bisherige Daten bei Änderung der Einstellungen verhalten

Wenn die Datenerkennung deaktiviert wird, nachdem Daten gesammelt wurden, zeigen die bisherigen Kennzahlen weiterhin Werte aus dem aktiven Zeitraum an. Zum Beispiel, wenn du die Datenerkennung im Mai deaktivierst und die Datenerkennung im April aktiv war:

- April-Werte werden weiterhin auf dem Dashboard angezeigt.
- Die Mai-Grafik wird **keine Daten verfügbar** anzeigen, da die Datenerfassung gestoppt wurde.

###
