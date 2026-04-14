---
title: "\xDCbersicht"
article_id: 30969987585938
translation_id: 30969987585938
locale: de
sidebar_position: 1
created_at: '2025-11-11T12:42:45Z'
updated_at: '2026-01-12T16:04:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Bei unserem Event Canvas 25 haben wir den KI-Workspace für Innovation vorgestellt, der visuelle KI-Workflows und kollaborative KI-Assistenten auf dem Canvas bietet. Zusätzlich zu den Endnutzer-Features führen wir neue Admin-Funktionen ein, die dir mehr Übersicht, intelligentere Steuerungsmöglichkeiten und nahtlose Wege bieten, die neuesten KI-Tools von Miro für deine Teams verfügbar zu machen.

Nutze diese Seite, um die für Admins auf der Enterprise-Stufe verfügbaren KI-Admin-Funktionen zu erkunden. Jeder Abschnitt beginnt mit einem kurzen Überblick und wird durch erweiterbare FAQs ergänzt, die verschiedene Aspekte jeder Funktion abdecken.

- [Miro KI-Admin-Kontrollen:](01-overview.md) entscheiden Sie, welche KI-Funktionen in Ihrer Organisation verfügbar sind, und verwalten Sie, wer sie nutzen kann.
- KI-Moderation: legen Sie organisationsweite Filterstufen (Strikt, Standard, Minimal) fest, um Eingaben zu überprüfen, die zu schädlichen oder unangemessenen Inhalten führen könnten.
- Admin-Analysen: nutzen Sie Dashboards im Produkt (Übersicht und Miro KI), um die Einführung zu verfolgen und die Aktivität der Organisation, Lizenzzuweisung, Vorlagenverwendung und die Nutzung von Miro KI in Ihrer Organisation zu verstehen.

:::note
Während der Betaversion von AI Workflows standen AI Custom Terms of Service und die granularen Admin-Steuerelemente von Miro AI den Kunden von AI Workflows zur Verfügung. Mit der nun allgemeinen Verfügbarkeit von AI Workflows sind diese Funktionen nur noch als Teil von Enterprise Guard verfügbar. Weitere Informationen findest du unter [Erweiterte KI-Verwaltung mit Enterprise Guard](01-overview.md).
:::

## Miro AI-Admin-Steuerelemente

Die Miro AI-Admin-Steuerelemente helfen dir dabei zu entscheiden, welche KI-Funktionen in deiner Organisation verfügbar sind und wer sie nutzen kann. Weitere Informationen findest du in der [Dokumentation zu den Miro AI-Admin-Steuerelementen](../managing-enterprise-teams-and-content/01-miro-ai-admin-controls.md).

**Zweck und Geltungsbereich**

**Was sind Miro KI Admin-Kontrollen?**

Miro KI Admin-Kontrollen ermöglichen es Admins, den Zugriff auf Miro KI-Funktionen innerhalb der Organisation zu verwalten. Abhängig von Ihrer Konfiguration können Sie den Zugriff für alle aktivieren, den Zugriff auf bestimmte Teams einschränken oder den Zugriff deaktivieren.

**Was ist der Unterschied zwischen einer KI-Kapazität und einem KI-Feature?**

Eine **Kapazität** ist eine Kategorie von KI-Funktionalität (z. B. Inhalte erstellen, mit Bildern arbeiten oder Aktivitäten zusammenfassen). Ein **Feature** ist eine spezifische Aktion innerhalb einer Kapazität (z. B. *Notizen erstellen* oder *Hintergrund entfernen*).

Feature-Level-Kontrollen (Verwaltung einzelner Features innerhalb einer Kapazität) sind über [Enterprise Guard](01-overview.md) verfügbar.

**Zugang und Voraussetzungen**

**Wo verwalte ich die Miro KI-Admin-Kontrollen?**

In der Admin-Konsole, gehe zu **Miro KI** > **Funktionen**. Von dort aus kannst du den Zugriff auf jede KI-Fähigkeit (und, falls verfügbar, einzelne KI-Features) aktivieren, einschränken oder entfernen.

**Wer kann diese Einstellungen konfigurieren?**

Unternehmens-Admins können in der Admin-Konsole den Zugang zu Miro KI verwalten (die Verfügbarkeit von KI-Features hängt von deinem Preisplan und den aktivierten Add-ons ab).

**Zugriffsoptionen und Verhalten**

**Was bedeuten die Zugriffsoptionen (Jeder, Niemand, Bestimmte Teams)?**

