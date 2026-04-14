---
title: Wähle dein eigenes Modell (Betaversion)
article_id: 29484232754578
translation_id: 29484232754578
locale: de
sidebar_position: 9
created_at: '2025-09-15T12:50:30Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-sidekicks
availability:
  notes: 'Verfügbar für: Teammitglieder Welche Preispläne: Free, Starter, Business,
    Enterprise Welche Plattformen: Browser, Desktop, Mobil'
---

Wenn du KI-Aktionen mit Miro [Flows](04-flows-overview.md) und KI-Kollegen durchführst, ermöglicht dir "Select Your Own Model", das am besten geeignete Large-Language-Modell (LLM) für die Aufgabe festzulegen.

Zum Beispiel kannst du bei der Bildgenerierung entscheiden, ob du Stable Diffusion 3.5 Large oder Gemini 2.5 Flash Image (Nano Banana) verwendest.

Deine Wahl kann von der Komplexität oder Spezifität deiner Aufgabe abhängen.

:::tip
Miro Flows und KI-Kollege beinhalten ein standardmäßig für jede Aufgabe vorausgewähltes LLM. Wenn du unsicher bist, welches Modell du wählen sollst, ist die Verwendung des Standardmodells der beste Start. Das Standardmodell wird mit einem „Empfohlen"-Label angezeigt.
:::

Der Modellselektor ist nur als Teil von Flows und KI-Kollege für Folgendes verfügbar:

- Dokumente und Bildformate in KI-Kollege und Flows
- Hauptlogik von KI-Kollege
- Anweisungsblock in Flows

Dieser Artikel erklärt, wie du dein eigenes Modell für Flows und KI-Kollege auswählst und gibt Informationen, um ein LLM für allgemeine Aufgaben zu wählen.

## Eigenes Modell auswählen

### Flows

Dokumente, Bilder und Anweisungsblöcke in einem Flow haben jeweils ein Eingabefeld, in dem du dein eigenes Modell auswählen kannst.

Gehe dazu wie folgt vor:

1. Füge ein Dokument, ein Bild oder einen Anweisungsblock zum Canvas hinzu.
2. Um die Liste der verfügbaren Modelle zu sehen, klicke oben rechts im Eingabefeld auf den Namen des Standardmodells. Zum Beispiel `AWS | Claude 3.5`.
3. Ein Modell auswählen.

Um mehr über die Erstellung von Flows und die Benutzeroberfläche von Flows zu erfahren, siehe [Flows](05-flows.md).

### KI-Kollege

Beim Erstellen oder Bearbeiten von KI-Kollegen siehst du den Abschnitt **Modell (fortgeschritten)**, und du kannst auswählen, welches Modell du für die Verarbeitung von KI-Kollegen, die Bildgenerierung und die Dokumentenerstellung verwenden möchtest.

Weitere Informationen zu KI-Kollegen findest du in der [Dokumentation zu KI-Kollegen](08-ai-sidekicks.md).

## Wie sich Modelle unterscheiden

Ein großes Sprachmodell (LLM) ist üblicherweise Mitglied einer Modellfamilie, die leistungsstarke, aber ressourcenintensive Modelle, optimale Modelle und die schnellsten, aber weniger leistungsfähigen Modelle umfasst.

Zum Beispiel umfasst die GPT-5-Familie GPT-5, GPT-5-mini und GPT-5-nano.

Die schnellsten, aber am wenigsten leistungsstarken Modelle sind ideal für niedrige Latenzzeiten.

### Gedankenverarbeitung und Nicht-Gedankenverarbeitung

Ein Hauptunterscheidungsmerkmal zwischen LLMs ist das Modell für "Reasoning" gegenüber "Non-reasoning".

*Reasoning* bedeutet, dass das Modell mehr Zeit benötigt, um eine qualitativ hochwertige Antwort zu liefern.

:::note
Reasoningbedeutet nicht immer das genaueste Ergebnis. Wenn viele Iterationen des Outputs erforderlich sind, ist ein hohes Reasoning möglicherweise nicht die effizienteste Wahl.
:::

Für komplexe Aufgaben wie das Erstellen von kundengerichteten Dokumenten, Priorisierungen und Aufgaben, die die Verarbeitung eines großen Informationsvolumens erfordern, ist ein Reasoning-Modell die beste Wahl.

Für einfache Aufgaben wie die Grammatikprüfung, Übersetzungen oder die Umformatierung von Texten ist ein Non-reasoning-Modell die effizienteste Wahl.

