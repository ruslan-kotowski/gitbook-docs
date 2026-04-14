---
title: "KI-Sicherheitsfunktionen und h\xE4ufige Fragen"
article_id: 30943405232914
translation_id: 30943405232914
locale: de
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:34:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Bei unserem Event Canvas 25 haben wir den KI-Workspace für Innovation vorgestellt, der visuelle KI-Workflows und kollaborative KI-Agenten auf dem Canvas bietet. Zusätzlich zu den Endnutzer-Features führen wir neue Admin-Funktionen ein, die dir mehr Übersicht, intelligentere Steuerungsmöglichkeiten und nahtlose Wege bieten, die neuesten KI-Tools von Miro für deine Teams verfügbar zu machen.

Nutze diese Seite, um die mit dem Enterprise Guard Add-on verfügbaren KI-Sicherheitsfunktionen zu erkunden. Jeder Abschnitt beginnt mit einem kurzen Überblick, gefolgt von erweiterbaren häufigen Fragen, die verschiedene Aspekte jeder Funktion abdecken.

- Granulare Miro AI Admin-Kontrollen: Setze den Funktionszugriff (Jeder/Keiner/Spezifische Teams) innerhalb jeder Funktionskategorie fest.
- [Nutzung von Miro AI mit Vorgaben blockieren](#h_block_ai_with_guardrails): Verwende Vorgaben, um alle KI-gestützten Interaktionen in Miro zu blockieren, wenn du sensible oder vertrauliche Daten schützen musst.
- [Admin-Analysen-Dashboard](#h_admin_analytics_overview): Verfolge Boards, Nutzer, Teams, Lizenzen und Vorlagen mit verlaufsbezogenen Trends und täglicher Aktualisierung.
- KI-Moderation (auch in der Enterprise-Stufe verfügbar): Lege organisationsweite Filterstufen (Strikt, Standard, Minimal) fest, um Prompts zu überprüfen, die zu schädlichen oder unangemessenen Inhalten führen könnten.
- Prompt-Sperrung: Sperre Prompts, die sensible Daten oder Quellcode enthalten, zum Zeitpunkt der Einreichung; zeige stattdessen eine Richtliniennachricht an, anstatt sie an ein LLM zu senden.
- Enterprise Guard und Microsoft Purview DSPM für KI-Integration: Leite Prompts und Antworten zur zentralen Überwachung, Prüfung und Steuerung an Purview weiter.

## Granulare Admin-Kontrollen von Miro AI für das Enterprise Guard-Add-on

Miro AI-Admin-Kontrollen ermöglichen es Unternehmens-Admins, zu entscheiden, welche KI-Funktionen in ihrer Organisation verfügbar sind, und zu verwalten, wer sie nutzen kann. Admins können sich auch die Modelle ansehen, die jede KI-Funktion unterstützen. Mit dem Enterprise Guard Add-on erstrecken sich die Miro AI-Kontrollen auf die Funktionsebene innerhalb jeder Funktionskategorie, was hilft, Funktionen basierend auf den organisatorischen Bedürfnissen und Sicherheitsanforderungen zu priorisieren. Neben der vollständigen Miro AI-Funktionskategorie können Admins auch spezifische Miro AI-Funktionen aktivieren, einschränken oder entfernen. Zum Beispiel kann innerhalb der Kategorie Bilder die Option „Bilder mit KI erstellen“ aktiviert und „Hintergrund entfernen“ deaktiviert werden. Verwende diese Kontrollen, um KI sicher einzuführen und Sicherheitsanforderungen zu erfüllen, während du die Einführung von KI-Funktionen förderst. Für mehr Informationen siehe die [Miro AI granular admin controls documentation](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Zweck und Geltungsbereich**

**Was ist granulare Kontrolle für Miro AI?**

Mit dem Enterprise Guard Add-on können Unternehmens-Admins den Zugriff auf einzelne KI-Funktionen innerhalb jeder Funktionskategorie aktivieren, einschränken oder entfernen. Damit kannst du genau auswählen, welche Funktionen die Teams nutzen dürfen.

**Warum granulare Kontrollen verwenden?**

Um die Einführung mit der Sicherheit in Einklang zu bringen. Zum Beispiel kannst du innerhalb der Kategorie Bilder die Erstellung von Bildern zulassen, während du das Entfernen von Hintergründen deaktivierst.

**Zugang und Voraussetzungen**

**Wer kann granulare Kontrollmöglichkeiten konfigurieren und in welchen Preisplänen?**

Unternehmens-Admins mit Enterprise-Plänen und dem Enterprise Guard Add-on, im Browser.

**Wo verwalte ich den Zugriff auf Funktionsebene?**

Admin-Konsole → Miro AI → Fähigkeiten. Erweitere eine Fähigkeit, um den Zugriff für ihre einzelnen Funktionen zu sehen und festzulegen.

**Kontrollen und Verhalten**

**Detaillierte Kontrollen: Was ist der Unterschied zwischen Steuerung auf Fähigkeits- und Funktionsebene und was passiert, wenn ich diese ein- oder ausschalte?**

- **Fähigkeitsebene:** Jeder, Niemand oder Bestimmte Teams gelten für die gesamte Kategorie. Wenn du eine Fähigkeit deaktivierst, verlieren Nutzer den Zugang zu dieser Fähigkeit und allen zugehörigen Funktionen auf den Boards. Wenn du alle Fähigkeiten deaktivierst, erscheint „KI nutzen“ als deaktiviert auf dem Board.
- **Funktionsebene:** Mit Enterprise Guard kannst du für jede Funktion „Jeder“, „Niemand“ oder „Bestimmte Teams“ einstellen. Wenn eine Funktion deaktiviert wird, wird nur der Zugang zu dieser Funktion entfernt; andere Funktionen in derselben Fähigkeit bleiben verfügbar, wenn sie aktiviert sind.

**Welche Zugriffsoptionen gibt es auf Funktionsebene?**

Für jede Funktion wähle zwischen Jeder, Niemand oder Bestimmte Teams. Jeder aktiviert die Funktion organisationsweit und übersteuert teambezogene Einschränkungen. Niemand entfernt den Zugriff für alle Nutzer. Bestimmte Teams richtet sich nur an ausgewählte Teams.

**Was passiert, wenn ich eine einzelne Funktion deaktiviere?**

Nutzer können auf diese Funktion auf keinem Board zugreifen, aber andere Funktionen in derselben Kategorie bleiben verfügbar, wenn sie aktiviert sind.

**Referenz und Beispiele**

**Welche Funktionen kann ich individuell steuern?**

Sieh dir die In-Produkt-Referenz für die aktuelle Liste an. Beispiele im Bereich Inhalt erstellen umfassen Notizen erstellen, Notizen clustern, Dokumente, Tabellen und Diagramme erstellen und bearbeiten sowie Textoperationen wie umschreiben, verkürzen, Ton anpassen und übersetzen. Im Bereich Bilder gibt es Bilder erstellen, Hintergrund entfernen und Untertitel hinzufügen. Unter Aktivität zusammenfassen sind „Auf einen Blick“ und Konversationszusammenfassung enthalten. Flows, KI-Kollege und Prototyping erscheinen, wenn sie für deine Organisation aktiviert sind.

**Kann ich sehen, welche Modelle spezifische Funktionen unterstützen?**

Ja. Admins können die mit jeder KI-Funktion verbundenen Modelle im Referenzbereich einsehen, um Überprüfung und Governance zu unterstützen.

## MIRO AI-Nutzung mit intelligenten Vorgaben blockieren

Verwende die intelligenten Vorgaben, um alle KI-gestützten Interaktionen in Miro zu blockieren, wenn du sensible oder vertrauliche Daten schützen musst. Wenn diese Vorgabe greift, werden alle Miro AI-Tools auf den betroffenen Boards deaktiviert, während die Zusammenarbeit ohne KI weiterhin möglich ist. Für Hintergrundinformationen und Einrichtung siehe die Übersicht zu intelligenten Vorgaben und Vorgaben definieren.

**Zweck und Geltungsbereich**

**Was bewirkt „Miro KI Nutzung blockieren“?**

Es deaktiviert alle Miro KI-Funktionen (zum Beispiel Texterstellung, Bildgenerierung/-erkennung, intelligente Vorschläge), wo immer diese Schutzmaßnahme gilt, und verhindert jegliche KI-gestützte Interaktion mit sensiblen oder klassifizierten Inhalten.

**Was bleibt den Nutzern verfügbar?**

Nutzer können weiterhin reguläre, nicht KI-gestützte Zusammenarbeit durchführen. Bereits KI-generierte Inhalte bleiben auf den Boards und können angesehen, verschoben oder manuell bearbeitet werden – aber Nutzer können Miro KI nicht verwenden, um diese zu verändern oder neu zu generieren.

**Zugang und Voraussetzungen**

**Wer kann diese Vorgabe konfigurieren und wo?**

Admins für sensible Inhalte konfigurieren Vorgaben in *Enterprise Guard* unter Datenklassifizierung → Vorgaben. (Unternehmens-Admins weisen die Rolle des Admins für sensible Inhalte zu.)

**Was benötige ich, bevor ich diese Vorgabe zuteile?**

Definiere deine Klassifizierungsstufen und (optional) die automatische Klassifizierung, damit die Vorgabe nach Klassifizierung angewendet werden kann (z. B. INTERN, VERTRAULICH).

**Verhalten und Auswirkungen**

**Wer ist betroffen, wenn die Leitplanke greift?**

Alle—einschließlich Board-Eigentümer und Miteigentümer—können auf den betroffenen Boards nicht auf Miro AI zugreifen oder es aufrufen.

**Entfernt es vorhandene KI-Inhalte?**

Nein. Es verhindert weitere KI-Interaktionen; bestehende KI-Inhalte bleiben weiterhin zur Ansicht und manuellen Bearbeitung verfügbar.

**Wann treten Änderungen in Kraft?**

Nachdem du deine Leitplanken-Updates veröffentlicht hast, wird die Durchsetzung sofort auf den betroffenen Boards wirksam.

**Einrichtung und Konfiguration**

**Wie aktiviere ich „Miro AI-Nutzung blockieren“ für eine Klassifizierung?**

1. Gehe zu *Enterprise Guard* → Datenklassifizierung → **Leitplanken**.
2. Klicke auf das **Bearbeiten-Symbol** für eine Klassifizierungsstufe (zum Beispiel VERTRAULICH).
3. Wähle das **„Miro AI-Nutzung blockieren“**-Kästchen aus und klicke auf **Fertig**.
4. Klicke auf **Weiter** und überprüfe die Auswirkungen, dann auf **Veröffentlichen**, um anzuwenden.

**Sollte ich den Standard- oder den strengen Modus verwenden?**

Im Standardmodus überschreiben die Vorgaben nicht die aktuellen Freigabeeinstellungen. Im strikten Modus überschreiben die Vorgaben aktive Freigaben und wenden die strengsten Kontrollen an. Wählt den Modus entsprechend eurer Änderungsmanagement-Bedürfnisse.

**Nutzererfahrung**

**Was sehen Nutzer auf Boards, auf denen KI gesperrt ist?**

Miro-KI-Einstiegspunkte erscheinen deaktiviert oder nicht verfügbar, und Nutzer können keine KI-Tools vom Canvas oder aus den Menüs auf diesen Boards aufrufen.

**Können Nutzer Ausnahmen für ein einzelnes Board beantragen?**

Nein. Die Vorgabe wird durch die Klassifizierungspolitik durchgesetzt. Ändert die Klassifizierung des Boards (oder die Politik für dieses Niveau), um die Durchsetzung zu ändern.

**Interaktionen mit anderen Steuerungen**

**Wie verhält sich dies im Vergleich zu granularen Miro KI-Admin-Steuerungen?**

Granulare Steuerungen verwalten, wer spezifische KI-Funktionen nutzen kann. Die Schutzmaßnahme ist eine Richtlinienebene: Wenn aktiv, blockiert sie KI unabhängig von Feature-Schaltern.

**Wie unterscheidet sich dies von Prompt-Blockierung oder KI-Moderation?**

- **Prompt-Blockierung** stoppt sensitive Prompts bei der Eingabe; KI bleibt für nicht-sensitive Prompts verfügbar.
- **KI-Moderation** filtert schädliche oder unangemessene Inhalte.
- **Miro KI-Nutzung blockieren** deaktiviert KI vollständig auf betroffenen Boards.

**Fehlerbehebung**

**KI erscheint immer noch auf einigen Boards. Was sollte ich überprüfen?**

- Bestätige, dass die Klassifizierung des Boards eine ist, bei der die Vorgabe aktiviert ist, und dass du auf **Veröffentlichen** geklickt hast, nachdem du die Vorgaben bearbeitet hast.
- Wenn du die automatische Klassifizierung verwendest, überprüfe, ob die Board-Klassifizierung basierend auf dem aktuellen Inhalt aktualisiert wurde.
- In Strikten vs Standard-Modi, stelle sicher, dass deine Erwartung dem von dir gewählten Rollout-Modus entspricht.

**Wir müssen die KI für einen Teil der Arbeit wieder aktivieren.**

Passt die Vorgabe für die relevante Klassifizierung an oder klassifiziert die Boards neu, die die KI zulassen sollten, und veröffentliche dann das Update.

## Admin-Analysenübersicht-Dashboard

**Umfang und Kennzahlen**

**Was deckt das Übersichts-Dashboard ab?**

Boards, Nutzer, Teams, Lizenzen und Vorlagen, mit verlaufsbezogenen Trends, wenn zutreffend.

**Wie wird "Aktiv in diesem Zeitraum" für Boards, Nutzer und Teams definiert?**

- **Boards:** Einzigartige Boards, die seit Beginn des ausgewählten Zeitraums geöffnet wurden. Dazu gehören auch Boards, die später in den Papierkorb verschoben wurden.
- **Nutzer:** Einzigartige Nutzer, die mindestens einmal seit Beginn des Zeitraums ein Board geöffnet haben. Dazu gehören auch Nutzer, die jetzt deaktiviert sind.
- **Teams:** Einzigartige Teams mit mindestens einem Mitglied, das seit Beginn des Zeitraums ein Board geöffnet hat. Kann Teams umfassen, die später in den Papierkorb verschoben wurden.

**Werden bei den Gesamtsummen Elemente im Papierkorb ausgeschlossen?**

Ja. Die Gesamtsummen für Boards und Teams schließen Elemente im Papierkorb aus. Bisherige „aktive“ Zählungen können Elemente enthalten, die später in den Papierkorb verschoben wurden.

**Was zeigt das Lizenzdiagramm?**

Zuordnungssummen und Verlauf für Full-, Free- und kostenlose eingeschränkte Lizenzen, der zeigt, wie viele Lizenzen derzeit genutzt werden.

**Was zeigt Vorlagen heute?**

Die am häufigsten verwendeten Vorlagen innerhalb eines Boards. Andere Quellen können in zukünftigen Versionen hinzugefügt werden.

**Zeit- und Verlaufsverhalten**

**Wie werden verlaufsbezogene Werte auf Übersichtsgrafiken angezeigt?**

Verlaufselemente zeigen die Werte am letzten Tag jedes Zeitraums. Es ist bis zu ein Jahr Verlauf oder bis zum frühesten vorhandenen Datum verfügbar.

**Datenaktualität und Steuerung**

**Wie oft werden die Übersichtsdaten aktualisiert und wo kann ich sie sehen?**

Mindestens einmal alle 24 Stunden. Ein Zeitstempel "Zuletzt aktualisiert" ist im Dashboard verfügbar.

**Wie ändere ich die Zeitspanne?**

Verwende den Zeitbereichsauswähler oben rechts auf der Analysen-Seite.

## Miro AI Moderation

Mit der Miro AI-Moderation können Unternehmens-Admins die Filterstufen für Prompts, die möglicherweise schädliche oder unangemessene Texte enthalten, anpassen. Du kannst die Empfindlichkeit der Miro AI-Moderation für die gesamte Organisation einstellen, um Inhalte wie Hass, sexuelle Inhalte, Gewalt und Selbstverletzung zu filtern. Dies hilft dir dabei, die Nutzung von Miro AI mit den Anforderungen, Richtlinien und der Risikobereitschaft deines Unternehmens in Einklang zu bringen. Weitere Informationen findest du in der [Miro AI-Moderationsdokumentation](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Zweck und Geltungsbereich**

**Was ist KI-Moderation in Miro?**

Die KI-Moderation ermöglicht es Unternehmens-Admins, ein organisationsweites Filter-Level festzulegen (Strikt, Standard oder Minimal), das Eingaben überprüft, die zu schädlichen oder unangemessenen Ausgaben führen könnten (z. B. Hass, sexuelle Inhalte, Gewalt, Selbstverletzung).

**Wer kann es konfigurieren und in welchen Preisplänen?**

Unternehmens-Admins bei Enterprise mit Enterprise Guard können die Einstellung in den Orgeinstellungen konfigurieren.

**Funktioniert es, wenn meine Organisation ihre eigene LLM (z. B. eine direkte Provider-Integration) verbindet?**

Wenn ein benutzerdefiniertes LLM verbunden ist, könnte der Moderationsauswahlschalter für diese Integration deaktiviert sein, und jegliches zuvor gewählte Level gilt nicht dafür.

**Zugang und Voraussetzungen**

**Wer kann es aktivieren und was wird benötigt?**

Admins im Enterprise-Plan mit dem Enterprise Guard Add-on können die KI-Moderation in den Organisationseinstellungen konfigurieren.

**Wie schalte ich es ein?**

Gehe zu Einstellungen → Miro AI → Moderation, wähle Streng/Standard/Minimal und klicke dann auf **Änderungen speichern**. Die Durchsetzung erfolgt sofort in der gesamten Organisation.

**Ebenen und Verhalten**

**Was bedeuten die Ebenen?**

- **Streng:** Blockiert Standard + Inhalte mit geringem bis mittlerem Risiko (z. B. subtile/verschlüsselte Hassbotschaften, anzügliche sexuelle Inhalte, nicht-graphische Gewalt, nicht-explizite Erwähnungen von Selbstverletzung).
- **Standard (empfohlen):** Blockiert mäßig bis stark schädliche Inhalte.
- **Minimal:** Blockiert nur stark schädliche Inhalte.

**Wann treten Änderungen in Kraft?**

Sofort für die gesamte Organisation.

**Werden Änderungen nachverfolgt?**

Ja. Aktualisierungen werden im Audit-Trail Ihrer Organisation aufgezeichnet.

**Einrichtung und Konfiguration**

**Wo stelle ich das Moderationsniveau ein oder aktualisiere es?**

Gehe zu Einstellungen → Miro AI → Moderation, wähle Strikt/Standard/Minimal, und klicke dann auf **Änderungen speichern**.

**Welches Anfangsniveau empfehlen Sie?**

Standard eignet sich für die meisten Organisationen; passe es basierend auf Rückmeldungen aus der Pilotphase und Risikotoleranz an.

**Interaktionen mit anderen Steuerungen**

**Wie steht die KI-Moderation in Beziehung zu Vorgaben und Prompt-Kontrollen?**

- **Intelligente Vorgaben:** Wenn ein Board durch die „Blockiere Miro-KI-Nutzung“ Vorgaben abgedeckt ist, wird die KI unabhängig vom Moderationsgrad deaktiviert.
- **Prompt-Blockierung:** Funktioniert zusammen mit der Moderation. Prompt-Blockierung stoppt sensitive Prompts bei der Eingabe; die Moderation filtert schädliche Kategorien.
- **Granulare Admin-Steuerungen:** Funktionsauswahl steuert, wer Zugriff auf KI-Funktionen hat, wenn die KI verfügbar ist.

**Fehlerbehebung und bewährte Verfahren**

**Wir erleben zu viele Fehlalarme.**

Erwägen Sie, von "Streng" auf "Standard" (oder von "Standard" auf "Minimal") zu wechseln und veröffentlichen Sie Beispiele für die akzeptable Nutzung. Wenn nach der Anpassung der Einstellungen weiterhin Probleme auftreten, kontaktieren Sie Ihren Miro Customer Success Manager, um dies zu melden, damit unser Produktteam dies überprüfen kann.

**Wir erleben, dass schädliche Inhalte durchschlüpfen.**

Wechseln Sie zu "Standard" oder "Streng" und geben Sie interne Richtlinien heraus. Überprüfen Sie die Situation nach Aktualisierungen der Richtlinien/Vorschriften. Wenn nach diesen Änderungen weiterhin Probleme auftreten, kontaktieren Sie Ihren Miro Customer Success Manager, um dies zu melden, damit unser Produktteam dies überprüfen kann.

## Prompt-Blockierung

Die Prompt-Blockierung erlaubt es Admins für sensible Inhalte, zu verhindern, dass Nutzer KI-Prompts einreichen, die sensible Informationen enthalten, und hilft Ihnen dabei, sensible Daten in Miro AI in Ihrer Organisation zu schützen. Miro prüft den Text, den ein Nutzer im Prompt-Feld eingibt, sowie alle textbasierten Inhalte, die sie vom Board hinzufügen. Wenn dieser Inhalt mit den in der Konfiguration für die Prompt-Blockierung ausgewählten Sensibilitätslabels oder Quellcode-Mustern übereinstimmt, blockiert Miro die Einreichung des Prompts.  Weitere Informationen findest du in der [Prompt-Blockierungsdokumentation](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Zweck und Geltungsbereich**

**Was ist Prompt-Blockierung?**

Prompt-Blockierung verhindert, dass Nutzer KI-Eingaben absenden, die sensible Informationen enthalten. Miro scannt den Text, den ein Nutzer in das Eingabefeld eingibt, und jegliche textbasierte Inhalte, die er vom Board hinzufügt; wenn diese mit ausgewählten Sensibilitätslabels oder Quellcode-Mustern übereinstimmen, wird die Eingabe blockiert und eine Meldung gemäß der Richtlinien angezeigt. Momentan unterstützen wir nur textbasierte Inhalte.

**Wie unterscheidet sich Prompt-Blockierung vom Board-Scanning?**

Beim Board-Scanning werden sensible Inhalte auf Boards ermittelt und die Boards können automatisch klassifiziert werden; Prompt-Blockierung überprüft, was Nutzer beim Einreichen an Miro KI senden möchten.

**Welche Sensibilitätslabels werden unterstützt?**

Verwenden Sie die unter Org-Ebene gelisteten Kategorien in der Referenz für Sensibilitätslabels und Infotypen.

**Was ist Scannen von Code?**

Scannen von Code blockiert Prompts, die erkennbaren Quellcode enthalten; hierfür ist ein Mindestblock von Code nötig (z.B. 5+ Zeilen), um ausgelöst zu werden. Du kannst es in der Konfiguration von Prompt-Blockierung ein-/ausschalten.

**Werden nichttextliche Inhalte (z.B. Bilder) gescannt?**

Nein. Derzeit unterstützt die Prompt-Blockierung nur textbasierte Inhalte.

**Zugriff und Voraussetzungen**

**Wer kann es aktivieren und was wird dafür benötigt?**

Sensitive Content Admins auf dem Enterprise-Plan mit dem Enterprise Guard Add-on können es in Einstellungen → Enterprise Guard → Datenerkennung → Konfiguration aktivieren.

**Wie aktiviere ich es?**

Öffne Prompt-Blockierung → Aktivieren, wähle „Alle auswählen“ oder spezifische Label-Kategorien, aktiviere optional das Scannen von Code, dann „Aktivieren“. Die Durchsetzung erfolgt unmittelbar organisationsweit.

**Verwaltung und Änderungen**

**Wie passe ich Labels oder das Scannen von Code später an?**

Gehe zu Einstellungen → Enterprise Guard → Datenerkennung → Konfiguration → Prompt-Blockierung → Verwalten,

- **Labels:** Wähle das *Alle auswählen* Kontrollkästchen, um alle Kategorien auszuwählen, oder wähle spezifische Label-Kategorien aus.
- **Scannen von Code:** Aktiviere das Scannen von Code, um Prompts zu blockieren, die Quellcode enthalten (mindestens 5 Zeilen). Für weitere Informationen siehe Scannen von Code.

Änderungen werden sofort wirksam.

**Was passiert mit Prompts, nachdem ich die Einstellungen geändert habe?**

Neu freigegebene Einträge werden durchgelassen. Einträge, die weiterhin zu gesperrten Mustern passen, bleiben gestoppt.

**Nutzererfahrung**

**Was sieht ein Nutzer, wenn ein Prompt blockiert wird?**

Eine Richtliniennachricht erscheint dort, wo sie den Prompt eingegeben haben, und die Anfrage wird an kein LLM gesendet.

**Wird nicht-textueller Inhalt (z. B. Bilder) gescannt?**

Nein. Zurzeit unterstützt die Prompt-Blockierung nur textbasierte Inhalte.

**Interaktionen mit anderen Steuerelementen**

**Wie funktioniert Prompt-Blockierung mit Vorgaben und Moderation?**

- **Intelligente Vorgaben:** Wenn „Die Nutzung von Miro AI blockieren“ gilt, ist die KI deaktiviert; Prompt-Blockierung wird nicht ausgelöst, da keine Prompts eingereicht werden können.
- **KI-Moderation:** Beide können angewendet werden, wenn die KI verfügbar ist – die Prompt-Blockierung stoppt sensible Daten; Moderation filtert schädliche Kategorien.
- **Detaillierte Admin-Steuerelemente:** Der Zugriff auf Funktionen gilt nur, wenn die KI verfügbar ist und der Prompt nicht blockiert ist.

##

## Enterprise Guard und Microsoft Purview DSPM für KI-Integration

Für Organisationen, die Microsoft Entra ID (ehemals Azure AD) als ihren Identitätsanbieter nutzen, leitet Enterprise Guard KI-Prompts und -Antworten sicher an Microsoft Purview Data Security Posture Management (DSPM) für KI weiter. Sicherheits- und Compliance-Teams können dann die Nutzung der generativen KI von einer einzigen vertrauenswürdigen Plattform aus überwachen, überprüfen und kontrollieren, den operativen Aufwand reduzieren, Risiken wie Datenlecks und Missbrauch mindern und die KI-Governance auf Enterprise-Ebene von Miro stärken. Weitere Informationen finden Sie in der [Dokumentation zur Enterprise Guard und Microsoft Purview DSPM für KI-Integration](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Zweck und Geltungsbereich**

**Was ist die Microsoft Purview DSPM für KI-Integration in Miro?**

Eine Integration, die Miro-KI-Prompts und -Antworten an das Microsoft Purview DSPM für KI weiterleitet, sodass Sicherheits- und Compliance-Teams KI-Aktivitäten an einem Ort überwachen, prüfen und steuern können.

**Wer kann diese Integration nutzen?**

Enterprise-Preispläne mit Enterprise Guard, verwaltet von Unternehmens-Admins mit Zugriff auf Enterprise-Integrationen. Ihre Miro-Organisation muss Microsoft Entra ID für Single Sign-on (SSO) verwenden. Eine Microsoft Purview-Lizenz ist erforderlich.

**Welche Vorteile gibt es?**

Zentralisierte Sichtbarkeit der Nutzung von Miro-KI im Purview AI-Hub, Prüfungsfähigkeit von Prompts und Antworten sowie die Übereinstimmung mit Ihren bestehenden Governance-Richtlinien in Purview.

**Welche Miro-KI-Aktivität ist derzeit enthalten?**

Derzeit werden textbasierte Prompts und Antworten über die Miro AI Features weitergeleitet. Bildinhalte werden nicht weitergeleitet.

**Werden alle Aktivitäten der Nutzer aufgezeichnet?**

Nur Aktivitäten von Nutzern, die sich über den konfigurierten Microsoft Entra-Tenant bei Miro anmelden, werden an Purview weitergeleitet.

**Wie lange dauert es, bis die Aktivitäten in Purview erscheinen?**

Normalerweise 10 bis 30 Minuten nach der KI-Aktion in Miro. Ansehen in Microsoft Purview → DSPM für KI → Aktivitätsexplorer, oder Audit-Protokolle überprüfen.

**Gibt es bemerkenswerte Einschränkungen?**

Derzeit kann ein Entra-Tenant gleichzeitig konfiguriert werden. In Umgebungen mit mehreren IdPs oder Tenants werden nur Benutzer protokolliert, die sich über den konfigurierten Tenant authentifizieren. Bilder sind nicht enthalten.

**Einrichtung und Konfiguration**

**Wie aktiviere ich die Integration?**

In Miro: Enterprise-Einstellungen → Enterprise-Integrationen → Microsoft Purview DSPM für KI aktivieren → Entra-Tenant-ID eingeben → Verbinden → mit einem Konto anmelden, das tenantweite Admin-Zustimmung gewähren kann → die Miro AI Governance-App akzeptieren → Verbunden bestätigen in Miro.

**Was sind die Voraussetzungen?**

- **Miro:** Enterprise-Preisplan mit Enterprise Guard, Unternehmens-Admin-Rolle, Entra ID für Single Sign-on konfiguriert. Um diese Funktion zu aktivieren, kontaktieren Sie Ihren Customer Success Manager.
- **Microsoft:** Microsoft Purview-Lizenz, die Entra-Tenant-ID, die für Miro SSO verwendet wird, und eine Entra-Rolle, die tenantweite Admin-Zustimmung gewähren kann.

**Wie stelle ich sicher, dass das Setup funktioniert?**

Führe eine einfache Miro AI-Aktion aus, warte 10–30 Minuten und überprüfe dann Microsoft Purview → DSPM für KI → Aktivitätsexplorer auf neue Miro-Einträge.

**Wie kann ich die Verbindung trennen oder den Mandanten wechseln?**

In Miro: Enterprise-Integrationen → Microsoft Purview für KI → Trennen. Um den Mandanten zu wechseln, zuerst die Verbindung trennen und dann mit der neuen Mandanten-ID erneut verbinden.

**Nutzung und Verwaltung**

**Wo kann ich die weitergeleiteten Daten in Purview einsehen?**

Microsoft Purview → DSPM für KI → Aktivitätsexplorer. Sie können auch Details in den Audit-Protokollen prüfen.

**Kann ich KI-Aktivitätsprotokolle exportieren oder archivieren?**

Verwenden Sie die Export-Tools von Microsoft Purview. Miro leitet die Aktivität an Ihr Microsoft-Mandant weiter, wo Ihre Richtlinien gelten.

**Kann ich Purview-Richtlinien auf Miro AI-Daten anwenden?**

Ja. Sobald die Daten erfasst sind, folgen sie dem Purview-Governance-Modell Ihrer Organisation.

**Wie sieht es mit den Datenschutz- und Sicherheitsverantwortlichkeiten aus?**

Miro leitet Prompts und Antworten an Ihr Microsoft-Mandant weiter. Governance- und Zugangskontrollen werden in Purview innerhalb Ihrer Umgebung verwaltet.

**Fehlerbehebung und Support**

**Der Zustimmungsschritt schlägt fehl oder wiederholt sich. Was sollte ich überprüfen?**

Stelle sicher, dass das Konto, das für die Verbindung verwendet wird, berechtigt ist, unternehmensweite Admin-Zustimmungen in Entra zu erteilen, oder ziehe einen globalen Microsoft-Admin hinzu.

**Ich sehe keine Aktivitäten in Purview. Was nun?**

Stelle sicher, dass Enterprise Guard aktiviert ist und du Zugriff auf Enterprise-Integrationen hast. Überprüfe, ob die Tenant-ID genau mit deiner Miro Single Sign-on Tenant übereinstimmt. Stelle sicher, dass eine Test-KI-Aktion von einem Nutzer durchgeführt wurde, der sich über diesen Tenant authentifiziert. Überprüfe die Purview-Lizenzen und Filter. Lasse bis zu 30 Minuten für die Erfassung zu.

**Wir verwenden mehrere Identitätsanbieter oder Tenants. Werden alle Nutzer protokolliert?**

Nein. Es wird nur die Aktivität von Nutzern weitergeleitet, die sich über den einzig konfigurierten Entra-Tenant anmelden.

**Wer unterstützt was?**

Wende dich für Setup- oder Verbindungsthemen in Miro an den Miro Support. Bei Problemen innerhalb von Microsoft Purview wende dich an den Microsoft Support.
