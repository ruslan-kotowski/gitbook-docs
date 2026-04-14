---
title: Miro AI-Moderationslevel festlegen oder aktualisieren (Beta)
article_id: 30613174297618
translation_id: 30613174297618
locale: de
sidebar_position: 3
created_at: '2025-10-29T01:15:35Z'
updated_at: '2026-01-12T11:22:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Mit der Moderation von Miro AI können Unternehmens-Admins die Filterstufen von Prompts anpassen, die potenziell zu schädlichen oder unangemessenen Ausgaben führen könnten. Du kannst die Sensibilität der Miro AI-Moderation in deiner Organisation steuern und in Kategorien wie Hass, sexuelle Inhalte, Gewalt und Selbstverletzung filtern. Dies hilft dir, die Nutzung von Miro AI an die Anforderungen und Richtlinien deiner Organisation sowie an ihre Risikotoleranz anzupassen.

**Hinweis**: Wenn deine Organisation ihren eigenen LLM-Anbieter verbindet (zum Beispiel eine direkte OpenAI-Integration), wird der Moderationsselektor deaktiviert, und jedes zuvor gewählte Level wird für diese Integration ignoriert.

## Voraussetzungen

- Stelle sicher, dass du das Add-on „Enterprise Guard“ hast.
- Stelle sicher, dass du ein **Company Admin** für die Organisation bist, die du konfigurieren möchtest.
- Überprüfe deine Governance- und Richtlinienanforderungen, um ein geeignetes Anfangsniveau zu wählen. Das Standardniveau wird für die meisten Organisationen empfohlen.

## Festlegen oder Aktualisieren des Moderationsniveaus für Miro AI

1. Öffne deine Organisations-**Einstellungen** in Miro.
2. Gehe zu **Miro AI** › **Moderation**.
3. Wähle ein Niveau:
   - **Strikt:** Blockiert alles im Standard sowie Inhalte mit geringem bis mittlerem Risiko (z. B. subtile oder codierte Hassrede, sexuell anzügliche Inhalte, nicht grafische Gewalt, nicht explizite Erwähnungen von Selbstverletzung).
   - **Standard (empfohlen):** Blockiert moderat bis stark schädliche Inhalte (z. B. explizite Hassrede, explizite sexuelle Inhalte, anschauliche Gewalt, Förderung von Selbstverletzung).
   - **Minimal:** Blockiert nur stark schädliche Inhalte.
4. Klicke auf **Bestätigen**.
   Die Änderung wird sofort auf alle in der Organisation angewendet und im Audit-Protokoll erfasst.

## Moderationslevel validieren (optional)

- Bitte eine Pilotgruppe, typische Prompts zu testen und über- oder untergefilterte Inhalte zu melden.
- Beobachte Support- oder Eskalationskanäle auf falsche positive oder nicht erkannte Schäden in der ersten Woche nach einer Änderung.

## Tipps und Best Practices

- Beginne mit **Standard** und passe basierend auf Rückmeldungen der Pilotgruppe und Eskalationsbewertungen an.
- Wenn Nutzer zu viele geblockte Prompts melden, versuche **Standard** (von Streng) oder **Minimal** (von Standard) und veröffentliche Beispiele für akzeptable Prompts.
- Wenn grenzwertige Inhalte durchrutschen, wechsle zu **Streng** und füge interne Richtlinien hinzu, um Reibungsverluste zu minimieren.
- Überprüfe das Niveau nach Policy-, Regulierungs- oder Einsatzbereichsänderungen.

## Fehlerbehebung

**Moderationssteuerung ist deaktiviert**
Eine benutzerdefinierte LLM-Integration ist verbunden. Trenne sie, um den Selektor wieder zu aktivieren. Solange sie verbunden ist, wird die zuvor gewählte Stufe für diese Integration ignoriert.

**Zu viele Fehlalarme**
Überlege, von **Strikt → Standard** zu wechseln und Beispiele für akzeptable Nutzung zu teilen. Überprüfe im Audit-Protokoll die jüngsten Änderungen, um den Zeitpunkt zu bestätigen.

**Gefährdung durch schädliche Inhalte**
Stelle sicher, dass das Niveau nicht **Minimal** ist. Erwäge je nach Risikobereitschaft **Standard** oder **Strikt**.

**Benutzer sind unsicher, warum Prompts blockiert werden**
Veröffentliche interne Richtlinien, die auf dein gewähltes Niveau, Beispiel-Prompts und Eskalationswege hinweisen.
