---
title: "Planer f\xFCr Jira"
article_id: 10648975837970
translation_id: 12813850994450
locale: de
sidebar_position: 22
created_at: '2023-08-01T10:07:40Z'
updated_at: '2026-02-09T13:21:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Mit dem Planer für Jira können Moderatoren und Teams Planungsevents auf einem Miro-Board durchführen und gleichzeitig Aktualisierungen in Echtzeit mit ihrem Jira-Board synchronisieren – das spart Stunden an manueller Arbeit.

> **Erhältlich für:** Business-Preisplan, Enterprise-Preisplan

Bei Planungsevents auf Team- oder Unternehmensebene, wie beispielsweise Program Increments (PI), Big Room, Roadmapping und Sprints, tauschen sich die Entwicklungsteams aus und sprechen sich untereinander ab.

:::tip
Der Planer ist jetzt für [Azure DevOps](https://help.miro.com/hc/articles/15280547945618) verfügbar.
:::

## Wie man einen Planer für Jira erstellt

1. Gehe zur [Erstellungssymbolleiste](https://help.miro.com/hc/articles/360017730553-Toolbars) auf der linken Seite des Boards.
2. Klicke auf **Weitere Apps** (**+**) und suche nach ‚Planner‘.
3. Klicke auf **Planer**, um die App zu starten.
4. Ein Cursor erscheint auf dem Board. Klicke irgendwo, um einen leeren Planer zu platzieren.
5. Klicke auf das **Jira-Board**-Dropdown und wähle ein Board aus, das mit dem Planer verbunden werden soll. Wenn du dein Jira-Konto noch nicht in Miro autorisiert hast, wirst du aufgefordert, dich anzumelden.
6. Das erste **Spalten**-Feld ist dein *Spaltentyp*. Nachdem du das Jira-Board ausgewählt hast, wird der Spaltentyp standardmäßig auf **Status** eingestellt und es werden bis zu 3 Spalten angezeigt. Klicke auf das erste **Spalten**-Feld, um einen anderen Spaltentyp aus dem Dropdown-Menü auszuwählen (du kannst Sprint, Status, Priorität, Fehlerbehebung von Versionen, Komponenten oder ein benutzerdefiniertes Feld auswählen).
7. Verwende das zweite Feld **Spalten**, um deinen Planer zu verfeinern. Wenn du beispielsweise „Sprint“ als Spaltenfeld festgelegt hast, kannst du dann auswählen, welche Sprints angezeigt werden sollen.
8. Füge neben Spalten deinem Planer auch **Swimlanes** hinzu, um Aufgaben auch über ein zweites Jira-Feld zu koordinieren (du kannst Sprint, Status, Priorität, Fehlerbehebung von Versionen, einzelne Komponenten oder ein benutzerdefiniertes Feld auswählen).

:::note
Der Planer unterstützt derzeit nur ein Jira-Board. Du kannst jedoch mehrere Planer auf einem einzigen Miro-Board erstellen.
:::

![Creating-a-planner-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696033042_Creating-a-planner-widget.gif)*Ein Planer erstellen*

## So arbeitest du mit dem Planer

Ziehe Jira-Karten über die Spalten, um sie zu aktualisieren. Wenn du zum Beispiel eine Jira-Karte aus dem Backlog auf einen Sprint im Planer ziehst, wird sie sowohl in Miro als auch in Jira aktualisiert.

![Dragging-stories-between-columns-planning-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696028306_Dragging-stories-between-columns-planning-widget.gif)*Jira-Karten zwischen Sprints verschieben*

Wähle ein Feld für **Swimlanes**, um deine Arbeit sowohl in Zeilen als auch in Spalten zu unterteilen. Wenn du Karten zwischen Swimlanes verschiebst, werden sowohl die Felder *Spalte* als auch *Swimlane* des Jira-Vorgangs aktualisiert.

![Choosing-a-swimlane.png](../../../../../../docs/integrations-apps/atlassian/images/21017725756946_Choosing-a-swimlane.png)*Auswahl eines Felds für Swimlanes*

Standardmäßig zeigt der Planer alle Vorgänge in deinem Backlog an. Um dich auf den aktuellen Sprint zu konzentrieren, wähle oben rechts das Filter-Symbol und setze ein Häkchen bei **Sprint**. Dann wähle den **Sprint**-Filter und aktiviere **Filter nach aktivem Sprint**. Wähle **Anwenden**, um deinen Sprint-Filter anzuwenden.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Vorgänge nach aktivem Sprint filtern.*

Du kannst auch das Dropdown-Menü **Vorgangstyp** verwenden und auswählen, welche Vorgangstypen in deinem Planer angezeigt werden sollen. Du kannst zum Beispiel nur nach der Story filtern.

![Filtering-by-issue-type-planning-widget.png](../../../../../../docs/integrations-apps/atlassian/images/21017725749138_Filtering-by-issue-type-planning-widget.png)*Nach Vorgangstyp filtern*

Teilnehmer können Jira-Karten kommentieren, um laufende Diskussionen und Anmerkungen zu verfolgen.

![Commenting_on_a_story.png](../../../../../../docs/integrations-apps/atlassian/images/21017696024594_Commenting%20on%20a%20story.png)*Eine Jira-Karte im Planer kommentieren*

:::note
Im Planer können keine Miro-Karten, Notizen und andere Objekte platziert werden.
:::

## Kapazität und Auslastung

Die visuelle Darstellung aller „Story Points“ in übersichtlichen Spalten hilft dir, in deinen Sprints und während der PI-Planungen fundierte Entscheidungen zu treffen. Dadurch steigerst du die Effizienz deines Teams und sorgst für eine optimale Arbeitsverteilung.

### Das Feld „Story Points“ in Jira-Karten aktivieren

1. Gehe zur [Erstellungssymbolleiste](https://help.miro.com/hc/articles/360017730553-Toolbars#Creation_toolbar) auf der linken Seite deines Boards.
2. Klicke auf **Mehr Apps** (**+**) und suche nach „Jira-Karten“.
3. Klicke auf **Jira-Karten**, um die App zu starten.
4. Klicke auf **Karten konfigurieren**.
5. Scrolle nach unten und schalte die **Story Points** ein.

![Enabling-Story-Points-for-Jira-Cards.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696030866_Enabling-Story-Points-for-Jira-Cards.gif)
*Story Points für Jira-Karten aktivieren*

### Kapazität und Auslastung verwenden

Sobald du Story Points aktivierst, kannst du einen neuen Planer erstellen oder ein Board mit einem vorhandenen Planer aktualisieren. Solange mindestens einem Vorgang auf dem Board Story Points zugewiesen sind, siehst du sofort die Felder **Kapazität** und **Auslastung** oben in jeder Spalte in deinem Planer.

![Balancing-Capacity-and-Load.gif](../../../../../../docs/integrations-apps/atlassian/images/21017725755794_Balancing-Capacity-and-Load.gif)*Kapazität und Auslastung in Einklang bringen*

### Was bedeuten Kapazität und Auslastung?

**Kapazität**: Gib die Kapazität für jede Spalte in deinem Planer manuell ein. Wenn die Kapazität geringer als die Auslastung ist, wird die Spalte rot und signalisiert dir, dass du die Kapazität deines Teams überschritten hast. Dieses visuelle Signal fordert dich dazu auf, die Vorgänge neu zuzuweisen, um eine ausgeglichene Arbeitsauslastung zu gewährleisten.

**Auslastung**: Dies ist die Summe der Story Points für alle Karten in einer bestimmten Spalte. Karten ohne Story Points werden in dieser Berechnung als 0 gewertet.

## Jira-Konfiguration

Um den Planer einzurichten, wähle zunächst ein Jira-Board aus, aus dem du Vorgänge importieren kannst. Diese können entweder von einem Jira-Scrum-Board oder einem Kanban-Board kommen.

Wenn du einen Planer erstellst, kannst du wählen, welches Jira-Feld du für deine Spalten und Zeilen (Swimlanes) verwenden möchtest, einschließlich:

- Sprints
- Status
- Fehlerbehebung in Version
- Komponente
- Priorität
- Bearbeitende Person
- Jedes benutzerdefinierte Feld mit einer Dropdown-Auswahl für einen Wert
- Jedes benutzerdefinierte Feld mit einer Dropdown-Auswahl für mehrere Werte

Wir unterstützen derzeit keine anderen Jira-Felder oder datumsbezogenen Felder.

Die Option „Sprint“ wird nur angezeigt, wenn das Feld „Sprint“ auf dem Bildschirm für „Vorgang bearbeiten“ in Jira verfügbar ist. Dies ist in der Regel für Jira Server/Data Center vorkonfiguriert, aber häufig ist es für die Cloud erforderlich, dass das Feld „Sprint“ manuell hinzugefügt wird. Lies mehr darüber, [wie man Vorgang-Bildschirme konfiguriert](https://support.atlassian.com/jira-cloud-administration/docs/configure-issue-screens/).

:::note
Geschlossene Sprints können im Planer nicht angezeigt werden.
:::

### So erstellst du einen Planer mit einem benutzerdefinierten JQL

Um einen Planer mit einem benutzerdefinierten JQL zu erstellen, erstelle zuerst ein Jira-Board mit deiner JQL-Abfrage. Nachdem das Jira-Board erstellt wurde, folge den Anweisungen oben zur Erstellung eines Planers. Wenn du zu Schritt 5 kommst, denke daran, das Jira-Board auszuwählen, das du mit deiner benutzerdefinierten JQL-Abfrage erstellt hast.

## Planer synchronisieren

### Von Miro zu Jira

Wenn du eine Karte zwischen benutzerdefinierten Feldern in Miro verschiebst, wird Jira automatisch aktualisiert. Dies kann einige Sekunden dauern.

### Von Jira zu Miro

Wenn du Änderungen an einem Sprint in Jira vornehmen, siehst du eine **Updates verfügbar**-Benachrichtigung im Planer-Kontextmenü. Dies kann einige Sekunden dauern, nachdem du die Änderungen in Jira vorgenommen hast.

Klicke auf den Planer, um das Kontextmenü zu öffnen, und klicke auf das **Mit Jira synchronisieren**-Symbol, um die neuesten Änderungen zu synchronisieren.

![Sync-planning-widget-with-jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017696029970_Sync-planning-widget-with-jira.png)*Updates von Jira mit Miro synchronisieren*

## Darstellung von Abhängigkeiten

Teilnehmer können die Abhängigkeiten zwischen den Aufgaben im Planer visuell darstellen. Erfahren Sie mehr über [Dependencies for Jira](https://help.miro.com/hc/articles/10649083010834).
