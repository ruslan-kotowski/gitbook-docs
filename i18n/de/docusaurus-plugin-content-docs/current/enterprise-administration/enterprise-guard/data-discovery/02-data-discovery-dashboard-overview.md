---
title: "\xDCbersicht \xFCber das Datenerkennungs-Dashboard"
article_id: 26806897106834
translation_id: 26806897106834
locale: de
sidebar_position: 1
created_at: '2025-05-19T11:10:19Z'
updated_at: '2025-11-25T15:51:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Das Datenerkennungs-Dashboard bietet eine zentrale Ansicht der sensiblen Informationen, die auf den Boards deiner Organisation festgestellt wurden. Es ermöglicht Admins, Datenrisiken zu überwachen, zu klassifizieren und zu verwalten, indem datenschutzbezogene oder geschäftskritische Inhalte identifiziert werden. Das Datenerkennungs-Dashboard enthält die folgenden Kennzahlen:

:::note
Alle Kennzahlen im Enterprise Guard schließen Boards von Papierkorb-Teams und Boards unter Aufbewahrungsfrist aus.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Titel** | **Beschreibung** | **Domain** | **Erscheint im Übersichts-Dashboard** | **Hat bisherige Kennzahl** |
| Anzahl der sensiblen Boards | Anzahl der Boards, denen mindestens ein integriertes Label, ein Suchbegriff-Label oder ein Datenschutzlabel zugewiesen ist | Datenerkennung | ✅ | ❌ |
| Anzahl der Boards mit geschäftskritischen Elementen | Anzahl der Boards, denen mindestens ein integriertes Label oder ein Suchbegriff-Label zugewiesen wurde | Datenerkennung | ✅ | ✅ |
| Anzahl der Boards mit datenschutzrelevanten sensiblen Inhalten | Anzahl der Boards, denen mindestens ein Datenschutzlabel zugewiesen wurde | Datenerkennung | ✅ | ✅ |
| Anzahl der Boards, denen ein Label zugewiesen ist, pro Label | Zähle für jedes einzelne Label in den drei Kategorien (integriert, Suchbegriff oder Datenschutz) die Anzahl der Boards, die mit diesem Label versehen sind. | Datenerkennung | ❌ | ❌ |
| Anzahl aktivierter datenschutzrelevanter Labels | Anzahl der aktivierten datenschutzrelevanten Labels | Datenerkennung | ❌ | ❌ |
| Anzahl der aktivierten Suchbegriff-Labels | Anzahl der aktivierten Suchbegriff-Labels | Datenerkennung | ❌ | ❌ |
| Anzahl aktivierter geschäftskritischer Labels | Anzahl der aktivierten Labels für geschäftskritische Daten | Datenerkennung | ❌ | ❌ |

## Fehler, leere Zustände und bisherige Änderungen verstehen

Zum Verständnis der Kennzahlen auf dem Enterprise Guard-Dashboard ist es unerlässlich, zu wissen, wie leere Zustände und Fehlermeldungen zu interpretieren sind.

### Verstehen, wie sich bisherige Daten bei Änderung der Einstellungen verhalten

Wenn die Datenerkennung deaktiviert wird, nachdem Daten gesammelt wurden, zeigen die bisherigen Kennzahlen weiterhin Werte aus dem aktiven Zeitraum an. Zum Beispiel, wenn du die Datenerkennung im Mai deaktivierst und die Datenerkennung im April aktiv war:

- April-Werte werden weiterhin auf dem Dashboard angezeigt.
- Die Mai-Grafik wird **keine Daten verfügbar** anzeigen, da die Datenerfassung gestoppt wurde.

## Ergebnisse der Datenerkennung anzeigen

Der Datenerkennungszyklus läuft mindestens einmal pro Stunde und durchsucht alle Board-Updates nach datenschutzrelevanten, geschäftskritischen oder benutzerdefinierten geschäftskritischen Informationen gemäß deiner Datenerkennungskonfiguration. Dazu zählen auch Boards, die bereits im vorherigen Datenerkennungszyklus gescannt wurden.

Die Ergebnisse der Datenerkennung erscheinen unter den Diagrammen mit den Kennzahlen. Du kannst Informationen wie den Label-Namen, Status, Typ, Klassifizierung, die Anzahl der Boards und so weiter ansehen.

Weitere Informationen über das Überprüfen von Boards mit datenschutzrelevanten Dokumentationen findest du in [diesem Artikel](16-review-boards-with-privacy-related-information.md).

Für weitere Informationen zur Überprüfung von Boards mit geschäftskritischen und benutzerdefinierten, geschäftskritischen Dateninformationen, [siehe diesen Artikel](14-review-boards-with-business-sensitive-and-custom-business-sensitive-information-beta.md).

Weitere Informationen zum Überprüfen von Boards mit benutzerdefinierten, geschäftskritischen Labels findest du [in diesem Artikel](15-review-custom-business-sensitive-labels-and-data-discovery-results.md).

:::note
- Um die Ergebnisse der Datenerkennung anzusehen, musst du die [Rolle des Admins für sensible Inhalte](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) haben. Die Rolle des Admins für sensible Inhalte kannst du bei deinem Unternehmens-Admin anfordern.

Obwohl wir kontinuierlich mit unseren Technologiepartnern und Kunden an der Verbesserung des Systems zur Erkennung sensibler Inhalte arbeiten, können wir nicht garantieren, dass 100 % der sensiblen Daten auf deinen Boards gefunden und markiert werden. Unser System zur Erkennung sensibler Inhalte verwendet Muster und andere Kriterien, um die Wahrscheinlichkeit einer Übereinstimmung zu bestimmen. Es kann vorkommen, dass das System Daten auf deinen Boards fälschlicherweise als wahrscheinlich sensibel kennzeichnet (falsch positiv) oder Daten nicht als sensibel kennzeichnet (falsch negativ). Dies wird von verschiedenen Faktoren beeinflusst, z. B. von der Nähe verwandter Begriffe oder der Formatierung sensibler Daten.

Weitere Informationen darüber, wie du falsch positive Übereinstimmungen unterdrücken kannst, findest du unter [Unterdrückung eines Treffers mit sensiblem Inhalt](11-suppress-a-sensitive-content-match.md).
:::

##

##
