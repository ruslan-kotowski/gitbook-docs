---
title: Miro AI-Referenz
article_id: 20970362792210
translation_id: 20970362792210
locale: de
sidebar_position: 17
created_at: '2024-08-26T09:34:26Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Verfügbar für: Alle Nutzer Preisplan: Free, Starter, Business, Enterprise,
    Education Plattformen: Browser, Desktop, Mobile'
---

Dieser Referenzartikel beschreibt die Funktionalitäten von Miro AI.

## Miro KI-Modelle

Modelle werden in der Regel auf Provider-Infrastruktur oder Microsofts Azure KI-Dienst oder AWS Bedrock gehostet. Für Kunden, die Miro über den AWS Marketplace beziehen, werden alle Modelle auf AWS Bedrock gehostet.

### KI-gestützte Erstellung & Iteration

| **Miro AI Funktion** | **Beschreibung** | **Modell** |
| --- | --- | --- |
| Gesprächszusammenfassungen | Erzeugt eine Zusammenfassung von langen Kommentar-Threads auf deinem Miro-Board. | GPT 4o-mini |
| Diagramm erstellen - Flussdiagramm | Erstellt ein Flussdiagramm aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | GPT-4o |
| Diagramm bearbeiten - Flussdiagramm | Bearbeitet ein Flussdiagramm aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | GPT-4o |
| Diagramm erstellen - Mindmap | Erstellt eine Mindmap aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | GPT 4o-mini |
| Diagramm bearbeiten - Mindmap | Bearbeitet eine Mindmap anhand eines Nutzer-Prompts und ausgewählten Board-Inhalten. | GPT-4o |
| Diagramm erstellen – ERD | Erstellt ein Entity-Relationship-Diagramm (ERD) anhand eines Nutzer-Prompts. Eine **Erstellen mit KI**-Option. | GPT 4o-mini |
| Diagramm bearbeiten - ERD | Bearbeitet ein ERD basierend auf einem Nutzer-Prompt und ausgewählten Board-Inhalten. | GPT-4o |
| Diagramm digitalisieren | Wandelt Bilder von handgezeichneten Diagrammen in vollständig bearbeitbare Diagramme in Miro um. | Claude 3.7 Sonnet (AWS Bedrock) |
| Dokument erstellen | Erstellt ein Miro-Dokument aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. Eine **Erstellen mit KI**-Option. | GPT-4o |
| Dokument bearbeiten | Bearbeitet ein Miro-Dokument aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | GPT-4o |
| Bild erstellen | Erstellt ein Bild aus einem Nutzer-Prompt, einschließlich Board-Objekten als Kontext. Eine **Erstellen mit KI**-Option. | Segmind Stable Diffusion 1B (SSD-1B) + StabilityAI Diffusion XL Refiner 1.0 |
| Bild bearbeiten | Bearbeitet ein Bild von einem Nutzer-Prompt mit Board-Objekten als Kontext. Eine **Erstellen mit KI**-Option. | GPT-4o |
| Bild in Prototyp umwandeln | Wandelt eine Skizze oder ein Prototypbild in einen editierbaren Miro-Prototyp um. | Eigenes Modell von Miro + Claude 3.7 Sonnet |
| Bild-Alt-Text | Generiert Alt-Text für ein Bild. Verbraucht keinen KI-Credit. | Miro eigenes Modell |
| Notizen erstellen | Erstellt Miro-Notizen aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | GPT-4o |
| Notizen bearbeiten | Bearbeitet Miro-Notizen eines Nutzer-Boards und ausgewählte Board-Inhalte. | GPT-4o |
| Notizenerfassung | Wandelt ein Bild von physischen Notizen in Miro-Notizen um. | Eigenes Modell von Miro |
| Prototyp erstellen | Erstellt einen Miro Prototype aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | GPT-4o + Claude 4.5 Sonnet + GPT 4o-mini + Gemini 2.5 Flash Image (nano-banana) |
| Prototyp-Bildschirm bearbeiten | Bearbeitet einen Miro Prototyp-Bildschirm aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | Claude 4.5 Sonnet + Gemini 2.5 Flash Image (nano-banana) |
| Hintergrund entfernen | Entfernt den Hintergrund aus einem Bild. | Eigenes Modell von Miro |
| Intelligentes Zeichnen | Wandelt eine Bleistiftzeichnung in eine Linie, Form oder Notiz um. | Eigenes Modell von Miro |
| Tabelle erstellen | Erstellt eine Miro-Tabelle aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | Claude 3.7 Sonnet |
| Tabelle bearbeiten | Bearbeitet eine Miro-Tabelle aus einem Nutzer-Prompt und ausgewählten Board-Inhalten. | Claude 3.7 Sonnet |

