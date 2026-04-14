---
title: Referenz der Kennzahlen des Enterprise Guard Dashboards
article_id: 26718144750610
translation_id: 26718144750610
locale: de
sidebar_position: 5
created_at: '2025-05-15T00:17:54Z'
updated_at: '2025-07-22T20:38:23Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: admin-analytics
---

:::note
Hinweise zu Kennzahlen:

- Alle Kennzahlen in Enterprise Guard schließen Boards von Teams im Papierkorb aus.
- Alle Klassifizierungskennzahlen schließen Vorlagen und Boards im Papierkorb aus.
:::

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| **Titel** | **Beschreibung** | **Domain** | **Erscheint im Übersichts-Dashboard** | **Hat bisherige Kennzahl** |
| Gesamtanzahl der klassifizierten Boards | Anzahl der Boards, denen ein Klassifizierungslabel zugewiesen ist | Klassifizierung | ✅ | ❌ |
| Anzahl der Boards pro Klassifizierung | Anzahl der Boards pro Klassifizierungslabel (Labelname) | Klassifizierung | ✅ | ❌ |
| Anzahl der nicht klassifizierten Boards | Anzahl der Boards, denen kein Klassifizierungslabel zugewiesen ist | Klassifizierung | ✅ | ✅ |
| Anzahl der manuell klassifizierten Boards | Anzahl der Boards mit einem manuell zugewiesenen Klassifizierungslabel (nicht durch automatische Klassifizierung) | Klassifizierung | ❌ | ✅ |
| Anzahl der automatisch klassifizierten Boards | Anzahl der Boards, die ein automatisch zugewiesenes Klassifizierungslabel durch die automatische Klassifizierung haben | Klassifizierung | ❌ | ✅ |
| Anzahl der sensiblen Boards | Anzahl der Boards, denen mindestens ein integriertes Label, ein Suchbegriff-Label oder ein Datenschutzlabel zugewiesen ist | Datenerkennung | ✅ | ❌ |
| Anzahl der Boards mit geschäftskritischen Elementen | Anzahl der Boards, denen mindestens ein integriertes Label oder ein Suchbegriff-Label zugewiesen wurde | Datenerkennung | ✅ | ✅ |
| Anzahl der Boards mit datenschutzrelevanten sensiblen Inhalten | Anzahl der Boards, denen mindestens ein Datenschutzlabel zugewiesen wurde | Datenerkennung | ✅ | ✅ |
| Anzahl der Boards, denen ein Label zugewiesen ist, pro Label | Anzahl der Boards für jedes Label (integriert, Suchbegriff oder Datenschutz) | Datenerkennung | ❌ | ❌ |
| Anzahl der aktivierten datenschutzrelevanten Labels | Anzahl aktivierter datenschutzrelevanter Labels | Datenerkennung | ❌ | ❌ |
| Anzahl der aktivierten Suchbegriff-Labels | Anzahl der aktivierten Suchbegriff-Labels | Datenerkennung | ❌ | ❌ |
| Anzahl der aktivierten geschäftskritischen Labels | Anzahl aktivierter geschäftskritischer Labels | Datenerkennung | ❌ | ❌ |
| Gesamtanzahl der Boards | Gesamtzahl der Boards in allen Stadien des Lebenszyklus (aktiv, Papierkorb, in der Aufbewahrung) | Inhaltslebenszyklus-Management | ✅ | ❌ |
| Anzahl aktiver Boards. Beachte, dass dies NICHT die Aktivität der Boards ist, sondern Boards, die sich im aktiven Lebenszyklusstadium befinden. | Gesamtanzahl der Boards im aktiven Lebenszyklusstadium | Inhaltslebenszyklus-Management | ✅ | ✅ |
| Anzahl der Boards im Papierkorb | Gesamtanzahl der Boards im Lebenszyklusstadium „im Papierkorb“ | Inhaltslebenszyklus-Management | ✅ | ✅ |
| Anzahl der Boards in Aufbewahrung | Gesamtzahl der Boards im Lebenszyklusstadium „in Aufbewahrung“ | Inhaltslebenszyklus-Management | ✅ | ✅ |
| Anzahl der Boards zur Aufbewahrung | Gesamtanzahl der Boards, denen mindestens eine nicht abgelaufene Aufbewahrungsrichtlinie zugewiesen ist | Content Lifecycle Management | ❌ | ✅ |
| Anzahl der Boards zur Löschung | Gesamtanzahl der Boards, denen mindestens eine nicht abgelaufene Löschungsrichtlinie zugewiesen ist | Inhaltslebenszyklus-Management | ❌ | ❌ |
| Anzahl der Boards gemäß einer Aufbewahrungsrichtlinie, gruppiert nach Richtlinien | Anzahl der Boards in einem beliebigen Lebenszyklusstadium, denen mindestens eine Aufbewahrungsrichtlinie zugewiesen ist | Inhaltslebenszyklus-Management | ✅ | ❌ |
| Anzahl der Boards gemäß einer Löschungsrichtlinie gruppiert nach Richtlinien | Anzahl der Boards in jedem Lebenszyklusstadium, denen mindestens eine Löschungsrichtlinie zugewiesen wurde | Inhaltslebenszyklus-Management | ✅ | ❌ |
| Anzahl der erstellten Boards an diesem Tag/in dieser Woche/in diesem Monat | Anzahl der in dieser Woche erstellten Boards | Inhaltslebenszyklus-Management | ❌ | ✅ |
| Anzahl der Boards, die an diesem Tag/in dieser Woche/in diesem Monat gelöscht (in den Papierkorb verschoben) wurden | Anzahl der in dieser Woche gelöschten (in den Papierkorb verschobenen) Boards | Inhaltslebenszyklus-Management | ❌ | ✅ |
| Anzahl der Boards unter Löschungsrichtlinien, gruppiert nach effektivem Löschungsrichtliniendatum pro Monat |  | Inhaltslebenszyklus-Management | ❌ | ❌ |
| Anzahl der Untersuchungen | Gesamtanzahl der Untersuchungen | eDiscovery | ✅ | ❌ |
| Anzahl der Aufbewahrungsfristen | Gesamtanzahl der Aufbewahrungsfristen | eDiscovery | ✅ | ❌ |
| Anzahl der Aufbewahrungsfristen für eine bestimmte Untersuchung | Gesamtanzahl der Aufbewahrungsfristen für eine bestimmte Untersuchung | eDiscovery | ❌ | ❌ |
| Anzahl der Boards unter Aufbewahrungsfrist | Gesamtzahl der Boards, die unter Aufbewahrungsfristen stehen, über alle Aufbewahrungsfristen hinweg | eDiscovery | ❌ | ❌ |
| Nutzer unter Aufbewahrungsfrist und die Gesamtanzahl ihrer Boards | Zeigt Nutzer unter Aufbewahrungsfrist und die Gesamtanzahl ihrer Boards an | eDiscovery | ❌ | ❌ |
