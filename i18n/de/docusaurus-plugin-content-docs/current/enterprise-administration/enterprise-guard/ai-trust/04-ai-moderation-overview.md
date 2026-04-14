---
title: "\xDCberblick \xFCber die KI-Moderation (Beta)"
article_id: 29491049430674
translation_id: 29491049430674
locale: de
sidebar_position: 2
created_at: '2025-09-15T16:27:59Z'
updated_at: '2026-01-12T11:21:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Mit der Miro KI-Moderation können Unternehmens-Admins Anpassungen an den Filterstufen von Eingabeaufforderungen vornehmen, die potenziell schädliche oder unangemessene Texte enthalten könnten. Du kannst die Miro KI-Moderationsempfindlichkeit organisationsweit einstellen, um Inhalte wie Hass, sexuelle Inhalte, Gewalt und Selbstverletzung zu filtern. Dies hilft dabei, die Nutzung von Miro AI an die Anforderungen, Richtlinien und Risikotoleranz deiner Organisation anzupassen.

:::note
*Wenn Ihre Organisation ihren eigenen LLM-Anbieter anschließt (beispielsweise eine direkte OpenAI-Integration), wird der Moderationsselektor deaktiviert und alle zuvor gewählten Stufen werden für diese Integration ignoriert.*
:::

## Moderationsstufen

Steuere Miro AI-Inhalte in deinem Unternehmen mit Miro AI-Moderation. Lege die Filterstufe auf Strikt, Standard oder Minimal fest, um zu bestimmen, welche Eingabeaufforderungen blockiert werden. Überprüfe die Tabelle unten, um die Stufen schnell zu vergleichen, und gehe dann zu den detaillierten Abschnitten für weitere Anleitungen.

| Stufe | Was es bewirkt | Am besten für | Kompromisse |
| --- | --- | --- | --- |
| Streng | Blockiert Angebote  mit geringem bis  mäßigem Risiko. | Stark regulierte Organisationen,  Bildungsinstitutionen. | Mehr falsch-positive Ergebnisse;  mögliches Überfiltern. |
| Standard (empfohlen) | Blockiert moderat bis stark schädliche Inhalte. | Die meisten geschäftlichen Anwendungsfälle. | Einige grenzwertige Inhalte könnten durchkommen. |
| Minimal | Blockiert nur stark schädliche Inhalte. | Kreative/Spiele-/Medien- Kontexte. | Mehr Aussetzung gegenüber geringem bis mittlerem Schaden. |

:::note
*Der Standardmodus wird für die meisten Organisationen empfohlen. Er filtert Inhalte, die die meisten Menschen für unangemessen oder schädlich halten, und erhält dabei eine breite Nutzungsmöglichkeit.*
:::

## Strikte Ebene

### Was es filtert

Alles im Standard, plus Inhalte mit niedrigem bis mittlerem Risiko (z. B. subtile oder codierte Hassrede, sexuell anzügliche Inhalte, nicht-graphische Gewalt oder nicht-explizite Erwähnungen von Selbstverletzung).

### Wann verwenden

- Regulierte Branchen oder risikoscheue Unternehmensrichtlinien
- Bildung oder Programme für junge Menschen
- Pilotprojekte mit geringer Risikotoleranz

### Kompromisse

- Mehr falsch-positive Erkennungen und blockierte Inhalte an der Grenze zur Zulässigkeit
- Erfordert Leitlinien zur Verringerung der Benutzerkonflikte

## Standardlevel (empfohlen)

### Was es filtert

Mäßig bis stark schädliche Inhalte (explizite Hassrede, explizite sexuelle Inhalte, grafische Gewalt, Aufrufe zur Selbstverletzung).

### Wann zu verwenden

- Die meisten Organisationen, die ein Gleichgewicht zwischen Sicherheit und Nutzbarkeit suchen

### Kompromisse

- Kontextuelle/grenzwertige Prompts können passieren

## Minimales Level

### Was es filtert

Nur stark schädliche Inhalte.

### Wann zu verwenden

- Kreative Teams, die einen breiteren Ausdruck benötigen (Gaming, Medien)
- Interne Ideenfindung mit klaren Eskalationswegen

### Kompromisse

- Höhere Exposition gegenüber gering bis mäßig schädlichen Inhalten in den Ausgaben

## Überwachung und Compliance

Änderungen des Moderationslevels werden im Audit-Protokoll der Organisation erfasst, einschließlich des vorherigen Wertes, des neuen Wertes, wer die Änderung vorgenommen hat und wann sie sich verändert hat. Weitere Informationen finden Sie in unserer Dokumentation zu [Audit-Protokolle](../security-management/01-audit-logs.md).

## Best Practices

- Starte mit "Default" und passe die Einstellungen basierend auf Pilotfeedback und Eskalationsüberprüfungen an.
- Kombiniere "Strict" mit klaren internen Anweisungen zu akzeptablen Prompts, um Fehlalarme zu reduzieren.
- Wenn du "Minimal" benötigst, lege fest, wann Teams problematische Ausgaben eskalieren oder melden sollen.
- Überprüfe deine Einstellungen nach größeren politischen oder regulatorischen Änderungen erneut.

- KI-Moderation im Überblick
- Moderationsebenen
- Strikte Ebene
- Standardebene (empfohlen)
- Minimale Ebene
- Auditing und Compliance
- Best Practices