### KI-gestützte KI-Kollegen

|  |  |  |
| --- | --- | --- |
| **Miro KI-Funktion** | **Beschreibung** | **Modell** |
| KI-Kollegen – Agiler Coach | Identifiziert die wichtigsten Themen in einer Retrospektive und schlägt die nächsten Schritte vor. | GPT-4o |
| KI-Kollege - Produktführung | Gibt Feedback und Vorschläge als Kommentare auf Rahmen, Notizen oder Text. Bietet auch Lösungsideen als Notizen. | GPT-4o |
| KI-Kollege - Produktmarketingleiter | Gibt Feedback und Vorschläge als Kommentare auf Rahmen, Notizen oder Text. | GPT-4o |

### KI-gestützte Sortierung

| **Miro AI-Funktion** | **Beschreibung** | **Modell** |
| --- | --- | --- |
| Sortierung von Notizen nach Stichwörtern | Sortiert Notizen nach Stichwörtern und gibt jeder Gruppierung einen Titel. | Claude 3.5 Haiku + Amazon Nova Micro |
| Sortierung von Notizen nach Meinung | Sortiert Notizen nach Meinung, wie Meinungen und Standpunkten, und teilt sie in positive, neutrale und negative Gruppierungen ein. | Claude 3.5 Haiku |

### Textbearbeitung mit KI

Die folgende Tabelle zeigt die Textbearbeitung powered by Miro AI:

|  |  |  |
| --- | --- | --- |
| **Miro AI-Funktion** | **Beschreibung** | **Modell** |
| Ton ändern | Ändert den Ton des ausgewählten Textes, um ihn freundlich, professionell, geschäftlich oder unterhaltsam zu gestalten. | GPT-5 nano |
| Rechtschreibung und Grammatik korrigieren | Korrigiert die Rechtschreibung und Grammatik des ausgewählten Textes. | GPT-5 |
| Für bessere Klarheit umformulieren | Formuliert ausgewählten Text zur besseren Klarheit neu. | GPT-5 Chat |
| Text kürzen | Kürzt den ausgewählten Text, ohne Klarheit und Lesbarkeit zu verlieren. | GPT-5 mini |
| Übersetzen | Übersetzt den ausgewählten Text ins Englische, Spanische, Deutsche, Französische, Japanische, Portugiesische, Koreanische, Polnische, Italienische, Türkische, Arabische, Russische, Dänische, Finnische, Norwegische, Niederländische, Schwedische oder Thailändische. Du kannst sowohl einzelne als auch mehrere Objekte gleichzeitig übersetzen. | GPT-5 mini |

### KI-gestützte Mindmaps

| **Miro AI-Funktion** | **Beschreibung** | **Modell** |
| --- | --- | --- |
| Mindmap erstellen | Generiert eine Mindmap von einem ausgewählten Stammknoten. | GPT 4o-mini |
| Mindmap - Mit Ideen erweitern | Generiert Ideen von einem ausgewählten Stammknoten oder untergeordneten Knoten. | GPT 4o-mini |
| Mindmap - Mit Themen erweitern | Generiert Themen von einem ausgewählten Stammknoten oder untergeordneten Knoten. | GPT 4o-mini |
| Mindmap - Mit Fragen erweitern | Generiert eine Frage von einem ausgewählten Stamm- oder untergeordneten Knoten. | GPT 4o-mini |

### KI-gestützte Präsentationen

Miro Präsentationen verwenden die folgenden Modelle:

- Amazon Titan
- Claude 4 Sonnet
- Claude 3.7 Sonnet
- Claude 3.5 Sonnet
- GPT-5
- GPT-4o
- Stable Diffusion 3.5 Large
- Stability Image Core

### Miro Insights

