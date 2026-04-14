---
title: Lucidspark-Boards in Miro importieren
article_id: 9549014537490
translation_id: 9549014537490
locale: de
sidebar_position: 7
created_at: '2023-01-12T09:05:07Z'
updated_at: '2026-01-19T14:30:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Personen: Alle Nutzer mit Bearbeitungszugriff auf sowohl Lucidspark- als
    auch Miro-Boards Pläne: Free, Starter, Business, Education und Enterprise Plattformen:
    Browser, Desktop'
---

Übertrage deine Lucidspark-Inhalte nahtlos in Miro und erlebe eine bessere Zusammenarbeit. Dieser Leitfaden beschreibt, wie du deine Boards importierst und was du während des Prozesses erwarten kannst.

> **Warnung:** Die Bearbeitung von importierten Inhalten ist unidirektional. Änderungen, die in Miro vorgenommen werden, werden nicht mit Lucidspark synchronisiert.

> **Hinweis:** Lucidspark-Boards mit freien oder eingeschränkten Lizenzen können migriert werden.

## So importierst du Lucidspark-Boards via PDF-Export

Befolge diese Schritte, um deine Lucidspark-Boards mithilfe der PDF-Export-Methode nach Miro zu importieren:

1. Stelle sicher, dass du die **Lucidspark**-Inhalte, die du nach Miro importieren möchtest, als PDF exportierst.
2. Klicke auf dem Miro **Dashboard** auf **+ Neu erstellen**.
3. Wähle **Importieren** und dann **Aus Lucidspark importieren**.
   Das **Dialogfeld Aus Lucidspark importieren** öffnet sich. Du kannst mehrere Lucidspark-PDFs auf einmal importieren.
4. Befolge die auf dem Bildschirm angezeigten Anweisungen im Dialogfeld.
5. Wähle **Boards importieren**.
6. Überprüfe die importierten Inhalte und nimm alle notwendigen Anpassungen vor. Obwohl Lucidspark und Miro ähnliche Funktionen haben, kann es dennoch Unterschiede bei den Stil- und Formatierungsoptionen geben. Schaue dir [Wie Lucidspark-Objekte in Miro erscheinen (Bulk PDF-Importmethode)](#lucidspark-object-mapping-bulk-import) an, um Anleitungen zur Abbildung der Objekte zu erhalten.

## Alternative Methode: Inhalte kopieren und einfügen

Als schnellere Alternative für kleinere Inhaltsmengen kannst du Elemente direkt von einem geöffneten Lucidspark-Board kopieren und auf ein Miro-Board einfügen.

> **Hinweis:** Jeder Nutzer mit Bearbeitungsrechten für die Boards von Lucidspark und Miro sollte in der Lage sein, Inhalte aus Lucidspark zu kopieren und in Miro einzufügen. Für Details, wie Objekte mit dieser Methode übersetzt werden, siehe [Wie Lucidspark-Objekte in Miro erscheinen (Kopieren/Einfügen-Methode)](#lucidspark-object-mapping-copy-paste).

## Wie Lucidspark-Objekte in Miro erscheinen (Kopieren/Einfügen-Methode)

Diese Tabelle bietet einen umfassenden Vergleich, wie Objekte übersetzt werden, wenn Sie Inhalte direkt von Lucidspark kopieren und in Miro einfügen.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Azure-Karten | Azure-Karten werden als Miro-Karten migriert: 1. Richte die Azure-Integration in Miro ein. 2. Konvertiere die Miro-Karten in [Azure-Karten](../../integrations-apps/microsoft/03-azure-cards.md). |
| Mitwirkende und Freigabe | 🟠 Kann manuell nachgebildet werden |
| Kommentare | 🟠 Kann manuell nachgebildet werden |
| Konnektoren & Trennlinien | Konnektoren |
| Container | Formen |
| Dokumente aus Dateien und URLs | 🟠 Kann manuell neu erstellt werden |
| Dokument-URLs (PDF) | Eingebettete Dokumente |
| Zeichnen | Bilder |
| Dynamische Tabellen | Tabellen |
| Emojis | Bilder |
| Rahmen | Rahmen |
| GIFs aus der Symbolleiste | Bilder |
| GIFs aus Dateien | Bilder |
| GIFs von URLs | GIFs |
| Bilder | Bilder |
| Jira-Karten | Jira-Karten werden als Miro-Karten migriert:  1. Richte die Jira-Integration in Miro ein 2. Konvertiere die Miro-Karten zu [Jira-Karten](../../integrations-apps/atlassian/03-jira-cards.md). |
| Lucid-Karten | Karten |
| Mindmap | Mindmap |
| Formen | Formen |
| Notiz | Notizen |
| Tabellen | Tabellen |
| Text | Text |
| Zeitachse | 🟠 Kann manuell nachgebildet werden |
| Videos und andere URLs | Vorschaubilder |

## Wie Lucidspark-Objekte in Miro erscheinen (Massen-PDF-Importmethode)

Diese Tabelle bietet einen umfassenden Vergleich der Objekte zwischen Lucidspark und Miro nach dem Massenimport deiner Inhalte via PDF.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Azure-Karten | Bilder |
| Mitwirkende und gemeinsame Nutzung | 🟠 Kann manuell neu erstellt werden |
| Kommentare | 🟠 Kann manuell neu erstellt werden |
| Konnektoren & Teiler | Konnektoren |
| Container | Formen |
| Dokumente | 🟠 Kann manuell neu erstellt werden |
| Zeichnen | Linien |
| Dynamische Tabellen | Formen und Konnektoren |
| Emojis | Bilder |
| Rahmen | Rahmen und Formen |
| GIFs | Bilder |
| Bilder | Bilder |
| Jira-Karten | Formen |
| Lucid-Karten | Formen |
| Mindmap | Formen und Konnektoren |
| Formen | Formen |
| Notiz | Notizen |
| Tabellen | Tabellen/Formen und Konnektoren |
| Text | Text |
| Zeitachse | Formen und Verbinder |
| Videos und andere URLs | 🟠 Kann manuell nachgebildet werden |

## Einschränkungen des Imports

Während Lucidspark und Miro ähnliche Funktionen bieten, sollten Sie sich der folgenden Unterschiede und Einschränkungen beim Import von Inhalten bewusst sein:

- Miro-Textfelder können bis zu 6.000 Zeichen, einschließlich Leerzeichen, aufnehmen. Jeder zusätzliche Text wird abgeschnitten.
- Farben und Stile werden auf die naheliegendsten Entsprechungen in Miro angepasst.
- Die Deckkraftwerte von Lucidspark werden beim Import nicht genau extrahiert.
- Miro-Notizen unterstützen keine Rotation, Farbpalettenanpassung oder Textaufzählung, die in Lucidspark angewendet worden sein könnten.

## Hilfe erhalten

> **Hinweis:** Für weitere Fragen und Unterstützung rund um die Lucidspark-Migration wende dich bitte an den [Miro-Support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) oder direkt an deinen Miro Customer Success Manager.