Die folgende Tabelle zeigt einige Reasoning und Non-reasoning Modelle.

| Fähigkeit zum logischen Denken | Modelle |
| --- | --- |
| Logisches Denken | GPT-5, GPT-5-mini, GPT-5-nano, Claude Sonnet 4, Claude Sonnet 4.5, Gemini 2.5, Gemini 2.5 Flash, o3, o4-mini |
| Kein logisches Denken | GPT 4o, GPT-4o-mini, GPT-4.1, GPT-4.1-mini, Claude Sonnet 3.7, Claude Sonnet 3.5, Gemini 2.5 Flash Lite |

### Stil

Jedes LLM hat einen einzigartigen "Stil". Wenn du mit verschiedenen Modellen experimentierst, wirst du vielleicht bemerken, dass ein bestimmter Ausgabestil deinen Anforderungen entspricht, sei es für Branding, Stimmung oder Vorlieben.

:::tip
Ältere Modelle haben einen ausgeprägteren Stil, insbesondere für kreative, unkonventionelle Ausgaben.
:::

## Dein KI-Modell nach Aufgabe auswählen

| Aufgabe | Modelle | Beschreibung |
| --- | --- | --- |
| Brainstorming | GPT-4o, o3, o4-mini, Sonnet 3.7 | Ideal für divergentes Denken, Ideenexplosionen für Features, verspielter Ton und "kreative Note." Nutzen Sie es zur Erstellung von Texten, wie zum Beispiel alternativen Überschriften und Mikrotext-Varianten. |
| Priorisierung & Bewertung | GPT-5, Claude Sonnet 4.5, Gemini 2.5 | Die besten Modelle für logisches Denken, für konsistente Bewertungen und klare Begründungen. Zum Beispiel RICE/MoSCoW im Backlog, Trade-off-Diskussionen und Roadmap-Ebenen. |
| Synthese & Forschung | GPT-5, GPT-5-mini, Claude Sonnet 4.5, GPT-4.1, Claude Sonnet 3.7, Gemini 2.5 Flash | Verwendung für durchschnittlich bis hochkomplexe Aufgaben. Zum Beispiel, um Personas aus Notizen zu erstellen und Erkenntnisse aus Datenbanken und Wissensbasen abzuleiten. |
| Schema & Transformation | GPT-5-mini, GPT-5-nano, GPT-4.1, Sonnet 3.7, Gemini 2.5 Flash, Gemini 2.5 Flash Lite | Formatänderungen erfordern in der Regel kein komplexes logisches Denken, daher liefern optimierte Versionen schneller Ergebnisse. Bleibe jedoch bei späteren Modellen, um Konsistenz bei großen Kontexten sicherzustellen (Notizen → Dokumente, Dokumente → Tabelle, Spezifikation → Diagramm) |
| Schnelle Textbearbeitungen | GPT-4o-mini, Gemini 2.5 Flash Lite, GPT-5-nano, Claude 3.7 | Die schnellsten Optionen. Am besten geeignet für einfache Textbearbeitungen, wie Grammatik, Übersetzungen und Umschreibungen zur besseren Verständlichkeit. |

## Modelle zur Bilderstellung wählen

Alle von Miro unterstützten großen Sprachmodelle (LLM) können Text und Bilder verarbeiten. Allerdings können die meisten keine Bilder erstellen.

Für die Bilderstellung ist Gemini 2.5 Flash Image (Nano Banana) außergewöhnlich gut darin, Ihre allgemeinen Anweisungen in ein Bild umzuwandeln.

Die meisten LLMs erwarten eine Bildbeschreibung und keine spezifischen Anweisungen. Zum Beispiel "ein Gemälde eines Hundes in einem lustigen Hut" als Beschreibung, im Gegensatz zu "ein lustiges Bild von einem Hund erstellen" als Anweisung. Nano Banana kann Bilder auf Basis spezifischer Anweisungen erstellen.

:::note
Verwenden Sie Nano Banana für gezielte Bearbeitungen an einem bestehenden Bild. Andere Modelle können ein bestehendes Bild als Stilreferenz verwenden.
:::

Hinsichtlich der Geschwindigkeit oder der Ausgabequalität gibt es kaum Unterschiede zwischen den LLMs. Wie bei jedem Anwendungsbeispiel kannst du mit verschiedenen Modellen experimentieren, um herauszufinden, welches am besten deinen Vorlieben entspricht.