Verwende das Dropdown-Menü neben einer Fähigkeit (oder Funktion, sofern verfügbar), um auszuwählen, wie der Zugriff gewährt wird.

| Option | Funktion | Wann verwenden |
| --- | --- | --- |
| **Jeder** | Ermöglicht den Zugriff für alle Nutzer und Teams in Ihrer Organisation (einschließlich später erstellter Teams). Alle restriktiven Team-Einstellungen werden überschrieben. | Standardausrollung in der gesamten Organisation. |
| **Niemand** | Entfernt den Zugriff für alle. Sie werden zur Bestätigung der Entfernung aufgefordert. | Umfassende Sperrung der Nutzung in der gesamten Organisation. |
| **Bestimmte Teams** | Ermöglicht den Zugriff nur für die von Ihnen ausgewählten Teams. | Pilotphase mit einer Teilmenge von Teams oder schrittweise Einführung. |

**Was passiert, wenn ich eine Funktion deaktiviere?**

Wenn eine Funktion deaktiviert wird, können Nutzer nicht mehr auf diese Funktion und die zugehörigen Features auf den Boards zugreifen. Wenn alle Miro KI-Funktionen deaktiviert sind, erscheint **Erstellen mit KI** als deaktiviert auf dem Board.

**Gelten diese Einstellungen für später erstellte Teams?**

Wenn du eine Funktion auf **Jeder** setzt, gilt sie für deine Organisation, einschließlich später erstellter Teams. Wenn du **Bestimmte Teams** wählst, musst du die Auswahl aktualisieren, wenn neue Teams erstellt werden (wenn du sie einbeziehen möchtest).

**Enterprise Guard und Kontrolle auf Feature-Ebene**

**Wie ändert Enterprise Guard, was ich kontrollieren kann?**

Mit [Enterprise Guard](01-overview.md) kannst du den Zugriff auf der **Feature-Ebene** innerhalb jeder Fähigkeit verwalten (nicht nur auf der Kategorie-Ebene). Dadurch kannst du einige Features erlauben, während du andere innerhalb derselben Fähigkeit einschränkst.

Beispiel: Du kannst *Bilder erstellen* erlauben und *Hintergrund entfernen* (innerhalb der Bilder-Funktion) einschränken.

**Sichtbarkeit und Verfügbarkeit**

**Warum sehe ich keine Einstellungen für Flows, KI-Kollege oder Prototyping?**

Einige Funktionen (wie **Flows**, **KI-Kollege** und **Prototyping**) sind nur sichtbar und verwaltbar, wenn sie für Ihre Organisation aktiviert sind.

**Kann ich sehen, welches KI-Modell eine Funktion antreibt?**

Ja. In der Admin-Konsole > **Miro AI** > **Funktionen** können Admins die Modelle einsehen, die jede KI-Funktion antreiben.

**Können Gäste oder Besucher Miro AI nutzen, wenn ich es aktiviere?**

Miro AI ist für **Mitglieder** verfügbar. Gäste und Besucher können Miro AI nicht verwenden.

**Fehlerbehebung und bewährte Praktiken**

**Ich habe die Zugriffseinstellungen geändert, aber die Nutzer sehen weiterhin Miro AI. Was sollte ich überprüfen?**

- **Geltungsbereich bestätigen:** Stelle sicher, dass du die richtige Fähigkeit (oder die spezifische Funktion, falls kontrolle auf Funktionsebene gilt) aktualisiert hast.
- **Teamausrichtung überprüfen:** Wenn auf *Bestimmte Teams* eingestellt, bestätige, dass das Team des Nutzers ausgewählt ist.
- **Ausbreitungszeit zulassen:** In einigen Fällen kann es kurz dauern, bis Änderungen auf alle Sitzungen angewendet werden.
- **Sitzung aktualisieren:** Bitte den Nutzer, den Browser-Tab zu aktualisieren, sich ab- und wieder anzumelden oder die Desktop-App neu zu starten (falls zutreffend).

## Miro AI Moderation

