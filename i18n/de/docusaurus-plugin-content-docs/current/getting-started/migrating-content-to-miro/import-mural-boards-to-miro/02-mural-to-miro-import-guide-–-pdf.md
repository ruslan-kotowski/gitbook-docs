---
title: Anleitung für den Import von Mural zu Miro – PDF
article_id: 22856050009362
translation_id: 22856050009362
locale: de
sidebar_position: 2
created_at: '2024-11-25T14:36:20Z'
updated_at: '2026-01-19T14:43:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personen: Nutzer mit Bearbeitungszugriff Pläne: Business, Education, Enterprise,
    Starter Plattformen: Browser, Desktop'
---

Du kannst deine bestehenden Mural-Boards in Miro importieren, indem du sie zuerst als PDF-Dateien aus Mural exportierst und dann diese PDFs in Miro importierst. Dieser Artikel bietet Anleitungen, um die besten Ergebnisse bei PDF-Importen zu erzielen, erklärt das Importverfahren und beschreibt, was du erwarten kannst, wenn verschiedene Mural-Elemente mit dieser Methode in Miro importiert werden.

Die PDF-Importmethode ist besonders effektiv für Inhalte, die sich möglicherweise nicht gut über Kopieren-Einfügen oder API-basierte Importe übertragen lassen. Der PDF-Importer von Miro analysiert die Formen und deren Koordinaten innerhalb des Mural-PDFs und versucht, das ursprüngliche Layout zu rekonstruieren. So können zum Beispiel sich überschneidende Linien als Tabellenstruktur interpretiert werden.

Bitte beachte, dass einige Objekte nach dem Import in Miro anders aussehen können und dass präzise Gestaltung und Layout eventuell manuelle Anpassungen oder Nachbildungen in Miro erfordern. Generell erzielen einfachere Inhalte mit weniger komplexen Gestaltungselementen genauere Importergebnisse.

## Richtlinien für den Import aus Mural

Um die besten Ergebnisse beim Importieren von Mural-Inhalten als PDFs zu erzielen, ist es hilfreich zu verstehen, wie der Importer funktioniert und welche Inhalte am effektivsten übertragen werden. Der PDF-Importer ordnet hauptsächlich grundlegende Formen und Linien zu.

:::note
**Hinweis:** Um Inhalte in Miro zu importieren, muss dein Mural-Inhalt unter einer vollständigen oder kostenlosen eingeschränkten Lizenz in Mural stehen.
:::

Klarer Abstand zwischen Elementen in deinem Mural ermöglicht es dem Miro-Importer, die Inhalte genauer zu analysieren. Ein Mural-Board mit vielen eng beieinander liegenden Elementen kann gemischte oder weniger genaue Importergebnisse erzeugen.

Um eine möglichst treue Übertragung zu gewährleisten, stelle sicher, dass dein Mural-Inhalt **nicht** folgende Attribute enthält, da diese möglicherweise nicht gut per PDF übertragen werden:

- Benutzerdefinierte Schriftarten
- Komplexe Stile, die grundlegende Formen transformieren (z.B. stark abgerundete Ecken bei Rechtecken, einzigartig gebogene Pfeile)
- Zahlreiche überlappende Formen und Linien
- Gedrehte Elemente

:::tip
**Tipp:** Wenn du das genaue Styling, komplexe Layouts oder präzise Koordinaten deines Mural-Inhalts beibehalten möchtest, ist die zuverlässigste Methode, die Inhalte als statisches Bild (z.B. PNG, JPG) aus Mural zu exportieren und dieses Bild dann in dein Miro-Board zu importieren.
:::

## Mural-Boards als PDFs in Miro importieren

In diesem Abschnitt wird erklärt, wie du deine Inhalte aus Mural mithilfe der PDF-Importfunktion in Miro importierst.

### Voraussetzungen für den PDF-Import

Bevor du mit dem Importprozess beginnst, stelle bitte sicher, dass du die folgenden Voraussetzungen erfüllst:

- Du musst Bearbeitungszugriff auf das Quell-Board in Mural haben (um es als PDF zu exportieren).
- Du musst Bearbeitungszugriff auf das Ziel-Board in Miro haben, in das du die Inhalte importieren möchtest.
- Du musst dein(e) Mural-Board(s) bereits als PDF-Dateien heruntergeladen haben.

