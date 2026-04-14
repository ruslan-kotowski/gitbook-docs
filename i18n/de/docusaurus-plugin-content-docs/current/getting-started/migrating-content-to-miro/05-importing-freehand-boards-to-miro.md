---
title: Importieren von Freehand-Boards in Miro
article_id: 18580556555538
translation_id: 18580556555538
locale: de
sidebar_position: 9
created_at: '2024-04-26T16:34:28Z'
updated_at: '2025-11-25T15:42:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personen: Alle Nutzer mit berechtigtem Preisplan Preispläne: Starter, Business,
    Education, Enterprise Plattformen: Browser, Desktop, Mobilgerät (für den Zugriff
    auf Miro und das Starten des Imports)'
---

Dieser Artikel erklärt, wie du Freehand-Boards in Miro importierst, einschließlich wie du deine Freehand-Boards vorbereitest, sowohl für Einzel- als auch für Massenimporte.

:::note
Änderungen, die du an importierten Inhalten in Miro vornimmst, werden nicht mit den Originalinhalten in Freehand synchronisiert.
:::

:::note
Du kannst nur Freehand-Boards importieren, die unter kostenlosen oder eingeschränkten Lizenzen stehen.
:::

## Ein einzelnes Board von Freehand nach Miro importieren

Du kannst einzelne Freehand-Boards einfach in Miro importieren, indem du sie im `.RTB`-Dateiformat von Miro exportierst. Hier erfährst du, wie es geht:

1. Rufe das Freehand-Board auf, das du in Miro exportieren möchtest.
2. Lade die Datei im .RTB-Format, dem proprietären Format von Miro, direkt von Freehand herunter. Navigiere zum **Tools**-Menü und wähle **Nach Miro-Board exportieren**. Die Datei wird in deinem standardmäßigen Download-Ordner gespeichert. Freehand wird dich benachrichtigen, sobald das Herunterladen abgeschlossen ist.
3. Öffne dein Miro-Dashboard.
4. Klicke im oberen rechten Bereich des Miro-Dashboards auf die Schaltfläche **+ Neu erstellen**, dann auf **Importieren** und anschließend auf **Backup importieren**.
5. Wähle die zuvor heruntergeladene `.RTB`-Datei aus deinem System aus.
6. Alle Inhalte werden jetzt in ein neues Miro Board in einem bearbeitbaren Format importiert.
7. Die meisten Inhalte lassen sich nahtlos migrieren, jedoch können aufgrund unterschiedlicher Stil- und Formatierungsoptionen zwischen Freehand und Miro kleinere Anpassungen erforderlich sein. Weitere Informationen findest du unter Verständnis der Freehand-Objektabbildung in Miro zu möglichen Unterschieden.

## Massenimport mehrerer Dateien von Freehand nach Miro

Zum gleichzeitigen Migrieren mehrerer Freehand-Boards bietet Miro einen Massenimportprozess an. Stelle zuerst sicher, dass deine Freehand-Boards korrekt vorbereitet sind.

**Voraussetzungen: Bereite deine Freehand-Boards für den Massenimport vor**

Befolge diese Schritte in Freehand, um deine Boards vorzubereiten:

1. In Freehand wähle in der Menüleiste auf der linken Seite **Dokumente** aus. Es öffnet sich ein Dropdown-Menü.
2. Wähle **Alle Dokumente** oder **Von mir erstellt** aus und spezifiziere den Zeitraum für die Boards, die du in Miro importieren möchtest.
3. Für jedes Board, das du importieren möchtest, wähle die drei Punkte (**...**) aus und klicke auf **Auswählen**.
4. Wähle im Dialogfeld unten auf deinem Bildschirm **Bewegen** aus.
5. Wähle einen Bereich aus, um deine Boards zu verschieben. Dies führt sie für eine leichtere Verarbeitung durch das Massenimport-Tool zusammen.

   Du hast erfolgreich mehrere Dateien für den Massenimport nach Miro vorbereitet.