Mit der Miro AI-Moderation können Unternehmens-Admins Filterstufen anpassen, die Eingaben filtern, die potenziell schädliche oder unangemessene Inhalte enthalten könnten. Du kannst die organisationsweite Empfindlichkeit der Miro AI-Moderation einstellen, um Inhalte wie Hass, sexuelle Inhalte, Gewalt und Selbstverletzung herauszufiltern. Dies hilft dir, die Nutzung von Miro AI mit den Anforderungen, Richtlinien und Risikobereitschaft deiner Organisation in Einklang zu bringen. Weitere Informationen findest du in der [Dokumentation zur Miro AI-Moderation](../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Zweck und Geltungsbereich**

**Was ist die KI-Moderation in Miro?**

Die KI-Moderation ermöglicht es Unternehmens-Admins, ein organisationsweites Filterlevel (Streng, Standard oder Minimal) festzulegen, das Eingaben filtert, die zu schädlichen oder unangemessenen Ausgaben führen könnten (z. B. Hass, sexuelle Inhalte, Gewalt, Selbstverletzung).

**Wer kann es konfigurieren und in welchen Preisplänen?**

Unternehmens-Admins im Enterprise-Preisplan mit dem Miro AI Workflows-Add-on können die Einstellung in den Unternehmens-Einstellungen konfigurieren.

**Funktioniert es, wenn mein Unternehmen sein eigenes LLM (z. B. eine direkte Anbieterintegration) verbindet?**

Wenn ein benutzerdefiniertes LLM verbunden ist, könnte der Moderationsselektor für diese Integration deaktiviert sein und alle zuvor gewählten Level werden nicht darauf angewendet.

**Zugang und Voraussetzungen**

**Wer kann es aktivieren und was wird benötigt?**

Company Admins mit dem Miro AI Workflows Add-on im Enterprise Preisplan können AI Moderation in den Organisationseinstellungen konfigurieren.

**Wie schalte ich es ein?**

Gehe zu Einstellungen → Miro AI → Moderation, wähle Strikt/Standard/Minimal und klicke dann auf **Änderungen speichern**. Die Durchsetzung erfolgt sofort für die gesamte Organisation.

**Stufen und Verhalten**

**Was bedeuten die Stufen?**

- **Strikt:** Blockiert Standard + Inhalte mit geringem bis mittlerem Risiko (z. B. unterschwelliger/verschlüsselter Hass, anstößiger sexueller Inhalt, nicht-grafische Gewalt, nicht-explizite Erwähnungen von Selbstverletzung).
- **Standard (empfohlen):** Blockiert Inhalte mit mittlerem bis schwerem Schadenspotenzial.
- **Minimal:** Blockiert nur Inhalte mit schwerem Schadenspotenzial.

**Wann treten die Änderungen in Kraft?**

Sofort für die gesamte Organisation.

**Werden Änderungen protokolliert?**

Ja. Änderungen werden im Audit-Trail Ihrer Organisation aufgezeichnet.

**Einrichtung und Konfiguration**

**Wo stelle ich das Moderationslevel ein oder aktualisiere es?**

Gehe zu Einstellungen → Miro AI → Moderation, wähle Strikt/Standard/Minimal, und klicke dann auf **Änderungen speichern**.

**Welches Startlevel empfehlen Sie?**

Standard ist für die meisten Organisationen geeignet; passe es basierend auf Pilotfeedback und Risikotoleranz an.

**Interaktionen mit anderen Steuerungen**

**Wie steht die KI-Moderation im Verhältnis zu Vorgaben und Promptsteuerungen?**

- **Intelligente Vorgaben:** Wenn ein Board durch die „Blockiere Miro KI-Nutzung“-Vorgabe abgedeckt ist, wird die KI unabhängig vom Moderationsniveau deaktiviert.
- **Prompt-Blockierung:** Funktioniert zusammen mit der Moderation. Die Prompt-Blockierung stoppt sensitive Prompts bei der Eingabe; Moderation filtert schädliche Kategorien.
- **Granulare Admin-Steuerungen:** Feature-Schalter regeln, wer auf KI-Funktionen zugreifen kann, wenn die KI verfügbar ist.

**Fehlerbehebung und Best Practices**

**Wir sehen zu viele Fehlalarme.**

Erwäge, von Strikt → Standard (oder Standard → Minimal) zu wechseln und Beispiele für akzeptable Nutzung zu veröffentlichen. Wenn die Probleme nach der Anpassung der Einstellungen bestehen bleiben, kontaktiere deinen Miro Customer Success Manager, um dies zu melden, damit unser Produktteam eine Überprüfung durchführen kann.

**Wir sehen, dass schädliche Inhalte durchrutschen.**

Wechsle zu Standard oder Strikt und gebe interne Anleitungen. Überprüfe dies nach Richtlinien-/Regulierungsaktualisierungen erneut. Wenn die Probleme nach diesen Änderungen weiterhin bestehen, kontaktiere deinen Miro Customer Success Manager, um dies zu melden, damit unser Produktteam eine Überprüfung durchführen kann.

## Admin-Analysen

Admin-Analysen bieten Unternehmens-Admins datengestützte, umsetzbare Einblicke in die Einführung, Nutzung und Verwaltung von Miro im großen Maßstab. Es umfasst zwei Dashboards: **Übersicht** und **Miro AI**. Weitere Informationen finden Sie unter [Analysen-Übersicht](../getting-started/admin-analytics/01-analytics-overview.md), [Übersichts-Dashboard](../getting-started/admin-analytics/02-overview-dashboard.md) und [Miro AI-Dashboard](../getting-started/admin-analytics/03-miro-ai-dashboard.md).

**Zweck und Geltungsbereich**

**Was sind Admin-Analysen?**

Admin-Analysen bieten vertrauenswürdige Kennzahlen innerhalb des Produkts, um dir zu helfen, zu verstehen, wie Miro genutzt wird, deine Organisation zu verwalten, die Einführung voranzutreiben und die Sicherheits- und Compliance-Anforderungen zu unterstützen.

**Welche Dashboards sind enthalten?**

Admin-Analysen umfassen zwei Dashboards: **Übersicht** (Aktivitäten und Einführung in der Organisation über Boards, Nutzer, Teams, Lizenzen und Vorlagen hinweg) und **Miro AI** (Einführung und Nutzung von Miro AI in der Organisation).

**Dashboards und Navigation**

**Wie wechsle ich zwischen den Dashboards?**

Verwenden Sie die Tabs oben auf der Analysen-Seite, um zwischen **Übersicht** und **Miro AI** zu wechseln.

**Wie ändere ich den Zeitraum?**

Verwenden Sie den **Zeitraum-Auswahlschalter** oben rechts auf der Analysen-Seite, um den angezeigten Zeitraum anzupassen (**täglich**, **wöchentlich**, **monatlich** oder **vierteljährlich**).

**Wann werden die Daten aktualisiert?**

Die Metriken werden **täglich** aktualisiert. Jedes Dashboard zeigt einen **Zuletzt aktualisiert**-Zeitstempel an.

**Übersichts-Dashboard**

**Was kann ich im Übersichts-Dashboard verfolgen?**

Das Übersichts-Dashboard hilft dir dabei, die Akzeptanz zu verfolgen und die Aktivität in der Organisation anhand dieser Kennzahlen-Gruppen zu verstehen:

- **Boards:** Board-Gesamtsummen, aktive Boards und bisherige Trends.
- **Nutzer:** Aktive Nutzertrends. Du kannst auch nach Rolle verfolgen, wie Mitglieder, Unternehmens-Admins, Gäste oder Gäste des Teams.
- **Teams:** Team-Anzahlen und Aktivitätslevel.
- **Lizenzen:** Zuweisung von Lizenztypen und wie sich die Zuweisung im Laufe der Zeit ändert.
- **Vorlagen:** Welche Vorlagen in deiner Organisation am häufigsten genutzt werden.

**Wie sollte ich verlaufsbezogene Diagramme interpretieren?**

- In Widgets, die verlaufsbezogene Daten anzeigen, repräsentieren Werte die Daten vom **letzten Tag jedes Zeitraums**.
- Der **laufende Zeitraum** wird in verlaufsbezogenen Diagrammen nicht angezeigt.
- Verlaufsbezogene Daten sind für bis zu **ein Jahr** verfügbar oder solange die Daten vorhanden sind.

**Miro AI-Dashboard**

**Was kann ich im Miro AI-Dashboard verfolgen?**

Das Miro AI-Dashboard hilft dir, die Akzeptanz zu verfolgen und zu verstehen, wie Miro AI in deiner Organisation genutzt wird, durch diese Kennzahlen:

- **Teams, die KI nutzen:** Teams, die aktiv KI-Funktionen nutzen, einschließlich der Gesamtzahl der Teams, die KI nutzen versus nicht nutzen. Du kannst die Nutzung nach Einsatzbereich filtern.
- **Personen, die KI nutzen:** Gesamtsummen der Akzeptanz für Personen, die KI nutzen versus nicht nutzen, mit monatlichem Verlaufsverlauf.
- **KI nach Einsatzbereich:** Nutzung im Zeitverlauf aufgeteilt in **KI-Erstellung** und **KI-Automatisierung**.
- **KI-Kollege-Zusammenarbeit:** wie häufig Teams über Chat-Sitzungen (Prompts, Nachfragen und Antworten) mit KI-Kollegen interagieren. Analysen zeigen die Anzahl der gestarteten Sitzungen an.
- **Ausgeführte KI-Flows:** wie oft Nutzer einen KI-Flow mit mindestens zwei aufeinanderfolgenden Schritten oder Knoten ausgeführt haben. Die Ausführung wird zum Zeitpunkt des ersten mit dem Flow verknüpften Ereignisses gezählt.

**Wie werden KI-Anwendungsbeispiele definiert?**

- **KI-Erstellung:** Aktionen wie das Erstellen aus Prompts und das Erstellen aus visuellem Kontext.
- **KI-Automatisierung:** Aktionen wie Verfeinerung über Chat oder Kontextmenü, Textbearbeitung, Sortierung und das Entfernen von Bildhintergründen.

**Sind KI-Credit-Nutzung und KI-Nutzungsmetriken gleichzusetzen?**

Nein. **KI-Credits stehen nicht direkt in Zusammenhang** mit den im Dashboard angezeigten KI-Nutzungskennzahlen.

**Datenüberlegungen**

**Warum sehe ich nur teilweise Daten?**

Wenn eine Funktion für einen Teil des ausgewählten Zeitraums deaktiviert war, können im Kennzahlenverlauf teilweise Daten angezeigt werden (zum Beispiel, wenn eine Funktion mitten im Monat aktiviert wurde).

**Warum zeigen Diagramme für einen Zeitraum keine Daten an?**

Wenn in einem bestimmten Zeitraum (Tag, Woche oder Monat) keine Aktivität aufgezeichnet wurde, zeigt das Diagramm für diesen Zeitraum keine Daten an.

**Ältere Daten scheinen zu fehlen. Was soll ich tun?**

Historische Daten sind für bis zu ein Jahr oder so weit zurück, wie die Daten existieren, verfügbar. Wenn ältere Daten zu fehlen scheinen, wenden Sie sich an den Miro Support, um eine Backfill-Verifizierung anzufordern.

**Fehlerbehebung und bewährte Verfahren**

**Unsere Zahlen sind niedriger als erwartet. Was sollte ich überprüfen?**

- Bestätige den **Zeitraum** und den Periodentyp (täglich, wöchentlich, monatlich, vierteljährlich).
- Denke daran, dass **historische Diagramme abgeschlossene Perioden** anzeigen, nicht die aktuell laufende Periode.
- Wenn eine Funktion mitten in einer Periode aktiviert wurde, sind **teilweise Daten** für diesen Zeitraum zu erwarten.

**Wie nutze ich diese Erkenntnisse effektiv?**

Nutze die Übersichtskennzahlen, um Teams, Vorlagen oder Lizenztrends auszumachen, die untergenutzt sind, und führe dann gezielte Maßnahmen zur Aktivierung durch. Verwende die Miro KI-Kennzahlen, um zu identifizieren, wo die KI-Annahme wächst, Unterstützer zu fördern und einen verantwortungsvollen Rollout zu leiten.

## Erweiterte KI-Governance mit Enterprise Guard

Enterprise Guard bietet zusätzliche erweiterte KI-Governance-Funktionen für Enterprise-Admins. Nutze diese Kontrollen, um den Zugriff feinabzustimmen, sensible Informationen zu schützen und die Überwachung und Compliance für die KI-Nutzung in Miro zu verstärken. Weitere Informationen findest du unter [Enterprise Guard KI-Sicherheitsfunktionen und FAQs](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md).

- [Detailierte Miro AI Admin-Kontrollen](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): Lege den Funktionszugriff auf (Alle/Keiner/Bestimmte Teams) innerhalb jeder Funktionskategorie fest.
- [Blockiere die Nutzung von Miro AI mit intelligenten Vorgaben](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): Verwende intelligente Vorgaben, um alle KI-gestützten Interaktionen in Miro zu blockieren, wenn du sensible oder vertrauliche Daten schützen musst.
- [Prompt-Blockierung](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): blockiere Prompts, die sensible Daten oder Quellcode enthalten, zum Zeitpunkt der Übermittlung; zeige stattdessen eine Richtliniennachricht an, anstatt sie an ein LLM zu senden.
- [Enterprise Guard und Microsoft Purview DSPM für KI-Integration](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md): leite Prompts und Antworten zur zentralen Überwachung, Prüfung und Steuerung an Purview weiter.
