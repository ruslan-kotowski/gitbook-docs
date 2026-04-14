---
title: Probleme beim Exportieren des Boards
article_id: 360020567820
translation_id: 360020567820
locale: de
sidebar_position: 3
created_at: '2021-03-18T12:15:46Z'
updated_at: '2025-11-05T13:45:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Du kannst dein [Miro-Board exportieren](../../import-and-export/export/03-how-to-export-your-board.md) als Bild, PDF oder CSV-Datei. Wenn du beim Exportieren deines Miro-Boards Probleme hast, könnten dir die folgenden Lösungen weiterhelfen.

## Ich kann das Board nicht exportieren

**Export-Schaltfläche fehlt auf meinem Board**

Die Export-Schaltfläche befindet sich im **Dreipunktmenü** (**...**), dann im Untermenü **Board**.

Keine Exportoption im [Board-Menü](../../../getting-started/start-here/your-first-board/05-toolbars.md):

1. Überprüfe, ob der Eigentümer/Miteigentümer des Boards erlaubt hat, das Board in den Inhaltseinstellungen zu exportieren.

   Um den Namen des Board-Eigentümers herauszufinden, klicke auf den Board-Namen in der oberen linken Ecke, um die Board-Informationskarte zu öffnen. Wenn dir diese Informationen nicht angezeigt werden, kannst du den Namen der Person, die dich zum Board eingeladen hat, in der Einladungs-E-Mail überprüfen.

   Kontaktiere den Eigentümer des Boards und bitte ihn, die Option für dich im **Fenster Freigeben** > **Freigabeeinstellungen** zu aktivieren. > **Berechtigungen**. Der Eigentümer/Miteigentümer muss auswählen, welche Kategorie von Nutzern den [Board-Inhalt kopieren](../../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md) kann.
   ![.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044218642_.gif.png)
   *Konfigurieren, wer das Board kopieren kann*
