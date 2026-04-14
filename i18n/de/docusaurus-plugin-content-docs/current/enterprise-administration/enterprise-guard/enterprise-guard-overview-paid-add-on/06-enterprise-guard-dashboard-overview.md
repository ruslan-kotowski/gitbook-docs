---
title: "Enterprise Guard Dashboard im \xDCberblick"
article_id: 26707467343890
translation_id: 26707467343890
locale: de
sidebar_position: 4
created_at: '2025-05-14T13:14:06Z'
updated_at: '2025-11-25T15:51:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

## Zentralisierte Sicherheits- und Governance-Ansicht

Das Enterprise Guard Dashboard bietet eine zentralisierte, umfassende Ansicht der Sicherheits- und Informations-Governance-Einblicke Ihrer Organisation in einer einheitlichen Übersicht. Dieses Dashboard ist für Enterprise Guard Admins konzipiert und fasst zentrale Kennzahlen aus wichtigen Domains – einschließlich Datenerkennung, Klassifizierung, Content Lifecycle und eDiscovery – in einer einzigen, konsolidierten Oberfläche zusammen. Es ermöglicht eine schnelle Sichtbarkeit der aktuellen Gefährdungen, der Abdeckung von Richtlinien und der rechtlichen Einsatzbereitschaft und befähigt Admins, potenzielle Risiken frühzeitig zu erkennen, rechtzeitig proaktive Maßnahmen zu ergreifen und sich mit Bereichen zu befassen, die Aufmerksamkeit erfordern.

## Echtzeit, umsetzbare Kennzahlen

Jede Kennzahl im Enterprise Guard Dashboard spiegelt Echtzeitdaten wider, die täglich aktualisiert werden. Alle Kennzahlen sind umsetzbar und verlinken direkt zu den jeweiligen Domain-Dashboards, was es Admins ermöglicht, detaillierte Einblicke zu erhalten und Einstellungen nach Bedarf zu konfigurieren. Egal, ob du die Empfindlichkeit von Boards, den Klassifizierungsstatus, Aufbewahrungsrichtlinien oder Aufbewahrungsfristen überwachst, dieses Dashboard bietet einen zentralen Ausgangspunkt. Dieser gestufte Ansatz gewährleistet Konsistenz im gesamten Enterprise Guard Produkt und vereinfacht die Navigation für beschäftigte Admins.

## Unterstützung für groß angelegte Governance

Das Enterprise Guard Dashboard ist besonders nützlich für Enterprise Guard Admins, die großangelegte Bereitstellungen im Enterprise-Preisplan verwalten. Es bringt Klarheit in komplexe Informations-Governance-Setups und unterstützt fundierte Entscheidungen, indem es die wichtigsten Signale an einem Ort zusammenführt. Im Rahmen unseres Engagements für ein intuitiveres Enterprise Guard-Erlebnis hilft das Enterprise Guard Dashboard den Admins nicht nur zu verstehen, was passiert, sondern auch, was als Nächstes zu tun ist – mit Links, um direkt aus den Daten heraus Maßnahmen zu ergreifen. Egal, ob du an die Führungsebene berichtest oder die tägliche Datenverwaltung leitest, dieses Dashboard stellt sicher, dass du schnell auf relevante Informationen zugreifen, Maßnahmen priorisieren und den Wert der Sicherheits- und Compliance-Strategie deines Unternehmens demonstrieren kannst.

## Zu den verwandten domainspezifischen Dashboards

Zusätzlich zum Dashboard von Enterprise Guard können Admins eine Reihe von domainspezifischen Dashboards erkunden, die darauf ausgelegt sind, tiefere Einblicke und Kontrolle in wesentlichen Governance-Bereichen zu bieten. Jedes dieser Dashboards ermöglicht fokussierte Entscheidungsfindung in seinem jeweiligen Bereich, während es die Ausrichtung mit dem umfassenderen Enterprise Guard-Framework beibehält. Dazu gehören:

- **Datenerkennungs-Dashboard:** Erkennt und analysiert, wo sich sensible Informationen auf deinen Boards befinden.
- **Klassifizierungs-Dashboard:** Verfolge und verwalte die Klassifizierungsabdeckung und Sensibilitätslabel auf Board-Ebene.
- **Content-Lifecycle-Dashboard:** Überwache Aufbewahrungsrichtlinien und automatisiere Lifecycle-Management-Aktionen.
- **eDiscovery-Dashboard:** Verschaffe dir einen Überblick über Aufbewahrungsfristen und optimiere die eDiscovery-Vorbereitungs-Workflows.

## Dashboard-Kennzahlen verstehen

Enterprise Guard-Dashboards umfassen zwei Arten von Kennzahlen: aktuelle Kennzahlen und verlaufsbezogene Kennzahlen. Um Klarheit und Konsistenz zu gewährleisten, ist jede im Enterprise Guard-Dashboard präsentierte Kennzahl in der [Dokumentation zu den Enterprise Guard-Dashboard-Kennzahlen](07-enterprise-guard-dashboard-metrics-reference.md) definiert.

:::note
Hinweise zu den Kennzahlen:

- Alle Kennzahlen in Enterprise Guard schließen Boards von Teams im Papierkorb und Boards unter Aufbewahrungsfrist aus.
- Alle Klassifizierungs-Kennzahlen schließen Vorlagen und Boards im Papierkorb aus.
:::

## Fehler, leere Zustände und verlaufsbezogene Änderungen verstehen

Zum Verständnis der Kennzahlen auf dem Enterprise Guard-Dashboard ist es unerlässlich, zu wissen, wie leere Zustände und Fehlermeldungen zu interpretieren sind.

### Verstehen, wie sich bisherige Daten bei Änderung der Einstellungen verhalten

Wenn ein Feature, wie z. B. Klassifizierung, nach der Datensammlung deaktiviert wird, zeigen die bisherigen Kennzahlen weiterhin Werte aus dem aktiven Zeitraum an. Zum Beispiel, wenn du die Klassifizierung im Mai deaktivierst und die Klassifizierung im April aktiv war, wobei 20 Boards klassifiziert wurden:

- April-Werte werden weiterhin auf dem Dashboard angezeigt.
- Die Mai-Grafik wird **keine Daten verfügbar**, da die Datenerfassung gestoppt wurde.