Um den Massenimport deiner vorbereiteten Freehand-Boards nach Miro durchzuführen, folge den Anweisungen im folgenden eingebetteten Miro-Board-Leitfaden:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1IT00=/?pres=1&amp;frameId=3458764590689727256&amp;embedId=507813406404&amp;&amp;autoplay=yep" width="100%"></iframe>

:::note
Wichtige Hinweise zum Massenimport:
- Das Freehand-Token, das für die Massenmigration verwendet wird, ist ab dem Datum, an dem Sie es erhalten haben, nur zwei Wochen lang gültig.
- Ab dem 31. Dezember 2024 um 23:59 Uhr MEZ werden Freehand und alle zugehörigen Migrationstoken eingestellt und ungültig gemacht. Nutzer können keine neuen Tokens mehr generieren oder auf Freehand für die Migration zugreifen.
:::

## Best Practices überprüfen

Für eine reibungslose Migrationserfahrung ist es wichtig, die Best Practices und Schlüsselaspekte zu verstehen, wenn du deine Inhalte von Freehand nach Miro überträgst. Bitte überprüfe die detaillierte Anleitung im unten eingebetteten Miro-Board:

<iframe allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen="allowfullscreen" frameborder="0" height="460" scrolling="no" src="https://miro.com/app/embed/uXjVKB1FWSM=/?pres=1&amp;frameId=3458764590691451227&amp;embedId=480338444592&amp;autoplay=yep" width="100%"></iframe>

## Objekt-Mapping in Miro

Diese Tabelle bietet einen umfassenden Vergleich, wie Objekte von Freehand typischerweise in Miro importiert und dargestellt werden, zusammen mit Hinweisen auf eventuelle manuelle Anpassungen:

|  |  |  |
| --- | --- | --- |
| **Freehand** | **Miro** | **Nachbesserungen erforderlich** |
| Boards | Kanban | Keine |
| Karten | Karten | Jira-Karten in Freehand werden als Jira-Karten in Miro importiert. Sie werden jedoch nicht mit der bestehenden Instanz verbunden, da die Nutzer ihre Jira-Konten in Miro neu authentifizieren müssen.    ADO-, Trello- und Asana-Karten werden nicht unterstützt. |
| Mitwirkende und gemeinsame Nutzung | Kann manuell neu erstellt werden | Keine |
| Kommentare | Kann manuell neu erstellt werden | None: keine |
| Konnektoren/Linien | Konnektoren/Linien | Keine |
| Zeichnungen/Diagramme/Formen | Formen, Text und Konnektoren | Keine |
| Dynamische Datentabellen | CSV | Die Inhalte können als .CSV-Datei vom Miro Board heruntergeladen und bearbeitet werden. |
| Einbettungen:    Google und Microsoft Docs, YouTube, Spotify, Loom | Name der Quelle (z. B. Google, YouTube) und die URL für das Einbetten | Wenn Nutzer ein Dokument erneut einbetten möchten, können sie es [per URL hochladen](../../using-miro/import-and-export/import/05-uploading-files-to-boards.md). |
| Emoji-Reaktionen | Kann manuell neu erstellt werden | Keine |
| Rahmen | Rahmen | Keine |
| Raster (Tabellen) | Tabellen | Keine |
| Gruppierte Objekte | Ungruppierte Objekte | Um Objekte neu zu gruppieren, markiere alle relevanten Objekte und drücke **Cmd/Strg + G**, oder klicke im Kontextmenü auf **Objekte gruppieren**. |
| Bilder | Bilder | Keine |
| Seiten | Eingebettetes Dokument | Der Inhalt kann als .docx-Datei vom Miro Board heruntergeladen und bearbeitet werden. |
| Prototypen | Name der Quelle (InVision) und die URL der Einbettung | Wenn Nutzer ein Dokument erneut einbetten möchten, können sie es per URL hochladen. |
| Smarte Widgets:    Flip-Karte, Umfrage, Dies oder Das, Diagramme, Zähler, Leaderboard, Spinner, Buzzer, Personen, Story Points, T-Shirt-Größe, Timer, Aktionsschaltflächen | PNG des smarten Widgets zum Zeitpunkt des Imports wird erstellt | Der Inhalt ist nicht bearbeitbar. |
| Notizen | Notizen | Die Schriftgröße des Textes in den Notizen muss eventuell angepasst werden. |
| Zeitachse (Gantt) | CSV | Die Inhalte können als .CSV-Datei vom Miro Board heruntergeladen und bearbeitet werden. |
| Wireframes | Wireframes | Einige Objekte müssen möglicherweise neu gezeichnet werden. |

