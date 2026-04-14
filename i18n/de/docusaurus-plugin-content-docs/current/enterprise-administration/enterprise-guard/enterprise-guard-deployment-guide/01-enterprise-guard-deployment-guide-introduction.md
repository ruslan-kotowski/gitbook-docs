---
title: "Enterprise Guard Bereitstellungsleitfaden Einf\xFChrung"
article_id: 17120515162386
translation_id: 17120515162386
locale: de
sidebar_position: 0
created_at: '2024-02-19T09:17:20Z'
updated_at: '2025-11-25T15:40:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Dieses Dokument führt dich durch den Einsatz des fortschrittlichen Sicherheitsprodukts Enterprise Guard von Miro, indem es die besten Praktiken für die Konfiguration und die Aktivierung durch den Nutzer beschreibt. Wenn du Fragen zum Inhalt dieses Leitfadens hast, wende dich bitte an dein Miro-Konto-Team.

## Wie du diesen Leitfaden verwendest

- Navigiere mit der Gliederung auf der linken Seite deines Bildschirms von Abschnitt zu Abschnitt
- Benutze den Leitfaden in Verbindung mit der Dokumentation der Funktionen, die überall verlinkt sind
- Passen Sie die Vorlagen an, um Ihren Nutzern Zeit zu sparen.

## Leitfaden Gliederung

- [Teil 1 | Admin-Rollen konfigurieren](02-enterprise-guard-deployment-guide-part-1-configure-admin-roles.md)
- [Teil 2 | Datensicherheit einführen](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md)
- [Teil 3 | Verwalten des Content Lifecycle](04-enterprise-guard-deployment-guide-part-3-manage-content-lifecycle.md)

## Warum du Enterprise Guard brauchst

Miro ist der unternehmenstaugliche Online-Arbeitsbereich für Innovation, der die Arbeit von verteilten Teams jeder Größe verändert.

Die strategische Arbeit in Miro hat stark zugenommen, und mit diesem Wachstum gibt es noch mehr Inhalte, die geschützt und verwaltet werden müssen.

Sensible Daten tauchen dort auf, wo die Kunden sie am wenigsten erwarten. Anhand einer Stichprobe von 100 Opt-in-Unternehmenskunden haben wir festgestellt, dass 62 % von ihnen Boards mit sensiblen Daten wie persönlichen Daten, Gesundheitsinformationen und Kreditkarteninformationen hatten. Dieses Risiko wird immer größer, da die Zahl der Boards für unsere Unternehmenskunden jedes Jahr um 250 % steigt.

Dieser Zuwachs an Inhalten macht es noch schwieriger, Risiken mit herkömmlichen Tools zu managen oder sich darauf zu verlassen, dass sich die Mitarbeiter an die Richtlinien des Unternehmens halten.

Enterprise Guard ist das erweiterte Add-on für Miro zur Datensicherheit und Datenverwaltung. Unternehmen können sensible Inhalte finden und sichern und Content Lifecycle Management betreiben - automatisch und in großem Umfang.

## Wir stellen vor: Enterprise Guard: eine umfassende Sicherheits- und Governance-Lösung für Miro

Miro hat diese Herausforderungen erkannt und deshalb **Enterprise Guard**, ein erweitertes Sicherheits- und Governance-Add-on, eingeführt. Enterprise Guard bietet eine Reihe von Funktionen, die es Organisationen ermöglichen, sensible Inhalte auf allen Miro-Boards effektiv zu identifizieren, zu klassifizieren, zu sichern und zu verwalten. Diese Lösung ist darauf zugeschnitten, die Einhaltung von Vorschriften und einen robusten Datenschutz im großen Maßstab zu gewährleisten.

Mit der Integration von Enterprise Guard in das Enterprise-Ökosystem von Miro steht Unternehmen jetzt ein leistungsstärkeres, automatisiertes und umfassenderes Sicherheitsframework zur Verfügung. Bei diesem Add-on geht es nicht nur um den Schutz von Daten. Es geht vor allem darum, Unternehmen in die Lage zu versetzen, auf sichere Weise – und ohne Behinderung des üblichen Geschäftsablaufs – im Team innovativ zu agieren,

## Enterprise Guard General Availability Release: Die wichtigsten Funktionen

![Die wichtigsten Funktionen des Enterprise Guard General Availability Release](images/26240574136338_Enterprise-Guard-Data-Security.png)

