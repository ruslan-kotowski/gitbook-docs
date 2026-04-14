---
title: "Miro-Plugin f\xFCr Sketch"
article_id: 360017731173
translation_id: 360017731173
locale: de
sidebar_position: 13
created_at: '2019-02-11T10:13:46Z'
updated_at: '2025-02-26T12:15:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Das Miro-Plugin für Sketch ermöglicht eine einfache und schnelle Übertragung von Bildern aus Sketch direkt auf das Board. Sende deine Artboards an Miro und aktualisiere sie einfach mit einem Klick. Synchronisiere alle deine Bilder, wenn du eine Änderung vornimmst, ohne sie erneut hochzuladen.

### Aktivieren des Plugins

1. 1. Lade das Sketch-Plugin von GitHub herunter: folge [diesem Link](https://github.com/miroapp/sketch_plugin) > **Code** > **ZIP herunterladen**:

Download_from_Github.jpg

2. 2. Entpacke den Inhalt des Zip-Archivs > doppelklicke auf das RealtimeBoard.sketchplugin-Bundle, um das Plugin zu installieren.

plugin_installed.jpg
Das Miro-Plugin für Sketch ist installiert.

3. 3. Um es zu aktivieren, öffne Sketch, gehe zu **Plugins >** **Plugins verwalten** und markiere das Kästchen **Miro by Miro**.

Miro_plugin_in_Sketch.jpg
Das Miro-Plugin ist in Sketch aktiviert.

4. 4. Danach ist eine Authentifizierung mit deinen Miro-Anmeldedaten erforderlich. Dazu klickst du auf **Plugins -** **Miro:** **Melde dich bei Miro an, melde dich bei Miro ab**.

Log_in_to_Miro_in_Sketch.jpg
Bei Miro anmelden

5. 5. Gib deine E-Mail-Adresse und dein Passwort ein oder klicke auf **Unternehmens-Anmeldedaten verwenden**, wenn du dich über SSO anmeldest.

Miro_login.jpg
Das Authentifizierungsfenster für die Anmeldung bei Miro

### Hinzufügen von Sketsch-Artboards zu Miro

Um eine Sketch Zeichenfläche zu Miro hinzuzufügen, gehe zu **Plugins:** **Miro -** **Synchronisiere alle Zeichenflächen mit Miro**.

Im Dialogfenster besteht die Option, zwischen Boards zu wählen, die du via E-Mail-Einladung oder [Projekt](../../using-miro/sharing-boards/16-projects.md)-/Teamzugriff bearbeiten kannst.

> *⚠️ Hinweis: Boards, auf denen du [Besucher](../../using-miro/sharing-boards/08-collaboration-with-visitors.md) bisst, sind nicht verfügbar.*

Wähle ein Board aus, indem du a) auf einen der Vorschläge im Dropdown-Menü klickst oder b) indem du den Namen des Boards eingibst. Klicke dann, um **alle** oder **ausgewählte Artboards** hinzuzufügen. Markiere das Kästchen, wenn du **Miro nach dem Synchronisieren öffnen** möchtest:

select_a_board.jpg
Auswählen eines Boards für die Synchronisierung

Klicke auf **Synchronisieren**und die Artboards werden auf deinem Board angezeigt.

artiboards_in_Miro.jpg
**Bitte beachte, dass Artboards nur an bestehende Boards in Miro gesendet werden können.**

:::warning
Beachte, dass das direkte Kopieren und Einfügen von Artboards nur in der *Miro-Browserversion* verfügbar ist.
:::

### Synchronisieren von Sketch-Artboards mit Miro

Um die bereits zu Miro hinzugefügten und in Sketch geänderten Zeichenflächen zu synchronisieren, gehst du zu **Plugins -** **Miro:** **Synchronisiere alle Zeichenflächen mit Miro**. Das Board, mit dem du die Artboards zuvor synchronisiert hast, wird im Dialogfenster automatisch ausgewählt. Wähle einfach aus, ob du **alle** oder nur **ausgewählte Artboards** synchronisieren möchtest. Markiere das Kästchen, wenn du **Miro nach dem Synchronisieren öffnen** möchtest:

syncing_boards.jpg
Artboards mit Miro synchronisieren

