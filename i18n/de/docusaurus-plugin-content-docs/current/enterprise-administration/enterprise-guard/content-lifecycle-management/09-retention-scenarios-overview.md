---
title: "Szenarien f\xFCr die Aufbewahrung"
article_id: 19205103343506
translation_id: 19205103343506
locale: de
sidebar_position: 9
created_at: '2024-05-28T17:58:22Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## Board wird während des Aufbewahrungszeitraums in den Papierkorb verschoben

**Aufbewahrungsrichtlinien haben Vorrang vor Papierkorb-Richtlinien.** Wenn ein Board, das unter Aufbewahrung steht, am Anfang oder der Mitte seiner Aufbewahrungsfrist in den Papierkorb verschoben wird, verbleibt das Board für die in der Papierkorb-Richtlinie festgelegte Dauer (standardmäßig 90 Tage) im Papierkorb. Nach dieser Zeit erscheint das Board nicht mehr im Papierkorb. Das Board bleibt jedoch bestehen und wird bis zum Ende der Aufbewahrungsfrist aufbewahrt. Danach wird das Board automatisch gelöscht. Abbildung 1 veranschaulicht dieses Szenario.

![Figure 1: Board is trashed during retention period](images/19205142065810_board_trashed_during_retention_period.png)*Abbildung 1: Board wird während der Aufbewahrungsfrist in den Papierkorb verschoben*

## Board wird nach Ablauf der Aufbewahrungsfrist in den Papierkorb verschoben

**Die Papierkorb-Richtlinie bleibt auch nach Ablauf der Aufbewahrungsfrist aktiv.** Wenn ein Board, das unter Aufbewahrung steht, nach Ablauf der Aufbewahrungsfrist in den Papierkorb verschoben wird, bleibt das Board für die in der Papierkorb-Richtlinie festgelegte Dauer (standardmäßig 90 Tage) im Papierkorb. Nach dieser Zeit erscheint das Board nicht mehr im Papierkorb. Nach Ablauf der Aufbewahrungsfrist kann das Board manuell endgültig gelöscht werden und wird nach Ablauf der Papierkorb-Richtlinie automatisch entsorgt. Abbildung 2 veranschaulicht dieses Szenario.

![Abbildung 2: Board wird nach Ablauf der Aufbewahrungsfrist in den Papierkorb verschoben](images/19205142072338_board_trashed_when_retention_period_is_ending.png)*Abbildung 2: Board wird nach Ablauf der Aufbewahrungsfrist in den Papierkorb verschoben*

## Team wird während der Aufbewahrungsfrist in den Papierkorb verschoben

**Wenn ein Team gelöscht wird, werden alle Boards, die zu einem Team gehören, dauerhaft gelöscht.** Wenn ein Team in den Papierkorb verschoben wird, werden alle Boards, die zu diesem Team gehören, nach 90 Tagen dauerhaft gelöscht, auch Boards, für die eine Aufbewahrungsrichtlinie gilt. Wenn ein Team im Papierkorb manuell von einem Admin dauerhaft gelöscht wird, gilt dasselbe: Alle Boards, die zu diesem Team gehören, werden dauerhaft gelöscht, auch wenn diese Boards unter Aufbewahrung stehen. Abbildung 3 veranschaulicht dieses Szenario.

![Figure 3: Team wird während der Aufbewahrungsfrist in den Papierkorb verschoben](images/19205142077458_team_trashed_during_retention_period.png)*Abbildung 3: Team wird während der Aufbewahrungsfrist in den Papierkorb verschoben*