**Weitere Informationen:** Anleitungen zum Exportieren aus Mural finden Sie in der Mural-Dokumentation unter [Export and download your mural's content](https://support.mural.co/s/article/export-and-download-your-mural-s-content) (externer Link).

### PDF importieren

Folgen Sie diesen Schritten, um Ihre Mural-PDF-Dateien in Miro zu importieren:

1. Klicken Sie im Miro-Dashboard auf die **+ Erstellen**-Schaltfläche.
2. Wählen Sie im Dropdown-Menü **Importieren** und dann **Aus Mural importieren**.
   Das **Boards aus Mural importieren**-Dialogfeld wird geöffnet.
3. Folge den Anweisungen auf dem Bildschirm im Dialogfeld. Du wirst aufgefordert, deine Mural-PDF-Dateien hochzuladen.
   Optional kannst du wählen, deinen importierten Inhalt einem bestimmten Miro-Bereich hinzuzufügen. Wenn du keinen Bereich angibst, wird der importierte Inhalt deinem Haupt-Team-Bereich hinzugefügt.
4. Sobald du deine Dateien hochgeladen und Optionen konfiguriert hast, wähle **Import boards**.
   Der Importvorgang beginnt. Du erhältst eine E-Mail-Benachrichtigung von Miro, sobald der Import abgeschlossen ist.

Du hast nun erfolgreich deinen Mural-Inhalt über PDF nach Miro importiert.

## Erwartete Ergebnisse

Beim Import von Mural-Objekten in Miro über PDF sind einige Abweichungen in der Formatierung und im Styling zu erwarten, da es Unterschiede zwischen den Plattformen gibt und die Natur der PDF-Konvertierung dies beeinflusst. Dieser Abschnitt beschreibt die typischen Importergebnisse für gängige Mural-Objekte und bietet einige bewährte Praktiken.

### Bereiche

Der äußerste Bereich in deinem Mural-Export wird in der Regel als Miro-Rahmen importiert. Andere, innere Bereiche werden normalerweise als reguläre Formen in Miro importiert.

:::note
**Hinweis:** Verschachtelte Bereiche (Bereiche innerhalb von Bereichen) können manchmal beim Import falsch erkannt oder strukturiert werden. Der PDF-Importer stützt sich auf visuelle Koordinaten, um Eltern-Kind-Beziehungen von Widgets zu bestimmen, was bei komplexer Verschachtelung zu Mehrdeutigkeiten führen kann.
:::

### Konnektoren

Der PDF-Importer erkennt und reproduziert hauptsächlich Verbindungen mit durchgezogenen Linien. Gepunktete oder gestrichelte Verbindungen werden möglicherweise nicht wie erwartet importiert.

Wenn ein Verbinder in Mural Text enthält, der direkt auf der Linie eingebettet ist, kann der PDF-Importer dies als zwei separate Linien mit dem Textobjekt in der Nähe interpretieren, anstatt als einen einzigen Verbinder mit Text.

![A connector with text that the PDF importer breaks into two lines.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Ein Verbinder mit Text, den der PDF-Importer in zwei Linien „zerlegt“.*

### Zeichnungen

Handgezeichnete Elemente aus Mural werden in Miro im Allgemeinen als eine Sammlung von Linien oder Kurven importiert.

Bei komplexen Zeichnungen kann der PDF-Importer manchmal fälschlicherweise Teile der Zeichnung mit überlappenden oder nahegelegenen Objekten verknüpfen und sie als Verbindungen interpretieren, obwohl keine beabsichtigt waren.

![A drawing may import as linked to a nearby or overlapping object.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Eine Zeichnung kann importiert werden, als ob sie mit einem benachbarten oder überlappenden Objekt verbunden wäre.*

### GIFs

Der PDF-Importer erkennt GIFs aus Mural, importiert sie jedoch als statische Bilder (normalerweise der erste Frame des GIFs).

:::note
**Hinweis:** Das PDF-Dateiformat selbst unterstützt keine animierten GIFs. Dies ist eine Einschränkung von PDF, nicht des Miro-Importers.
:::

### Bilder

Bilder von deinem Mural-Board werden als Bilder in Miro importiert. Aufgrund von Unterschieden in den Koordinatensystemen zwischen Mural und Miro und dem PDF-Konvertierungsprozess kann sich ihre genaue Position auf dem Board jedoch leicht ändern.

### Listen

Listen (sowohl nummerierte als auch Aufzählungslisten) aus Mural werden in der Regel als Listen in Miro importiert. Für die besten Ergebnisse sollten deine Listen in Mural die Standardmarker verwenden (Standardnummern für geordnete Listen und einfache Aufzählungszeichen für ungeordnete Listen).

![A numbered list, and a bulleted list, with default markers, numerals and bullets respectively.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Eine nummerierte Liste und eine Aufzählungsliste mit Standardmarkierungen, Ziffern und Aufzählungszeichen.*

### Mindmaps

Die PDF-Importmethode funktioniert am besten für Mural-Mindmaps, die einen einzigen Wurzelknoten und sichtbare Ränder an allen Knoten haben. Komplexe Mindmaps mit mehreren Wurzeln oder versteckten Rändern werden möglicherweise nicht genau importiert.

![A basic Mind map is easier to import as PDF.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Eine einfache Mindmap ist leichter als PDF zu importieren*

Der PDF-Importer kann Schwierigkeiten haben, Mindmaps genau zu interpretieren, da diese häufig viele Linien und Objekte in unmittelbarer Nähe enthalten. Sollte Ihre PDF-Mindmap schlecht importiert werden, ziehen Sie in Betracht, den Inhalt der Mindmap direkt von Mural nach Miro zu kopieren und einzufügen. Während bei der Kopier-und-Einfügen-Methode manuelle Anpassungen des Stils und Maßstabs in Miro erforderlich sein können, könnte die strukturelle Treue bei einigen Mindmaps insgesamt höher sein.

### Formen

Der PDF-Importer ist so konzipiert, dass er grundlegende Mural-Formen (z. B. Rechtecke, Ovale, Dreiecke) als bearbeitbare Miro-Formen importiert.

![Only basic shapes import as editable content.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Nur grundlegende Formen werden als bearbeitbare Inhalte importiert*

Fortgeschrittene, benutzerdefinierte oder stark gestylte Formen aus Mural sowie gedrehte Formen können stattdessen als statische Bilder und nicht als bearbeitbare Miro-Formen importiert werden.

### Notizen

Standard-Notizen aus Mural werden in der Regel als Miro-Notizen importiert. Für die höchste Genauigkeit verwenden Sie Mural-Notizen mit den standardmäßigen Seitenverhältnissen (z. B. die gängigen Größen 3x3 oder 5x3).

![Sticky notes with the default size can be easily imported.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Notizen mit der Standardgröße lassen sich leicht importieren*

:::note
**Hinweis:** Runde Notizen aus Mural werden in Miro als reguläre Formen importiert, da Miro keine native runde Notiz-Funktion hat.
:::

Überlappende oder gedrehte Notizen können möglicherweise nicht mit hoher Genauigkeit importiert werden und erfordern unter Umständen manuelle Anpassungen oder Neupositionierungen in Miro.

![Import results vary for rotated sticky notes, and sticky notes that overlap.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Importresultate variieren bei gedrehten und überlappenden Notizen.*

### Tabellen

Einfache Tabellen aus Mural mit klaren Gitterlinien werden in der Regel als Miro-Tabellen oder als eine Ansammlung von Formen und Linien, die eine Tabellenstruktur bilden, mit hoher Genauigkeit importiert.

Tabellen mit komplexer Geometrie können als eine Reihe von nicht verbundenen Linien und Textfeldern importiert werden. Für die besten Ergebnisse beim Import von Tabellen sollten die Tabellen in Ihrem Mural-Export **nicht** über folgende Attribute verfügen:

- Zusammengeführte Zellen
- Unsichtbare oder versteckte Rahmen
- Abgerundete Ecken an Zellen oder dem Tabellenrand

![Complex tables do not import with high fidelity.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Komplexe Tabellen werden nicht mit hoher Wiedergabetreue importiert.*

### Text

Textobjekte aus Mural werden in der Regel als editierbarer Text in Miro importiert, oft in einem einzigen Textblock oder einer Form, die dem originalen Mural-Textfeld entspricht.

Um den Textimport mit höchster Genauigkeit sicherzustellen, verwenden Sie in Mural Standard-Schriftarten und -Ränder.

:::note
**Hinweis:** Die Schriftgröße kann nach dem Import variieren, und möglicherweise muss sie in Miro manuell angepasst werden.
:::

Der PDF-Importer kann Text, der benutzerdefinierte Schriftarten verwendet oder komplexes Styling hat (z. B. mehrere Stile innerhalb eines einzigen Textblocks), in mehrere kleinere Textblöcke aufteilen.
