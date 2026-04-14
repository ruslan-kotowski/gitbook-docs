---
title: Miro AI-Prompting-Leitfaden
article_id: 30226743358226
translation_id: 30226743358226
locale: de
sidebar_position: 1
created_at: '2025-10-14T17:24:22Z'
updated_at: '2025-11-25T15:54:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Bessere Prompts führen zu besseren Ergebnissen, wenn du mit einem beliebigen AI-Modell arbeitest. Ausführlichere Prompts erzeugen in der Regel Ergebnisse, die besser mit deinen Vorstellungen übereinstimmen. Kürzere, weniger detaillierte Prompts geben dem AI-Modell mehr Freiheit, zu interpretieren, was du möchtest, was zu überraschenden Ergebnissen führen kann.

Dieser Prompting-Leitfaden hilft dir dabei, bessere Prompts zu erstellen, wenn du mit den Miro AI-Funktionen arbeitest.

## RISEN Framework

Das RISEN-Framework für AI-Prompting ist ein strukturierter Ansatz, um von Anfang an bessere Ergebnisse zu erzielen. Es beinhaltet:

- **Rolle:** Ist die KI ein Creator, Berater oder Problemlöser? Spielt sie eine bestimmte Rolle in deinem Team? *Beispiele: „Du bist ein Senior-Produktdesigner, der...“ oder „Du bist ein erfahrener technischer Autor, der...“*
- **Eingabe:** Hier gibst du der KI die Informationen, die sie benötigt, um ihre Aufgabe zu erfüllen. In Miro können dies schriftliche Informationen oder Kontext vom Board sein. Zum Beispiel, wenn du ein Prototyp erstellst, könntest du die Funktionen des Produkts oder die einzubeziehenden Seiten angeben.
- **Schritte:** Hier gibst du der KI an, was genau sie tun soll. Während du hier allgemeine Anweisungen geben kannst, führt genauere Vorgaben in der Regel zu besseren Ergebnissen. *Beispiel: „1. Fasse das im Kontext des Boards bereitgestellte Material zusammen. 2. Erstelle eine Notiz für jeden wichtigen Punkt des Materials. 3. Organisiere die Notizen nach ihrer voraussichtlichen Wirkung.“*
- **Erwartung:** Wenn du nicht spezifizierst, was du als Ergebnis erwartest, entscheidet die KI das selbst, was nicht immer richtig ist. Sei hier konkret; anstatt „Erstelle eine Präsentation“ zu sagen, gib an „Erstelle eine Präsentation mit zwölf Folien“ und lege fest, welches Thema jede Folie behandeln soll.
- **Eingrenzen:** Falls es Dinge gibt, die du *nicht* im Output haben möchtest, solltest du das am Ende spezifizieren. Du kannst z. B. einen KI-Prototyp für einen Online-Checkout-Prozess entwerfen, der *keine* Anmeldeseite im Workflow integriert.

Indem du jeden dieser Parameter definierst, weiß Miro AI genau, was du von seinem Output erwartest und erzeugt insgesamt bessere Ergebnisse.

## Kontext von deinem Miro-Board hinzufügen

Eines der stärksten Features von [Miro AI](../01-miro-ai-overview.md) ist die Fähigkeit, Kontext vom aktuellen Board hinzuzufügen. Dies ermöglicht es dir, eine große Menge an Informationen in strukturierter Form einzubinden, um den Output der KI zu verbessern.

Hier einige Tipps, um das Beste aus dem Board-Kontext herauszuholen:

- **Wähle nicht alles auf dem Board aus.** Auch wenn es einfacher erscheint, alles auf dem Board als Kontext auszuwählen, führt eine Fokussierung auf nur die relevantesten Informationen zu den besten Ergebnissen.
- **Füge branchenspezifischen Kontext zum Board hinzu.** Obwohl Miro AI leistungsfähig ist, basiert es ebenso wie die meisten anderen KI-Modelle auf einem allgemeinen großen Sprachmodell (LLM). Das Hinzufügen von branchenspezifischer Dokumentation, die für deinen Prompt relevant ist, hilft dabei, beim ersten Mal bessere Ergebnisse zu erzielen. Dies kann Dinge beinhalten wie ein Glossar von Fachbegriffen, ein Beispiel für ein spezifisches Ergebnis, das du erzeugen möchtest, oder andere branchenspezifische Kenntnisse, die jemand außerhalb deiner Branche wahrscheinlich nicht kennt.
- **Nutze Miro AI, um Kontext zu schaffen.** Wenn du etwas wie ein Produktdesign-Briefing basierend auf Notizen aus einem Meeting benötigst, kannst du Miro AI verwenden, um dies in einem Dokument auf deinem Board zu erstellen. Nimm die nötigen Bearbeitungen vor und nutze dies als Kontext, anstatt verstreute Meeting-Notizen einzubeziehen, die verwirrend sein könnten.

## Miro AI Starter Prompts

Neu bei Miro AI? Kein Problem! Wir haben einsatzbereite Starter Prompts für beliebte Workflows erstellt. Ersetze einfach die variablen Platzhalter (zum Beispiel [Rolle], [Artefakt], [Ton]) durch deinen Kontext und führe dann das Prompt aus. Erkunde unsere Starter Prompts nach Workflow:

- [Starter-Prompts zur Generierung von Inhalten und Ideenfindung](02-content-generation-and-ideation-starter-prompts.md)
- [Starter-Prompts zur Inhaltsanalyse und -organisation](03-content-analysis-and-organization-starter-prompts.md)
- [Starter-Prompts zur Workflow-Optimierung](04-workflow-optimization-starter-prompts.md)

## Feature-spezifische Prompting-Tipps

Miro AI bietet allgemeine und spezialisierte KI-Kollegen, AI-Modus, Workflows und Formatspezifische AI-Tools, um sich besser auf das gewünschte Ergebnis zu konzentrieren. Wenn du beispielsweise versuchst, einen Prototyp zu erstellen, öffne Miro Prototypes, anstatt zu versuchen, einen über den allgemeinen KI-Kollegen zu erstellen.

### Miro Prototypes

[Miro Prototypes](../../miroverse/prototyping/07-miro-prototypes-add-on.md) ermöglichen es dir, mit AI ein- oder mehrseitige Prototyp-Workflows zu erstellen. Befolge diese Tipps, um bessere Prototyping-Ergebnisse zu erzielen:

- Gib die Bildschirme an, die der Prototyp enthalten soll, insbesondere wenn einige außerhalb eines typischen UX-Musters für die Nutzerreise liegen, die du gestaltest.
- Wenn du irgendwelche Produkt- oder Designanforderungen hast (z. B. Hex-Codes für bestimmte Farben), füge diese als Kontext auf deinem Board hinzu.
- Füge Screenshots von ähnlichen Seiten oder Designs hinzu, die du als Inspiration verwenden möchtest, als Kontext auf deinem Board.
- Gib im Prompt Informationen über deinen Zielnutzer an (z. B. "Studierende" oder "Design-Teamleiter").

### Miro-Präsentationen

Nutze die KI, um [Präsentationen](../../formats/02-create-miro-slides-with-ai.md) zu erstellen und deine Präsentationsvorbereitung zu beschleunigen. Befolge diese Tipps, um bessere Foliensätze zu generieren:

- Definiere die Farbpalette oder andere Stilüberlegungen in deinem Prompt. Wenn du eine Farbpalette im Miro-Markencenter angegeben hast, füge diese in deinem Prompt ein.
- Füge Inhalte für bestimmte Folien als Dokumente oder Notizen als Kontext auf dem Board hinzu.
- Gib in deinem Prompt an, wer dein Publikum ist (z.B. „Führungskräfte“ oder „Venture-Capital-Geber“).

### Bilder

Verwende Miro AI, um Bilder auf deinen Boards zu erstellen. Hier sind einige Tipps, um bessere Bilder zu erstellen:

- Gib den Bildstil an (z. B. „fotorealistisch“, „digitale Malerei“, „impressionistisch“).
- Beziehe relevanten Kontext vom Board ein, wie eine Beschreibung, was das Bild enthalten soll (du kannst dies auch im Prompt-Feld einfügen, aber wenn es bereits auf dem Board existiert, nutze es als Kontext).
- Füge alle spezifischen Details hinzu, die das Bild enthalten soll (z. B. „die Person trägt einen Laptop“ oder „ein Stapel Bücher steht auf dem Tisch“).
- Je spezifischer dein Prompt ist, desto besser wird das ursprüngliche Ergebnis.

## Bearbeiten und Iterieren mit Miro AI

Miro AI ist ein Werkzeug zur Unterstützung deiner Arbeit und kein Ersatz für menschliche Einsicht und Wissen. Bearbeitung und Iteration sind ein wichtiger Schritt, um bessere Ergebnisse zu erzielen, sowohl mit KI als auch manuell.

Bei der Erstellung von Formaten mit Miro AI hast du die Möglichkeit, Änderungen vorzunehmen, bevor du die Inhalte zu deinem Board hinzufügst. In Miro Prototypes und Miro-Präsentationen kannst du jeweils einen Bildschirm oder eine Folie bearbeiten, aber so viele Bearbeitungsrunden durchführen, wie du benötigst. Du kannst auch jederzeit zu früheren Versionen zurückkehren, bevor du die Inhalte zum Board hinzufügst.

Hier sind einige Tipps zum Bearbeiten mit Miro AI:

- Spezifiziere jeweils eine Bearbeitung, wenn du Ergebnisse verfeinerst. Zu viele Anweisungen auf einmal einzugeben, kann unerwartete Ergebnisse liefern.
- Konzentriere dich auf den Inhalt, nicht auf den Stil, da du nur einen Bildschirm oder eine Folie auf einmal bearbeiten kannst.
- Versuche andere Formulierungen oder Schlüsselwörter, wenn das Ergebnis nicht deinen Erwartungen entspricht.

Wenn du ein Format erstellt hast, das du weiterentwickeln möchtest, aber bereits auf das Board hinzugefügt hast, kannst du dieses Objekt als Kontext für die nächste Iteration verwenden. Dies ist eine gute Option, wenn du beispielsweise den Stil einer Folienpräsentation ändern oder zusätzliche Bildschirme in einem Prototypen-Workflow hinzufügen möchtest.

:::note
Während die Verwendung von früher durch KI generierten Arbeiten als Kontext für die Iteration neuer Versionen ein guter Ausgangspunkt ist, kann die KI Aspekte der Arbeit basierend auf anderen Promptelementen oder zusätzlichem Kontext ändern. Überprüfe daher alle Ergebnisse genau.
:::
