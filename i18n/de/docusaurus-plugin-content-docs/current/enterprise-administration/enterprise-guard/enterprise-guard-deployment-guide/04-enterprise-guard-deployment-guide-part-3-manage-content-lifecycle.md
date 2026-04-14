---
title: 'Enterprise Guard Einführungshandbuch Teil 3: Verwalten des Content Lifecycle'
article_id: 17121851926546
translation_id: 17121851926546
locale: de
sidebar_position: 3
created_at: '2024-02-19T10:01:34Z'
updated_at: '2025-11-25T15:41:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
availability:
  notes: 'Relevante Teams: ** Beispiele für Teams, mit denen du zusammenarbeiten musst,
    um Content Lifecycle-Funktionen zu implementieren, sind GRC (Governance, Risk,
    Compliance), Compliance Management, Legal und/oder Records Management.'
---

## Inhaltslebenszyklus-Management im Überblick

In den meisten Unternehmen wachsen die Inhalte exponentiell, sowohl was das Volumen als auch die Komplexität angeht. Die richtige Verwaltung und Governance von Miro-Boards ist u. a. aus folgenden Gründen wichtig:

- Proaktives Einhalten von branchenspezifischen Vorschriften oder internen Organisationsrichtlinien
- Risikominimierung in Szenarien wie Rechtsstreitigkeiten oder Sicherheitsverletzungen
- Aufrechterhaltung der organisatorischen Effizienz

Wir unterstützen derzeit die folgenden Funktionen:

- [Richtlinien für den Papierkorb](https://help.miro.com/hc/articles/13860817985426-Trash-Policy)
- [Aufbewahrungsrichtlinien](https://help.miro.com/hc/articles/16855776325778-Retention-policies)

## Content Lifecycle Management - Überblick über den Einsatz von Content Lifecycle Management

Während das empfohlene Verfahren von [Teil 2: Deploy Data Security](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md) umfasst die progressive Konfiguration und die Kommunikation mit dem Nutzer, Content Lifecycle Management nicht.

Weder Papierkorb- noch Aufbewahrungsrichtlinien dürften die Aktivitäten der Nutzer in Miro stören und können daher sofort konfiguriert werden.

## Eine globale Richtlinie für die Aufbewahrung einführen

Derzeit wird nur eine globale Richtlinie für die Aufbewahrung von Daten von Enterprise Guard unterstützt. Zusätzliche Konfigurationsmöglichkeiten werden in Zukunft verfügbar sein und mehr Flexibilität bieten. Berücksichtige die gesetzlichen Anforderungen deiner Branche und die Richtlinien deines Unternehmens, um die Dauer deiner globalen Aufbewahrung zu bestimmen.

Da eine größere Granularität nicht möglich ist, kann es von Vorteil sein, deine globale Richtlinie zur Aufbewahrung so zu konfigurieren, dass sie der längsten von deiner Organisation erwarteten Anforderung entspricht. Wenn beispielsweise bestimmte Inhalte in Miro aufgrund einer gesetzlichen Vorschrift 5 Jahre lang aufbewahrt werden müssen, sollte deine globale Richtlinie zur Aufbewahrung auf 5 Jahre festgelegt werden.

Du kannst den Geltungsbereich der Boards, die unter diese Richtlinie zur Aufbewahrung von 5 Jahren fallen, später reduzieren, wenn Miro granularere Geltungsbereiche wie Klassifizierungsstufe oder Team veröffentlicht.

[So konfigurierst du Richtlinien zur Aufbewahrung](https://help.miro.com/hc/articles/16855776325778-Retention-policies)

## Konfiguriere die Richtlinie für den Papierkorb

Miro-Boards werden standardmäßig nach 90 Tagen automatisch und dauerhaft aus dem Papierkorb gelöscht. Du kannst die Standardeinstellung anpassen und Boards innerhalb von 30, 60, 90 oder 180 Tagen automatisch und endgültig aus dem Papierkorb löschen.

Wenn du die Frist für die automatische und dauerhafte Löschung von Boards geändert hast, gilt die aktualisierte Frist nur für Boards, die neu in den Papierkorb verschoben werden. Boards müssen von Board-Eigentümern oder Board-Miteigentümern manuell in den Papierkorb verschoben werden.

Wenn sich ein Board im Papierkorb befindet, die Richtlinie zum Papierkorb aber noch nicht abgelaufen ist, können bestimmte Nutzer die Boards manuell und dauerhaft löschen. Wähle in den Papierkorb-Einstellungen zwischen Board-Eigentümern und Admins, wer das darf.

[So konfigurierst du Richtlinien für den Papierkorb](https://help.miro.com/hc/articles/13860817985426-Trash-settings)

## Aufbewahrung und Papierkorb arbeiten zusammen

Richtlinien zur Aufbewahrung haben Vorrang vor Richtlinien zum Papierkorb und zur manuellen, dauerhaften Löschung. Siehe die Beispiele und das Diagramm unten.

Beispiele:

- Wenn ein Board in den Papierkorb verschoben und vom Board-Eigentümer manuell dauerhaft gelöscht wird, das Board aber unter eine Richtlinie zur Aufbewahrung fällt, bleibt das Board erhalten. Nach Ablauf der Aufbewahrungsfrist wird das Board sofort und endgültig gelöscht.
- Wenn ein Board in den Papierkorb verschoben wird und die dauerhafte Löschfrist endet, das Board aber unter eine Richtlinie zur Aufbewahrung fällt, wird das Board aufbewahrt. Nach Ablauf der Aufbewahrungsfrist wird das Board sofort und endgültig gelöscht.

![Enterprise-Guard-Papierkorb-Policies.pngRückhaltung](images/17121851918994_Enterprise-Guard-Trash-Policies.png)
*und Papierkorb arbeiten zusammen*