2. Vergewissere dich, dass dein Browser, dein Preisplan und dein Gerät das Exportieren unterstützen. Hier kannst du die Verfügbarkeit überprüfen. Wenn dein Browser, Preisplan oder Gerät die Exportoption nicht unterstützt, empfehlen wir, zu einem anderen Browser oder Gerät zu wechseln oder [ein Upgrade für dein Team durchzuführen](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

   |  |  |  |  |  |  |
   | --- | --- | --- | --- | --- | --- |
   |  | Free-Preisplan | | Starter-, Business-, Enterprise-, Education-Preispläne | | Export als CSV (alle Preispläne) |
   |  | Niedrige Auflösung | Hohe Auflösung ohne Wasserzeichen | Niedrige  Auflösung | Hohe Auflösung  ohne Wasserzeichen |
   | Google Chrome | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Safari | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Firefox | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Opera | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Edge < 79 | ✘ | ✘ | ✘ | ✔ | ✘ |
   | [Desktop-App](../../../getting-started/apps-for-devices/05-desktop-app.md) | ✔ | ✘ | ✔ | ✔ | ✔ |
   | Tablet | ✔ | ✘ | ✔ | ✔ | ✘ |
   | Mobil | ✘ | ✘ | ✘ | ✘ | ✘ |

**Für Exporte in niedriger Qualität**

Um Probleme zu beheben, schließen Sie Browser-Tabs und Hintergrund-Tabs. Sie können auch versuchen, den Browser zu wechseln.

Für Exporte in hoher Qualität tun Sie Folgendes:

- Verbergen Sie Rahmen, die Sie nicht exportieren möchten. Inhalte in verborgenen Rahmen werden nicht exportiert.
- Teilen Sie das Board in kleinere Boards auf, um sie zu exportieren.

**Allgemeine Tipps**

- Packs alles, was du exportieren möchtest, in Rahmen, da nur Widgets innerhalb von Rahmen exportiert werden.
- Vermeide PDF in PDF. Wenn du ein PDF auf einem Board hast, das als PDF exportiert werden soll, ersetze das PDF auf dem Board durch Bilder in geringer Qualität.
- Konvertiere hochauflösende Bilder in JPEG oder verkleinere sie mit einem externen Tool.
- Überprüfe die Statusseite von Miro auf relevante Störungen.
- Unterteile das Board in Rahmen und exportiere die Rahmen separat. Einzelne PDFs können später mit einem externen Tool wieder zusammengefügt werden.
- Teile große Boards in kleinere Boards auf und nutze [Bereiche](../../spaces/01-spaces.md), um organisiert zu bleiben und zusammengehörende Boards zu gruppieren.

**„Beim Erstellen des PDF-Dokuments ist leider etwas schiefgelaufen.“**

Versuche, das Board in Rahmen zu unterteilen und die Rahmen einzeln zu exportieren, da das Problem durch die Größe des Boards verursacht werden könnte.

Wenn das nicht hilft, überprüfe [die Konsolenprotokolle deines Browsers](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md). Wenn die Protokolle die folgende Meldung enthalten:

```
ERR_CONNECTION_ABORTED
```

*wo:*

Der Export wird von der Sicherheitssoftware auf deinem Gerät oder einer Firewall in deinem Netzwerk blockiert.

Du (oder dein System-Admin) musst die Einstellungen deines Antivirenprogramms und/oder deiner Firewall so konfigurieren, damit Miro das Exportverfahren durchführen kann.

Wenn du dir unsicher bist, [kontaktiere Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).

**Nichts passiert, wenn ich versuche, ein Board als PDF zu exportieren, und Miro zeigt keinen Fehler an**

Dieses bekannte Problem tritt hauptsächlich im Safari-Browser auf, wenn Pop-up-Fenster deaktiviert sind. Um das Problem in Safari zu beheben, [gehe wie folgt vor](https://support.apple.com/en-gb/guide/safari/sfri40696/mac). Stelle sicher, dass du Pop-up-Fenster für miro.com oder alle Websites aktivierst. Kehre zu Miro zurück und versuche erneut, dein Board zu exportieren.

Für Chrome [gehe wie folgt vor](https://support.google.com/chrome/answer/95472?hl=en&co=GENIE.Platform%3DDesktop).

## Ich habe Probleme mit exportierten Dateien (PDFs, Bilder, CSVs)

**Bilder/PDFs sind auf dem exportierten Dokument verschwommen**

Wenn hochgeladene Bilder oder PDFs auf deiner gespeicherten Datei verschwommen sind:

1. Stelle den Board-Zoom auf 100 % ein und lass die Bilder/PDFs rendern, bevor du das Board exportierst
2. Das hochgeladene Bild oder die PDF-Datei ist eventuell zu komplex oder zu groß für den Export. Um die Datei zu verkleinern, wandle das Bild/die PDF-Datei in ein PNG-Format um und ersetze es auf dem Board. Exportiere das Board danach noch einmal

Der Free-Preisplan unterstützt nur einen Export in geringer Qualität. Wenn du dein Board in hoher Qualität exportieren möchtest, empfehlen wir, [es zu einem kostenpflichtigen Team zu verschieben](../../managing-boards/04-how-to-move-a-board.md) oder [dein Team upzugraden](../../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md).

**Die Reihenfolge der Seiten ist nicht die gleiche wie die Reihenfolge der Rahmen auf dem Board**

Die Reihenfolge der als PDF exportierten Rahmen ist die gleiche wie im Rahmen-Panel. So änderst du die Reihenfolge der Rahmen:

1. Öffne die Board-Übersicht in der unteren linken Ecke
2. Ziehe Rahmen, um ihre Position auf der Liste zu ändern. Du kannst auch [Magic organize](../../essential-tools/07-frames.md) verwenden, um deine Rahmen schnell in der Reihenfolge anzuordnen, in der sie auf dem Board platziert sind.
   ![move_frames.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057584914_move%20frames.gif)
   *Die Reihenfolge der Rahmen ändern*

**Die exportierte Datei ist abgeschnitten**

Wenn du **dein Board als Bild exportierst**, füge alle Inhalte, die du exportieren möchtest, in die ausgewählte, exportierte Fläche ein.

![save_as_image.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057583890_save%20as%20image.gif)
*Das Board als Bild exportieren*

Wenn du **dein Board als PDF exportierst**, erstelle einen Rahmen, der alle Inhalte umfasst, die du exportieren möchtest. Dann [exportiere den Rahmen](../../import-and-export/export/03-how-to-export-your-board.md).

**Die exportierte PDF-Datei enthält keine Rahmentitel**

Wenn du dein Board als PDF-Datei exportierst, sind die Rahmentitel nicht Teil des Exports. Du kannst die Rahmentitel ersetzen, indem du das [Text-Werkzeug](../../essential-tools/16-text.md) verwendest und den Text auf die Rahmen setzt. Die Titel werden auf deiner PDF-Datei angezeigt.

**Die Daten in einer exportierten CSV-Datei sind nicht strukturiert**

Derzeit behält der CSV-Export die Struktur oder die Verhältnisse des Boards nicht bei. Wenn du jedoch [Tabellen](../../advanced-tools/05-grid.md) als CSV-Datei exportierst, wird die Struktur gespeichert.

Wenn du eine [Mindmap](../../advanced-tools/03-mind-map.md) als Datei mit intelligenter Datenstruktur exportieren möchtest, verwende den [Mindmap Downloader](https://miro.com/marketplace/mindmapdownloader/?backUrl=%2Fmarketplace%2F).

**Die Schriftarten auf der exportierten Datei unterscheiden sich von den Schriftarten auf dem Board**

Miro-Exporte verwenden die Schriftarten, die auf dem Betriebssystem deines Geräts installiert sind. Wenn die Schriftart in deinem Betriebssystem nicht vorhanden ist, wird eine ähnliche Schriftart von deinem System verwendet. Wenn dieselbe Schriftart wie auf deinem Miro-Board benötigt wird, wähle eine andere Schriftart auf dem Board oder installiere die benötigte Schriftart auf deinem Gerät.

## Ich finde die exportierte Datei nicht

**Ich finde die exportierte Datei auf meinem Gerät nicht**

**Wenn du Miro in einem Browser verwendest**

werden die Dateien in dem Ordner gespeichert, in dem die Browser-Downloads standardmäßig gespeichert sind. Du kannst die Download-Optionen in den Browser-Einstellungen überprüfen.

**Wenn du die Miro Desktop-App oder Tablet-App verwendest**

schau im Downloads-Ordner auf deinem Gerät nach. Du kannst auch deine Dateien nach dem Namen des Boards durchsuchen.

**Miro erstellt jedes Mal einen neuen Ordner, wenn ich ein Board exportiere**

> **Relevant für**: [Windows Desktop-App](../../../getting-started/apps-for-devices/05-desktop-app.md)

Es kann sein, dass der Pfad in den Miro-App-Einstellungen gespeichert wurde. So löschst du den Pfad:

1. Lösche die Desktop-App von Miro
2. Gib unten links in der Windows-Suchleiste **%AppData%** ein und öffne den Ordner **Local**, dann lösche den Ordner **RealTimeBoard**
3. Öffne **%AppData%** erneut, gehe zum Ordner **Roaming**, und lösche den Ordner **RealTimeBoard**

Installiere die neueste [Miro-App](https://miro.com/apps/).

Wenn keine der Lösungen hilft, [wende dich an den Miro Support](../../tools/troubleshooting/06-contacting-miro-support.md).