Um Kundenfeedback zusammenzufassen, verwendet [Miro Insights](https://help.miro.com/hc/articles/25438311770770) GPT-4o.

### AWS Marketplace-Kunden

**AWS Marketplace-Modelle**

| **Miro-AI-Funktion** | **Modell** |
| --- | --- |
| Gesprächszusammenfassungen | Claude Haiku 3.7 (AWS Bedrock) |
| Diagramm erstellen – Flussdiagramm | Claude Sonnet 3.7 (AWS Bedrock) |
| Diagramm bearbeiten – Flussdiagramm | Claude Sonnet 3.7 (AWS Bedrock) |
| Diagramm erstellen – Mindmap | Claude Sonnet 3.7 (AWS Bedrock) |
| Diagramm bearbeiten – Mindmap | Claude Sonnet 3.7 (AWS Bedrock) |
| Diagramm erstellen – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| Diagramm bearbeiten – ERD | Claude Sonnet 3.7 (AWS Bedrock) |
| Dokument erstellen | Claude Sonnet 3.7 (AWS Bedrock) |
| Dokument bearbeiten | Claude Sonnet 3.7 (AWS Bedrock) |
| Notizen erstellen | Claude Sonnet 3.7 (AWS Bedrock) |
| Notizen bearbeiten | Claude Sonnet 3.7 (AWS Bedrock) |
| Notizen erfassen | Claude Sonnet 3.7 (AWS Bedrock) + Eigenes Modell von Miro |
| Bild erstellen | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Bild bearbeiten | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Alternativtext für Bild | Claude Sonnet 3.7 (AWS Bedrock) |
| Prototyp erstellen | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Prototyp-Bildschirm bearbeiten | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Bild in Prototyp umwandeln | Claude Sonnet 3.7 + Eigenes Modell von Miro |
| Tabelle erstellen | Claude Sonnet 3.7 (AWS Bedrock) |
| Tabelle bearbeiten | Claude Sonnet 3.7 (AWS Bedrock) |
| Diagramm digitalisieren | Claude Sonnet 3.7 (AWS Bedrock) |
| Sortierung von Notizen nach Schlüsselwörtern | Claude Sonnet 3.7 (AWS Bedrock) + Miro eigenes Modell |
| Sortierung von Notizen nach Meinung | Miro eigenes Modell |
| KI-Kollege | Claude Sonnet 3.7 (AWS Bedrock) |
| KI-gestütztes Textbearbeiten | Claude Sonnet 3.7 (AWS Bedrock) |
| KI-gestützte Mindmaps | Claude Sonnet 3.7 (AWS Bedrock) |

## Eigene Modellwahl

Die folgenden Listen zeigen, welche Modelle verfügbar sind mit [Select Your Own Model](10-select-your-own-model-beta.md), verfügbar für [Flows](04-flows-overview.md) und KI-Kollege.

### Große Sprachmodelle

**Claude**

- Claude 3.7 Sonnet
- Claude Sonnet 4

**OpenAI**

- GPT-4o
- GPT-4o Mini
- OpenAI o4-mini
- GPT-5
- GPT-5 Mini
- GPT-4.1
- GPT-4.1 Mini

### Bildmodelle

**Stability AI**

- Stable Image Core
- Stable Image Ultra
- Stable Diffusion 3.5 Large

**Amazon**

- Amazon Titan Image Generator
- Amazon Nova Canvas

**Google**

- Gemini 2.5 Flash Image (Nano Banana)
- Vertex AI Imagegen 3
- Vertex AI Imagegen 3 Fast
- Vertex AI Imagegen 4

## Miro KI-Credits und Add-on

Miro weist Ihrem Konto jeden Monat eine bestimmte Anzahl von KI-Credits zu. Die Anzahl der zugewiesenen Credits hängt von Ihrem Preisplan ab. Ihre Zuweisung wird am ersten Tag jedes Kalendermonats zurückgesetzt.

Für jede von Ihnen durchgeführte KI-Aktion verbrauchen Sie KI-Credits. Die meisten KI-Aktionen verbrauchen einen (1) Credit pro Aktion, einige Funktionen können jedoch mehr verbrauchen.

Um deine Zuteilung von Miro KI-Credits zu erhöhen, kannst du optional ein Miro KI-Credit-Add-on-Abonnement erwerben. Mehr dazu erfährst du unter [Miro KI-Credits und KI-Add-on](../../plans-billing/billing-and-payments/03-miro-ai-credits.md).

## Datenschutz und Sicherheit bei Miro AI

Ab dem 3. Februar 2025 erfasst Miro KI-Interaktionsdaten von Nutzern des Free-Preisplans, um Miro AI Funktionen wie KI-Zusammenfassungen, Diagramme und KI-Kollegen zu verbessern.

Um mehr darüber zu erfahren, wie Miro KI-Interaktionen nutzt, um Miro AI zu verbessern, und wie du deine Datenpräferenzen steuern kannst, siehe [Qualitätsverbesserungen in Miro AI](19-miro-ai-quality-improvements.md).