## Wichtige Einschränkungen

Achte auf die folgenden Einschränkungen und strukturellen Unterschiede, wenn du deine Inhalte von Freehand nach Miro migrierst, um einen reibungsloseren Übergang zu gewährleisten:

- Miro-Textfelder können bis zu 6.000 Zeichen, einschließlich Leerzeichen, aufnehmen. Jeder zusätzliche Text wird abgeschnitten.
- Miro-Notizen unterstützen keine Farbpalettenanpassungen oder Textaufzählungen in der gleichen Weise wie Freehand; einige Formatierungen können davon abweichen.
- Freehand Smart Widgets werden als statische Bilder (PNGs) importiert und können nicht in Miro bearbeitet werden.
- Kommentare, Emoji-Reaktionen und Prototypen aus Freehand werden nicht nach Miro migriert.
- Der für den Massenimport erforderliche Freehand-Token ist nur zwei Wochen lang ab dem Datum gültig, an dem du ihn erhalten hast.
- Ab dem 31. Dezember 2024 um 23:59 Uhr EST werden Freehand und alle zugehörigen Migrationstoken eingestellt und ungültig gemacht. Nutzer können keine neuen Tokens mehr generieren oder auf Freehand zugreifen.

### Vergleiche die Organisationsstruktur zwischen Freehand und Miro

Um deine Migration effektiv zu planen, ist es wichtig zu verstehen, wie die Organisationsstrukturen in Freehand mit denen in Miro übereinstimmen:

**Organisationsebenen von Freehand**

- Teams: Jede Subdomain, auf die du in InVision Zugriff hast, gilt als Team. Wenn du nur Zugang zu einer Subdomain hast, hast du nur ein Team.
- Gruppen: Dokumentenordner, die das Gruppieren und Freigeben von Dokumenten in deinem Team erleichtern.
- Bereiche: Eine zusätzliche Organisationsebene innerhalb von Gruppen für deine Dokumente.

:::note
Wenn dein Team in Freehand die Bereichsübersicht genutzt hat, musst du diesen Inhalt manuell nach Miro migrieren. Wir empfehlen, den Inhalt der Bereichsübersicht auf ein Miro-Board zu kopieren.
:::

**Miro-Organisationsschichten**

- Organisationen: Normalerweise hast du nur Zugang zu einer einzigen Organisation in Miro.
- Teams: Gemeinsame Arbeitsbereiche, in denen Nutzer an Boards und Projekten zusammenarbeiten (früher gelegentlich als "Spaces" bezeichnet, beachte die sich entwickelnde Terminologie von Miro; generell sind Teams der primäre kollaborative Arbeitsbereich).
- Projekte: Sammlungen von Boards innerhalb eines Teams, die das Organisieren, Abrufen und Freigeben von Boards erleichtern.

Betrachte deine InVision-Gruppen als grob gleichwertig mit Miro-Projekten (oder was konzeptionell ähnlich wie Bereiche/Spaces zum Organisieren von Boards innerhalb eines Teams gewesen sein könnte). Für jede InVision-Gruppe, die du migrieren möchtest, empfehlen wir, ein Miro-Projekt mit demselben Namen zu erstellen. Wenn du zum Beispiel eine InVision-Gruppe mit dem Namen "Acme Corp Relaunch Project" hast, empfehlen wir dir, ein Miro-Projekt mit dem gleichen Namen "Acme Corp Relaunch Project" innerhalb des entsprechenden Miro-Teams einzurichten.

:::tip
Bei weiteren Fragen zur Freehand-Migration wende dich bitte an den [Miro-Support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) oder direkt an deinen Miro Customer Success Manager.
:::