- **Datenerkennung:** Enterprise Guard ermöglicht einen proaktiven, gründlichen Datenerkennungsprozess. Dies ist entscheidend für die Identifizierung sensibler Daten wie Kreditkartennummern, Sozialversicherungsnummern und andere kritische Informationen, die auf den verschiedenen Miro-Boards zu finden sind. Mit dieser wichtigen, proaktiven Strategie lassen sich potenzielle Schwachstellen aufdecken und mindern, um Datenschutzverletzungen zu verhindern und die Compliance zu gewährleisten.
- **eDiscovery**. Ermöglicht die sichere Aufbewahrung, Verfolgung und den Export von Board-Daten, um rechtliche, Compliance- und Sicherheitsanforderungen zu erfüllen. Die eDiscovery-Funktion in Enterprise Guard unterstützt Unternehmen bei der Einhaltung gesetzlicher Vorschriften durch [Legal Holds](../../canvas-25-admin-features/ediscovery/02-legal-hold-overview.md), [Content Logs](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md) und [Board-Exportfunktionen](../../canvas-25-admin-features/ediscovery/13-board-export-api-overview.md).

  Legal Holds verhindern das dauerhafte Löschen von Inhalten, die für Ermittlungen oder rechtliche Angelegenheiten relevant sind, indem alle Boards, mit denen ein Nutzer interagiert, erhalten bleiben - einschließlich aller ihrer Versionen. Inhaltsprotokolle liefern detaillierte Aufzeichnungen der Aktivitäten von Nutzern, die exportiert und in externe Tools für Audits oder rechtliche Prüfungen integriert werden können. Mit den eDiscovery-APIs können Unternehmenskunden auch Board-Daten in großem Umfang exportieren und so sicherstellen, dass wichtige Informationen für rechtliche und Compliance-Workflows zugänglich sind.
- **Automatische Klassifizierung** Lege Kriterien fest, anhand derer Miro deine Boards automatisch nach sensiblen Inhalten klassifizieren kann.
- ****Intelligente Vorgaben:**** Setze Sicherheitsregeln in Echtzeit durch und schränke ein, was Nutzer mit einem Board machen können, z. B. die Replikation von Board-Inhalten und das Freigeben von Inhalten auf verschiedenen Ebenen (öffentlich, Team, Organisation), basierend auf der manuellen oder automatischen Klassifizierung des Boards. Dies gewährleistet dauerhaften Datenschutz und Compliance, ohne den Geschäftsbetrieb zu behindern.
- **Papierkorbrichtlinie:** Die Papierkorbrichtlinie von Enterprise Guard ermöglicht eine bessere Kontrolle über das Löschen und Wiederherstellen von Miro-Boards. Die Einrichtung automatischer Löschfristen (30, 60, 90, 180 Tage) ermöglicht es Organisationen, regulatorische Anforderungen zu erfüllen und dabei die richtige Balance zwischen Datenaufbewahrung und Risikominimierung für das Unternehmen zu finden.
- **Aufbewahrung:** Gewährleiste Datenschutz und Compliance, indem du es Admins ermöglichst, Richtlinien zu definieren, zu bearbeiten und zu löschen, die auf die Bedürfnisse eures Unternehmens zugeschnitten sind. Diese Richtlinien spielen eine entscheidende Rolle beim Schutz von Miro-Boards in der Organisation, denn sie ermöglichen die Aufbewahrung bestimmter Boards für einen festgelegten Zeitraum. Die Aufbewahrung stellt sicher, dass Miro-Boards vor dem Ablauf der Aufbewahrungsfrist nicht versehentlich oder absichtlich gelöscht werden. Mithilfe von Aufbewahrungsrichtlinien können Organisationen den Datenschutz, die Compliance und die Aufbewahrung geschäftskritischer Informationen sicherstellen.
- Löschung Aktiviere die automatische Bereinigung von Boards, indem du sie auf der Grundlage von Richtlinien zur Aufbewahrung archivierst und löschst. [Die Löschung](../../canvas-25-admin-features/content-lifecycle-management/03-disposition-overview.md) stellt sicher, dass Boards nur so lange wie nötig aufbewahrt werden und nach einer gewissen Zeit der Inaktivität automatisch in den Papierkorb verschoben werden. Die Standardeinstellungen für den Papierkorb legen fest, wer die Boards wiederherstellen kann und wann sie endgültig gelöscht werden - und unterstützen so Compliance, betriebliche Effizienz und Datensicherheit.
- ****Verwaltung von Verschlüsselungsschlüsseln****:**** Bietet eine zentrale Kontrolle über die Verschlüsselungsschlüssel, so dass Unternehmen die Aktivitäten im Zusammenhang mit den Schlüsseln überwachen und den Zugang bei Bedarf sperren können. Die gewährleistet eine zusätzliche Ebene der Datensicherheit.