### Deaktivieren des Plugins

Um die Synchronisierung von Sketch und Miro zu beenden, gehe zu **Plugins >** **Plugins verwalten** und deaktiviere das Kästchen **Miro by Miro**.

disable_Miro_sync.jpg
Das Miro-Plugin ist in Sketch deaktiviert.

### Mögliche Probleme und wie man sie löst

|  |  |  |
| --- | --- | --- |
| **Fehlermeldung/Problem** | **Mögliche Ursachen** | **Lösung** |
| 1. Ein Fehler ist aufgetreten. Während der Synchronisierung ist ein Fehler aufgetreten. Bitte versuche es erneut“. | 1. 1. Du verwendest eine veraltete Version von Sketch./span>  2. 2. Dein Sketch-Artboard ist riesig (es befindet sich ein sehr großes Bild im Sketch-Artboard). | 1. 1. Aktualisiere auf die neuere Version des Sketch-Plugins.  2. 2. Überprüfe die Bildgröße und verringere sie, wenn nötig. |
| 2. Verbindungsfehler Etwas ist schiefgelaufen | 1. 1. Das Plugin kann keine Verbindung mit Miro-API herstellen.  2. 2. Die Rate wird durch Miro-API begrenzt.  3. 3. Es gibt andere mögliche Probleme mit dem Netzwerk. | Melde dich ab und melde dich bei deinem Miro-Profil in Sketch an. Dann versuche erneut, das Artboard zu synchronisieren. |
| 3. Während der Synchronisierung ist ein Fehler aufgetreten. Bitte versuche es erneut“. | Das Problem kann durch Änderungen in deinen Netzwerkeinstellungen verursacht werden. | Zeichne Konsolenprotokolle auf und [sende einen Bug-Report an das Supportteam von Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md). |
| 4. 4. Das Sketch-Plugin friert ein und funktioniert nicht wie erwartet, wenn es versucht, mehrere Artboards mit Miro zu synchronisieren. | Dies geschieht, wenn du ein riesiges Miro-Board hast und versuchst, mehrere Artboards über das Sketch-Plugin zu synchronisieren. | Erstelle ein neues Miro-Board in Miro und synchronisiere jeweils ein einziges Artboard damit. |
| 5. 5. Die Boards erscheinen nicht in den Suchergebnissen von Sketch. | Dies geschieht, wenn ein Board in ein anderes [Projekt](../../using-miro/sharing-boards/16-projects.md) in Miro verschoben wurde oder wenn du keinen Platz in dem Projekt hast, in dem sich das Board befindet. | 1. 1. Überprüfe, ob ein Board, das nicht in der Sync-Liste in Sketch erscheint, in ein anderes Projekt in Miro verschoben wurde.  2. 2. Überprüfe, ob du einen Sitz in einem Projekt hast, in dem sich ein Board befindet. |
| 6. 6. Sketch ersetzt vorhandene Artboards auf einem Miro-Board nicht – sie werden auf der Leinwand dupliziert anstatt ersetzt. | Dies geschieht, wenn ein mit Sketch synchronisiertes Board [in ein anderes Miro-Team](../../using-miro/managing-boards/04-how-to-move-a-board.md) [verschoben](../../using-miro/managing-boards/04-how-to-move-a-board.md) worden ist. In diesem Fall werden die Bilder bei der ersten Synchronisation dupliziert. Im weiteren Verlauf werden sie ersetzt. | Lösche die vorherigen Artboards aus dem Miro-Board.  Die Duplikate werden ebenfalls ersetzt. |

#### So zeichnest du Sketch-Protokolle für den Miro-Support auf

1. Öffne die Spotlight-Suche /span>(klicke auf das Lupensymbol in der oberen rechten Ecke des Bildschirms). >Konsole:

spotlight_search.jpg
Spotlight-Suche

2. 2. Gib in das Suchfeld der Konsole**sketch-rtb-error** ein und suche nach Nachricht/beliebig:

search_in_Sketch.jpg
Konsolensuche

3. 3. Klicke auf die Zeile mit der Meldung im unteren Bereich der Konsole, mache einen Screenshot und teile ihn mit uns.

error_message.jpg
Konsole-Fehlermeldung
