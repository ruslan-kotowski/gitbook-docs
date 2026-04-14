---
title: "Abh\xE4ngigkeiten f\xFCr Jira"
article_id: 10649083010834
translation_id: 10649083010834
locale: de
sidebar_position: 7
created_at: '2023-03-22T10:22:08Z'
updated_at: '2025-11-25T16:22:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

Ordne bestehende Abhängigkeiten zu oder erstelle neue zwischen Jira-Karten auf deinem [Planer](../../integrations-apps/atlassian/21-planner-for-jira.md) oder an einer beliebigen Stelle auf deinem Miro-Board, und sie werden sofort in Jira synchronisiert. Mit der Abhängigkeiten-App kannst du Abhängigkeiten zwischen Teams in Echtzeit während der Planungsübungen identifizieren, visualisieren, diskutieren und aufzeichnen.

> ****💡**** Diese Funktion ist jetzt für [Azure DevOps](08-dependencies-for-azure-devops.md) verfügbar.

> **Erhältlich für:** Business-Preisplan, Enterprise-Preisplan
>
> **Verfügbar mit:** Desktop-Browser, Desktop-App

## So funktionieren Abhängigkeiten

Abhängigkeiten erscheinen als Verbindungslinien und zeigen die Beziehungen zwischen Jira-Karten an.

Sie sind nur sichtbar, wenn du Abhängigkeiten auf dem Board öffnest. Die Teilnehmer können verschiedene Abhängigkeitstypen filtern, um Blockierungen und Beziehungen zu diskutieren.

![Dependencies-app.png](../../../../../../docs/using-miro/facilitation-tools/images/13244544218258_Dependencies-app.png)
*Abhängigkeiten zwischen Jira-Karten auf einem Planer-Widget abgebildet*

## So erstellst du eine neue Abhängigkeit

1. Gehe zur Erstellungssymbolleiste auf der linken Seite des Boards.
2. Klicke auf das **Symbol für Abhängigkeiten**. Wenn das Symbol für Abhängigkeiten sich nicht bereits in deiner Erstellungssymbolleiste befindet, musst du es unter **Tools, Medien und Integrationen** (**+**) hinzufügen.
3. Das Feld für Abhängigkeiten wird geöffnet.
4. Klicke auf **Neue Abhängigkeit**.
5. Klicke auf **Erste Karte** und wähle einen Jira-Vorgang aus dem Dropdown-Menü oder über die Suche aus.
6. Wähle den **Abhängigkeitstyp** basierend auf den in deiner Jira-Instanz verfügbaren Optionen aus (z. B. blockiert, klont, dupliziert oder bezieht sich auf).
7. Klicke auf **Zweite Karte** und wähle einen Jira-Vorgang aus dem Dropdown-Menü oder über die Suche aus.
8. Klicke auf **Entwurf speichern**, oder **In Jira speichern**direkt.

:::tip
Entwurfsabhängigkeiten werden nur in Miro gespeichert. Du kannst Entwürfe von Abhängigkeiten erstellen, um sie den anderen Teilnehmenden und Teams während der Planung vorzuschlagen. Sobald sie geprüft und diskutiert wurden, kannst du sie entweder in Jira speichern oder löschen.
:::

![dependencies-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537435953426_dependencies-entry-point.png)
*Erstellen einer neuen Abhängigkeit und Speichern in Jira*

## So siehst du Abhängigkeiten an und filterst sie

1. Gehe zur Erstellungssymbolleiste auf der linken Seite des Boards.
2. Klicke auf das **Symbol für Abhängigkeiten**. Wenn das Symbol für Abhängigkeiten noch nicht in deiner Erstellungssymbolleiste ist, musst du es unter **Tools, Medien und Integrationen** (**+**) hinzufügen.
3. Das Abhängigkeiten-Feld wird geöffnet und alle vorhandenen Abhängigkeiten werden als Linien auf dem Board angezeigt.
4. Klicke auf das **Symbol für Filter** oben im Abhängigkeiten-Feld.
5. Verwende die Schalter, um nach **Abhängigkeitstyp** und **Synchronisierungsstatus** zu filtern.
6. Verwende das Dropdown-Menü **Linien anzeigen**, um zu steuern, wann Abhängigkeiten angezeigt werden. Wähle **Immer**, um alle aktiven Abhängigkeiten anzuzeigen. Wähle **Nach Auswahl**, um Abhängigkeiten nur dann zu sehen, wenn du auf eine bestimmte Azure-Karte oder einen Abhängigkeitstyp klickst.

Gepunktete Linien zeigen Entwurfsabhängigkeiten und durchgezogene Linien zeigen Abhängigkeiten, die mit Jira synchronisiert wurden. Die Linienfarbe stellt den Abhängigkeitstyp dar.

![Filtering-dependencies.gif](../../../../../../docs/using-miro/facilitation-tools/images/13245295619730_Filtering-dependencies.gif)
*Filtern der Abhängigkeitsansicht* *im Planer-Widget*

## So kannst du eine Abhängigkeit bearbeiten, speichern oder rückgängig machen

1. Gehe zur Erstellungssymbolleiste auf der linken Seite des Boards.
2. Klicke auf das **Symbol Abhängigkeiten**.
3. Das Abhängigkeitenfeld wird geöffnet.
4. Klicke auf das **Symbol Bearbeiten** neben einer Abhängigkeit.

![The_option_to_edit_a_Dependency.jpg](../../../../../../docs/using-miro/facilitation-tools/images/10866625733778_The%20option%20to%20edit%20a%20Dependency.jpg)
*Bearbeiten einer Abhängigkeit*

Du kannst die **erste Karte** und die **zweite Karte** einer Abhängigkeit sowie den **Abhängigkeitstyp ändern.**

*![Editing_a_dependency.gif](../../../../../../docs/using-miro/facilitation-tools/images/10866808392722_Editing%20a%20dependency.gif)**Ändern der ersten Karte und des Abhängigkeitstyps*

Klicke auf **In Jira speichern**, um einen Entwurf der Abhängigkeit in Jira zu speichern und zu synchronisieren.

![Save_to_Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/10868740630034_Save%20to%20Jira.png)
*Speichern eines Entwurfs der Abhängigkeit in Jira*

Klicke auf **Zum Entwurf zurückkehren**, um eine synchronisierte Abhängigkeit wieder in den Entwurf zurückzusetzen.

![Revert_to_draft.png](../../../../../../docs/using-miro/facilitation-tools/images/10868741500690_Revert%20to%20draft.png)
*Eine in Jira synchronisierte Abhängigkeit wieder in den Entwurf zurücksetzen*

Klicke auf das **Papierkorb**-Symbol, um eine Abhängigkeit zu löschen.
![Delete_dependency.png](../../../../../../docs/using-miro/facilitation-tools/images/10868804195986_Delete%20dependency.png)*Eine Abhängigkeit löschen*
