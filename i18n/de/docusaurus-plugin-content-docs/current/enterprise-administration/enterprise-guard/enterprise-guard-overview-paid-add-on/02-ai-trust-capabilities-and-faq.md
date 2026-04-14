---
title: "KI-Sicherheitsfunktionen und h\xE4ufige Fragen"
article_id: 30943405198994
translation_id: 30943405198994
locale: de
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:32:10Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-granular-admin-settings
---

Bei unserem Event Canvas 25 haben wir den KI-Workspace für Innovation vorgestellt, der visuelle KI-Workflows und kollaborative KI-Agenten auf dem Canvas bietet. Zusätzlich zu den Endnutzer-Features führen wir neue Admin-Funktionen ein, die dir mehr Übersicht, intelligentere Steuerungsmöglichkeiten und nahtlose Wege bieten, die neuesten KI-Tools von Miro für deine Teams verfügbar zu machen.

Nutze diese Seite, um die KI-Sicherheitsfunktionen zu erkunden, die mit dem Enterprise Guard Add-on verfügbar sind. Jeder Abschnitt beginnt mit einem kurzen Überblick und wird durch erweiterbare FAQs ergänzt, die verschiedene Aspekte jeder Fähigkeit abdecken.

- Granulare Miro AI Admin-Kontrollen: Lege den Zugriff auf das Feature-Level (Alle/Keiner/Spezifische Teams) innerhalb jeder Fähigkeitengruppe fest.
- [Blockiere die Nutzung von Miro KI mit intelligenten Vorgaben](#h_block_ai_with_guardrails): Verwende intelligente Vorgaben, um alle KI-gestützten Interaktionen in Miro zu blockieren, wenn du sensible oder vertrauliche Daten schützen musst.
- [Admin Analysen-Dashboard Überblick](#h_admin_analytics_overview): Verfolge Boards, Nutzer, Teams, Lizenzen und Vorlagen mit verlaufsbezogenen Trends und täglichem Update.
- KI-Moderation (auch in der Enterprise-Stufe verfügbar): lege organisationsweite Filterstufen (Streng, Standard, Minimal) fest, um Prompts zu überprüfen, die zu schädlichen oder unangemessenen Ausgaben führen könnten.
- Prompt-Blockierung: blockiere Prompts, die sensible Daten oder Quellcode enthalten, direkt bei der Einreichung; zeige stattdessen eine Richtliniennachricht, anstatt sie an ein LLM zu senden.
- Enterprise Guard und Microsoft Purview DSPM für KI-Integration: leite Prompts und Antworten an Purview zur zentralen Überwachung, Prüfung und Steuerung weiter.

## Miro KI granulare Admin-Kontrollen für das Enterprise Guard Add-on

Miro AI-Admin-Kontrollen ermöglichen es Unternehmens-Admins, zu entscheiden, welche KI-Funktionen in ihrer Organisation verfügbar sind und zu verwalten, wer sie nutzen kann. Admins können sich auch die Modelle ansehen, die jede KI-Funktion unterstützen. Mit dem Enterprise Guard Add-on erweitern sich die Miro AI-Kontrollen bis zur Funktionsebene innerhalb jeder Funktionskategorie, was dabei hilft, Funktionen basierend auf organisatorischen Bedürfnissen und Sicherheitsanforderungen zu priorisieren. Neben der vollständigen Miro AI-Funktionskategorie können Admins auch spezifische Miro AI-Funktionen aktivieren, einschränken oder entfernen. Zum Beispiel kann innerhalb der Kategorie Bilder die Option „Bilder mit KI erstellen“ aktiviert und „Hintergrund entfernen“ deaktiviert werden. Verwende diese Kontrollen, um KI sicher einzuführen und Sicherheitsanforderungen zu erfüllen, während du die Einführung von KI-Funktionen förderst.  Weitere Informationen findest du in der [Dokumentation zu den granularen Admin-Kontrollen in Miro AI](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Zweck und Geltungsbereich**

**Was bedeutet granulare Kontrolle für Miro KI?**

Mit dem Enterprise Guard Add-on können Unternehmens-Admins den Zugriff auf einzelne KI-Funktionen innerhalb jeder Funktionsgruppe aktivieren, einschränken oder entfernen. So können Sie genau festlegen, welche Funktionen die Teams nutzen dürfen.

**Warum granulare Kontrollen verwenden?**

Um die Einführung mit der Sicherheit in Einklang zu bringen. Beispielsweise können Sie bei Bildern die Funktion "Bilder erstellen" aktivieren, während Sie "Hintergrund entfernen" deaktivieren.

**Zugriff und Voraussetzungen**

**Wer kann granulare Steuerungen konfigurieren und auf welchen Plänen?**

Company Admins auf Enterprise-Plänen mit dem Enterprise Guard Add-on, im Browser.

**Wo verwalte ich den Zugriff auf Funktionenebene?**

Admin Konsole → Miro AI → Fähigkeiten. Erweitern Sie eine Fähigkeit, um den Zugriff auf ihre einzelnen Funktionen zu sehen und festzulegen.

**Kontrollen und Verhalten**

**Granulare Kontrollen: Was ist der Unterschied zwischen Kapazitäts- und Funktionssteuerung und was passiert, wenn ich sie ein- oder ausschalte?**

- **Kapazitätssteuerung:** Alle, Niemand oder Bestimmte Teams gelten für die gesamte Kategorie. Wenn du eine Kapazität deaktivierst, verlieren die Nutzer den Zugriff auf diese Kapazität und alle ihre Funktionen über die Boards hinweg. Wenn du alle Kapazitäten deaktivierst, erscheint "KI nutzen" auf dem Board als deaktiviert.
- **Funktionssteuerung:** Mit Enterprise Guard kannst du pro einzelne Funktion Alle, Niemand oder Bestimmte Teams festlegen. Das Deaktivieren einer Funktion entfernt nur den Zugriff auf diese Funktion; andere Funktionen innerhalb derselben Kapazität bleiben verfügbar, wenn sie aktiviert sind.

**Welche Zugriffsmöglichkeiten gibt es auf Funktionsebene?**

Für jede Funktion kannst du zwischen Alle, Niemand oder Bestimmte Teams wählen. "Alle" aktiviert die Funktion organisationsweit und übergeht teambezogene Einschränkungen. "Niemand" entzieht allen Nutzern den Zugriff. "Bestimmte Teams" richtet sich nur an ausgewählte Teams.

**Was passiert, wenn ich eine einzelne Funktion deaktiviere?**

Nutzer können auf keinem Board auf diese Funktion zugreifen, aber andere Funktionen innerhalb derselben Fähigkeit bleiben verfügbar, wenn sie aktiviert sind.

**Referenz und Beispiele**

**Welche Funktionen kann ich individuell steuern?**

Siehe die in der Anwendung eingebettete Referenz für die aktuelle Liste. Beispiele unter „Inhalte erstellen“ umfassen Erstellen von Notizen, Gruppieren von Notizen, Erstellen und Bearbeiten von Dokumenten, Tabellen, Diagrammen und Textoperationen wie Umschreiben, Kürzen, Tonanpassung und Übersetzung. Bilder umfassen Bilder erstellen, Hintergrund entfernen und Bildunterschriften hinzufügen. Der Abschnitt „Aktivität zusammenfassen“ umfasst „Auf einen Blick“ und Gesprächszusammenfassung. Flows, KI-Kollegen und Prototyping erscheinen, wenn sie für Ihre Organisation aktiviert sind.

**Kann ich sehen, welche Modelle bestimmte Funktionen unterstützen?**

Ja. Admins können im Referenzbereich die mit jeder KI-Funktion verbundenen Modelle einsehen, um Überprüfung und Steuerung zu unterstützen.

## Nutzung von Miro KI mit intelligenten Vorgaben blockieren

Verwende die intelligenten Vorgaben, um alle KI-unterstützten Interaktionen in Miro zu blockieren, wenn du sensible oder geheime Daten schützen musst. Wenn diese Vorgabe greift, sind alle Miro AI-Tools auf den betroffenen Boards deaktiviert, während die Zusammenarbeit ohne KI weiterhin möglich bleibt. Weitere Informationen zur Einrichtung findest du im Überblick zu den intelligenten Vorgaben und unter Vorgaben definieren.

**Zweck und Geltungsbereich**

**Was bewirkt „Miro AI-Nutzung blockieren“?**

Es deaktiviert alle Miro AI-Funktionen (zum Beispiel Texterstellung, Bilderstellung/-erkennung, intelligente Vorschläge), wo immer diese Schutzmaßnahme greift, und verhindert jegliche KI-gestützte Interaktion mit sensiblen oder vertraulichen Inhalten.

**Was steht den Nutzern weiterhin zur Verfügung?**

Nutzer können weiterhin regulär ohne KI zusammenarbeiten. Bereits von der KI erstellte Inhalte bleiben auf den Boards und können angesehen, verschoben oder manuell bearbeitet werden—aber die Nutzer können Miro AI nicht verwenden, um sie zu ändern oder neu zu erstellen.

**Zugriff und Voraussetzungen**

**Wer kann diese Vorgaben konfigurieren und wo?**

Admins für sensible Inhalte konfigurieren Vorgaben in *Enterprise Guard* unter Datenklassifizierung → Vorgaben. (Unternehmens-Admins weisen die Rolle des Admins für sensible Inhalte zu.)

**Was benötige ich, bevor ich diese Vorgabe zuweise?**

Definiere deine Klassifizierungsstufen und optional die Auto-Klassifizierung, damit die Vorgabe entsprechend der Klassifizierung angewendet werden kann (zum Beispiel INTERN, VERTRAULICH).

**Verhalten und Auswirkungen**

**Wen betrifft es, wenn das Schutzgeländer greift?**

Alle – einschließlich Board-Eigentümer und Miteigentümer – können Miro AI auf den betroffenen Boards nicht aufrufen oder verwenden.

**Entfernt es vorhandene KI-Inhalte?**

Nein. Es verhindert weitere KI-Interaktionen; vorhandene KI-Inhalte bleiben zur Ansicht und manuellen Bearbeitung verfügbar.

**Wann treten die Änderungen in Kraft?**

Nachdem Sie Ihre Schutzgeländer-Updates veröffentlicht haben, erfolgt die Durchsetzung sofort auf den betroffenen Boards.

**Einrichtung und Konfiguration**

**Wie aktiviere ich „Blockiere Miro AI-Nutzung“ für eine Klassifizierung?**

1. Gehe zu *Enterprise Guard* → Datenklassifizierung → **Schutzmaßnahmen**.
2. Klicke auf das **Symbol**, um eine Klassifizierungsstufe (zum Beispiel VERTRAULICH) zu bearbeiten.
3. Wähle das Kontrollkästchen **Miro AI-Nutzung blockieren** und klicke auf **Fertig**.
4. Klicke auf **Weiter**, überprüfe die Auswirkungen und klicke dann auf **Veröffentlichen**, um die Änderungen anzuwenden.

**Sollte ich den Standardmodus oder den strikten Modus verwenden?**

Im Standardmodus überschreiben die Vorgaben keine bestehenden Freigabeeinstellungen. Im strikten Modus setzen die Vorgaben aktive Freigaben außer Kraft und wenden die strengsten Kontrollen an. Wählen Sie entsprechend Ihren Änderungsmanagementanforderungen.

**Nutzererfahrung**

**Was werden Nutzer auf Boards sehen, auf denen KI blockiert ist?**

Die Miro-KI-Einstiegspunkte erscheinen deaktiviert oder nicht verfügbar, und Nutzer können keine KI-Tools von der Canvas oder den Menüs auf diesen Boards aufrufen.

**Können Nutzer Ausnahmen für ein einzelnes Board anfragen?**

Nein. Die Vorgabe wird durch die Klassifizierungsrichtlinie durchgesetzt. Ändere die Klassifizierung des Boards (oder die Richtlinie für diese Ebene), um die Durchsetzung zu ändern.

**Interaktionen mit anderen Kontrollen**

**Wie verhält sich das im Vergleich zu den granularen Miro KI-Admin-Kontrollen?**

Granulare Kontrollen steuern, wer bestimmte KI-Funktionen nutzen kann. Die Richtlinie ist eine zusätzliche Ebene: Wenn aktiv, blockiert sie die KI unabhängig von Funktionsumschaltungen.

**Wie unterscheidet sich das von der Prompt-Blockierung oder der KI-Moderation?**

- **Prompt-Blockierung** stoppt sensible Prompts bei der Eingabe; KI bleibt für nicht sensible Prompts verfügbar.
- **KI-Moderation** filtert schädliche oder unangemessene Inhalte.
- **Nutzung von Miro KI blockieren** deaktiviert die KI vollständig auf betroffenen Boards.

**Fehlerbehebung**

**KI erscheint immer noch auf einigen Boards. Was sollte ich überprüfen?**

- Bestätige, dass die Klassifizierung des Boards eine ist, bei der die Vorgaben aktiviert sind, und dass du nach dem Bearbeiten der Vorgaben auf **Veröffentlichen** geklickt hast.
- Wenn die automatische Klassifizierung genutzt wird, prüfe, ob die Klassifizierung des Boards basierend auf dem aktuellen Inhalt aktualisiert wurde.
- Stelle im Modus "Streng vs. Standard" sicher, dass deine Erwartung dem von dir ausgewählten Rollout-Modus entspricht.

**Wir müssen die KI für einen Teil der Arbeit wieder aktivieren.**

Passe die Vorgaben für die relevante Klassifizierung an oder klassifiziere die Boards neu, die KI zulassen sollen, und veröffentliche dann das Update.

## Admin-Analysen-Übersichtsdashboard

**Umfang und Kennzahlen**

**Was umfasst das Übersichtsdashboard?**

Boards, Nutzer, Teams, Lizenzen und Vorlagen, mit verlaufsbezogenen Trends, wo anwendbar.

**Wie wird „In diesem Zeitraum aktiv“ für Boards, Nutzer und Teams definiert?**

- **Boards:** Einzigartige Boards, die seit Beginn des gewählten Zeitraums geöffnet wurden. Beinhaltet Boards, die später in den Papierkorb verschoben wurden.
- **Nutzer:** Einzigartige Nutzer, die seit Beginn des Zeitraums mindestens einmal ein Board geöffnet haben. Beinhaltet Nutzer, die jetzt deaktiviert sind.
- **Teams:** Einzigartige Teams mit mindestens einem Mitglied, das seit Beginn des Zeitraums ein Board geöffnet hat. Kann Teams beinhalten, die später in den Papierkorb verschoben wurden.

**Schließen die Summen Artikel im Papierkorb aus?**

Ja. Die Summen für Boards und Teams schließen Artikel aus, die sich derzeit im Papierkorb befinden. Bisherige „aktive“ Zählungen können Artikel beinhalten, die später in den Papierkorb verschoben wurden.

**Was zeigt das Lizenzdiagramm?**

Zuweisungssummen und Verlauf für vollständige, kostenlose und kostenlose eingeschränkte Lizenzen, die widerspiegeln, wie viele Lizenzen momentan genutzt werden.

**Was zeigt Vorlagen heute?**

Am meisten genutzte Vorlagen innerhalb eines Boards. Weitere Quellen können in zukünftigen Versionen hinzugefügt werden.

**Verhalten von Zeit und Verlauf**

**Wie werden verlaufsbezogene Werte in Übersichtscharts angezeigt?**

Verlaufs-Widgets zeigen die Werte zum letzten Tag jedes Zeitraums. Es sind bis zu ein Jahr Verlauf verfügbar oder so lange, wie Daten vorhanden sind.

**Aktualität der Daten und Steuerungsoptionen**

**Wie oft werden die Daten im Überblick aktualisiert und wo kann ich dies sehen?**

Mindestens einmal alle 24 Stunden. Ein "Zuletzt aktualisiert"-Zeitstempel ist im Dashboard verfügbar.

**Wie ändere ich den Zeitraum?**

Nutze den Zeitraum-Auswahlfilter oben rechts auf der Analysen-Seite.

## Miro AI Moderation

Mit der Miro AI-Moderation können Unternehmens-Admins die Filterungsebenen für Prompts anpassen, die potenziell schädlichen oder unangemessenen Text enthalten könnten. Du kannst die unternehmensweite Sensibilität der Miro AI-Moderation so einstellen, dass Inhalte wie Hassreden, sexuelle Inhalte, Gewalt und Selbstverletzung gefiltert werden. Dies hilft dir, die Nutzung von Miro AI mit den Anforderungen, Richtlinien und der Risikotoleranz deines Unternehmens in Einklang zu bringen. Weitere Informationen findest du in der [Miro AI-Moderationsdokumentation](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Zweck und Geltungsbereich**

**Was ist die Moderation in Miro?**

Die Moderation ermöglicht es Unternehmens-Admins, ein organisationsweites Filterungsniveau (Streng, Standard oder Minimal) festzulegen, das Eingaben filtert, die zu schädlichem oder unangemessenem Inhalt führen könnten (z. B. Hass, sexuelle Inhalte, Gewalt, Selbstverletzung).

**Wer kann es konfigurieren und in welchen Preisplänen?**

Unternehmens-Admins im Enterprise-Preisplan mit Enterprise Guard können die Einstellung in den Organisationseinstellungen konfigurieren.

**Funktioniert es, wenn meine Organisation ihr eigenes LLM verbindet (z. B. eine Direktanbieter-Integration)?**

Wenn ein benutzerdefiniertes LLM verbunden ist, kann der Moderationswähler für diese Integration deaktiviert sein, und jede zuvor gewählte Stufe wird darauf nicht angewendet.

**Zugriff und Voraussetzungen**

**Wer kann es aktivieren und was benötige ich?**

Admins im Unternehmen mit dem Enterprise Guard Add-on können die KI-Moderation in den Organisationseinstellungen konfigurieren.

**Wie schalte ich es ein?**

Gehe zu Einstellungen → Miro AI → Moderation, wähle Strikt/Standard/Minimal und klicke dann auf **Änderungen speichern**. Die Umsetzung erfolgt sofort in der gesamten Organisation.

**Stufen und Verhalten**

**Was bedeuten die Stufen?**

- **Streng:** Blockiert Standard + Inhalte mit geringem bis moderatem Risiko (z. B. subtile/verschlüsselte Hassinhalte, anzügliche sexuelle Inhalte, nicht-grafische Gewalt, nicht-explizite Erwähnungen von Selbstverletzung).
- **Standard (empfohlen):** Blockiert Inhalte mit moderatem bis schwerem Schadenspotenzial.
- **Minimal:** Blockiert nur Inhalte mit schwerem Schadenspotenzial.

**Wann treten Änderungen in Kraft?**

Sofort für die gesamte Organisation.

**Werden Änderungen protokolliert?**

Ja. Aktualisierungen werden im Audit-Trail Ihrer Organisation aufgezeichnet.

**Einrichtung und Konfiguration**

**Wo stelle ich die Moderationsstufe ein oder aktualisiere sie?**

Gehe zu Einstellungen → Miro AI → Moderation, wähle Strikt/Standard/Minimal und klicke dann auf **Änderungen speichern**.

**Welche Anfangsstufe empfehlen Sie?**

Standard ist für die meisten Organisationen geeignet; passe die Stufe basierend auf dem Feedback des Pilotprojekts und der Risikotoleranz an.

**Interaktionen mit anderen Kontrollen**

**Wie steht die KI-Moderation im Verhältnis zu Vorgaben und Prompt-Kontrollen?**

- **Intelligente Vorgaben:** Wenn ein Board durch die Vorgabe „Miro AI-Nutzung blockieren“ abgedeckt ist, wird KI unabhängig vom Moderationslevel deaktiviert.
- **Prompt-Blockierung:** Arbeitet zusammen mit der Moderation. Prompt-Blockierung stoppt sensitive Prompts bei der Eingabe; Moderation filtert schädliche Kategorien.
- **Detaillierte Admin-Kontrollen:** Feature-Schalter bestimmen, wer auf KI-Funktionen zugreifen kann, wenn KI verfügbar ist.

**Fehlerbehebung und bewährte Verfahren**

**Wir sehen zu viele falsch-positive Ergebnisse.**

Erwägen Sie, von Strikt → Standard (oder Standard → Minimal) zu wechseln und Beispiele für akzeptable Nutzung zu veröffentlichen. Wenn nach der Anpassung der Einstellungen weiterhin Probleme bestehen, wenden Sie sich an Ihren Miro Customer Success Manager, um dies zu melden, damit unser Produktteam dies überprüfen kann.

**Wir sehen, dass schädliche Inhalte durchrutschen.**

Wechseln Sie zu Standard oder Strikt und geben Sie interne Anweisungen. Überprüfen Sie die Situation nach Aktualisierungen der Richtlinien/Vorschriften erneut. Wenn diese Probleme nach den Änderungen weiterhin bestehen, wenden Sie sich an Ihren Miro Customer Success Manager, um dies zu melden, damit unser Produktteam dies überprüfen kann.

## Prompt-Blockierung

Die Prompt-Blockierung erlaubt es Admins für sensible Inhalte, zu verhindern, dass Nutzer KI-Prompts einreichen, die sensible Informationen enthalten, und hilft Ihnen dabei, sensible Daten in Miro AI in Ihrer Organisation zu schützen. Miro scannt den Text, den ein Nutzer im Prompt-Feld eingibt, sowie jeden textbasierten Inhalt, den sie vom Board hinzufügen. Wenn dieser Inhalt mit den in der Konfiguration für die Prompt-Blockierung ausgewählten Sensibilitätslabels oder Quellcode-Mustern übereinstimmt, blockiert Miro die Einreichung des Prompts. Für weitere Informationen siehe die [Dokumentation zur Prompt-Blockierung](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Zweck und Geltungsbereich**

**Was ist Prompt-Blockierung?**

Prompt-Blockierung verhindert, dass Nutzer KI-Prompts absenden, die sensible Informationen enthalten. Miro scannt den Text, den ein Nutzer in das Prompt-Feld eingibt, sowie alle textbasierten Inhalte, die sie vom Board hinzufügen. Wenn dieser den ausgewählten Sensibilitätslabels oder Quellcode-Mustern entspricht, wird die Einreichung blockiert und eine Richtlinienmeldung angezeigt. Derzeit unterstützen wir nur textbasierte Inhalte.

**Wie unterscheidet sich Prompt-Blockierung vom Board-Scanning?**

Beim Board-Scanning wird sensible Inhalte auf Boards ermittelt und die Boards können automatisch klassifiziert werden; Prompt-Blockierung überprüft, was Nutzer beim Einreichen an Miro AI senden möchten.

**Welche Sensibilitätslabels werden unterstützt?**

Verwenden Sie die auf Organisationsebene aufgeführten Kategorien aus der Sensibilitätslabel- und Infotypen-Referenz.

**Was ist Scannen von Code?**

Scannen von Code blockiert Prompts, die erkennbaren Quellcode enthalten; es erfordert designbedingt einen Mindestblock von Code (z. B. 5+ Zeilen), um ausgelöst zu werden. Du kannst es in der Konfiguration der Prompt-Blockierung ein-/ausschalten.

**Werden nicht-textbasierte Inhalte (z. B. Bilder) gescannt?**

Nein. Zurzeit unterstützt Prompt-Blockierung nur textbasierte Inhalte.

**Zugriff und Voraussetzungen**

**Wer kann es aktivieren und was benötige ich?**

Sensitive Content Admins auf Enterprise mit dem Enterprise Guard Add-on können es in Einstellungen → Enterprise Guard → Datenerkennung → Konfiguration aktivieren.

**Wie schalte ich es ein?**

Öffne Prompt-Blockierung → Aktivieren, wähle „Alle auswählen“ oder spezifische Label-Kategorien, aktiviere optional das Scannen von Code, dann „Aktivieren“. Die Durchsetzung erfolgt sofort unternehmensweit.

**Verwaltung und Änderungen**

**Wie kann ich später Labels oder das Scannen von Code anpassen?**

Gehe zu Einstellungen → Enterprise Guard → Datenerkennung → Konfiguration → Prompt-Blockierung → Verwalten,

- **Labels:** Wähle das *Alle auswählen*-Kontrollkästchen, um alle Kategorien auszuwählen, oder wähle spezifische Label-Kategorien aus.
- **Scannen von Code:** Aktiviere das Scannen von Code, um Prompts zu blockieren, die Quellcode (mindestens 5 Zeilen) enthalten. Weitere Informationen findest du unter Scannen von Code.

Änderungen werden sofort wirksam.

**Was passiert mit Prompts, nachdem ich die Einstellungen geändert habe?**

Neu freigegebene Elemente werden durchgelassen. Elemente, die weiterhin blockierten Mustern entsprechen, bleiben gestoppt.

**Nutzererlebnis**

**Was sieht ein Nutzer, wenn ein Prompt blockiert wird?**

An der Stelle, an der der Prompt eingegeben wurde, erscheint eine Richtlinienmeldung, und die Anfrage wird nicht an ein LLM gesendet.

**Wird nicht-textueller Inhalt (z. B. Bilder) gescannt?**

Nein. Momentan unterstützt die Prompt-Blockierung nur textbasierte Inhalte.

**Interaktionen mit anderen Kontrollen**

**Wie funktioniert Prompt-Blockierung mit Vorgaben und Moderation?**

- **Intelligente Vorgaben:** Wenn „Die Nutzung von Miro AI blockieren“ gilt, ist die KI deaktiviert; Prompt-Blockierung wird nicht ausgelöst, da keine Prompts eingereicht werden können.
- **Moderation:** Beide können angewendet werden, wenn KI verfügbar ist – die Prompt-Blockierung stoppt sensible Daten; Moderation filtert schädliche Kategorien.
- **Granulare Admin-Kontrollen:** Der Zugriff auf Funktionen gilt nur, wenn die KI verfügbar ist und der Prompt nicht blockiert wird.

##

## Enterprise Guard und Microsoft Purview DSPM für die KI-Integration

Für Organisationen, die Microsoft Entra ID (ehemals Azure AD) als ihren Identitätsanbieter nutzen, leitet Enterprise Guard KI-Prompts und -Antworten sicher an Microsoft Purview Data Security Posture Management (DSPM) für KI weiter. Sicherheits- und Compliance-Teams können dann die Nutzung generativer KI von einer einzigen vertrauenswürdigen Plattform aus überwachen, auditieren und steuern. Dies reduziert den Betriebsaufwand, mindert Risiken wie Datenverlust und Missbrauch und stärkt Miro’s unternehmensweite KI-Governance auf höchstem Niveau. Weitere Informationen finden Sie in der [Enterprise Guard und Microsoft Purview DSPM für die KI-Integration-Dokumentation](../integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Zweck und Geltungsbereich**

**Was ist die Integration von Microsoft Purview DSPM für KI in Miro?**

Eine Integration, die Miro AI-Prompts und -Antworten an das DSPM für KI von Microsoft Purview weiterleitet, sodass Sicherheits- und Compliance-Teams die KI-Aktivitäten an einem Ort überwachen, prüfen und regeln können.

**Wer kann diese Integration nutzen?**

Enterprise-Preispläne mit Enterprise Guard, verwaltet von Unternehmens-Admins mit Zugang zu Enterprise-Integrationen. Deine Miro-Organisation muss Microsoft Entra ID für SSO nutzen. Eine Microsoft Purview-Lizenz ist erforderlich.

**Welche Vorteile gibt es?**

Zentralisierte Überblick von Miro AI-Nutzung im AI-Hub von Purview, Prüfbarkeit der Prompts und Antworten sowie die Ausrichtung an den bestehenden Governance-Richtlinien in Purview.

**Welche Miro AI-Aktivitäten sind heute eingeschlossen?**

Im Moment werden textbasierte Prompts und Antworten über Miro KI-Funktionen weitergeleitet. Bildinhalte werden nicht weitergeleitet.

**Werden alle Nutzeraktivitäten protokolliert?**

Nur Aktivitäten von Nutzern, die sich über den konfigurierten Microsoft Entra-Tenant bei Miro anmelden, werden an Purview weitergeleitet.

**Wie lange dauert es, bis Aktivitäten in Purview erscheinen?**

In der Regel 10 bis 30 Minuten nach der KI-Aktion in Miro. Ansehen in Microsoft Purview → DSPM für KI → Aktivitäts-Explorer oder Audit-Protokolle prüfen.

**Gibt es bemerkenswerte Einschränkungen?**

Im Moment kann jeweils nur ein Entra-Tenant konfiguriert werden. In multi-IdP oder multi-Tenant Umgebungen werden nur Nutzer, die sich über den konfigurierten Tenant authentifizieren, protokolliert. Bilder sind nicht enthalten.

**Einrichtung und Konfiguration**

**Wie aktiviere ich die Integration?**

In Miro: Enterprise-Einstellungen → Enterprise-Integrationen → Microsoft Purview DSPM für KI aktivieren → Ihre Entra-Tenant-ID eingeben → Verbinden → mit einem Konto anmelden, das tenantsweite Admin-Zustimmung erteilen kann → die Miro AI Governance-App akzeptieren → "Verbunden" in Miro bestätigen.

**Was sind die Voraussetzungen?**

- **Miro:** Enterprise-Preisplan mit Enterprise Guard, Unternehmens-Admin-Rolle, Entra ID für SSO konfiguriert. Um diese Funktion zu aktivieren, kontaktieren Sie Ihren Customer Success Manager.
- **Microsoft:** Microsoft Purview-Lizenz, die Entra-Tenant-ID, die für Miro-SSO verwendet wird, und eine Entra-Rolle, die tenantsweite Admin-Zustimmung erteilen kann.

**Wie kann ich die Einrichtung bestätigen?**

Führe eine einfache Miro AI-Aktion durch, warte 10–30 Minuten und überprüfe dann Microsoft Purview → DSPM for AI → Aktivität Explorer auf neue Miro-Einträge.

**Wie trenne ich die Verbindung oder wechsle den Tenant?**

In Miro: Enterprise-Integrationen → Microsoft Purview für KI → Trennen. Um den Tenant zu wechseln, trenne zuerst die Verbindung und stelle sie dann mit der neuen Tenant-ID wieder her.

**Nutzung und Governance**

**Wo kann ich die übermittelten Daten in Purview einsehen?**

Microsoft Purview → DSPM for KI → Aktivitäten-Explorer. Details können Sie auch in den Audit-Protokollen prüfen.

**Kann ich KI-Aktivitätsprotokolle exportieren oder archivieren?**

Nutzen Sie die Export-Tools von Microsoft Purview. Miro leitet die Aktivität an Ihren Microsoft-Tenant weiter, wo Ihre Richtlinien angewendet werden.

**Können Purview-Richtlinien auf Miro-AI-Daten angewendet werden?**

Ja. Nach der Erfassung folgt die Datenverarbeitung Ihrem Purview-Governance-Modell Ihrer Organisation.

**Wie steht es um die Verantwortlichkeiten für Datenschutz und Sicherheit?**

Miro leitet Prompts und Antworten an Ihren Microsoft-Tenant weiter. Governance- und Zugriffskontrollen werden in Purview innerhalb Ihrer Umgebung verwaltet.

**Fehlerbehebung und Support**

**Der Zustimmungsschritt schlägt fehl oder wiederholt sich. Was sollte ich überprüfen?**

Stelle sicher, dass das für Connect verwendete Konto in Entra unternehmensweite Admin-Zustimmungen erteilen kann, oder ziehe einen globalen Microsoft-Admin hinzu.

**Ich sehe keine Aktivität in Purview. Was nun?**

Bestätige, dass Enterprise Guard aktiviert ist und du Zugriff auf Enterprise-Integrationen hast. Überprüfe, ob die Mandanten-ID genau mit deinem Miro SSO-Mandanten übereinstimmt. Stelle sicher, dass eine Test-KI-Aktion von einem Nutzer, der sich über diesen Mandanten authentifiziert hat, durchgeführt wurde. Prüfe Purview-Lizenzen und Filter. Warte bis zu 30 Minuten für die Übertragung.

**Wir verwenden mehrere Identitätsanbieter oder Mandanten. Werden alle Nutzer protokolliert?**

Nein. Es wird nur die Aktivität von Nutzern weitergeleitet, die sich über den konfigurierten Entra-Mandanten anmelden.

**Wer unterstützt was?**

Wende dich für die Einrichtung oder Konnektivität in Miro an den Miro Support. Bei Problemen innerhalb von Microsoft Purview wende dich an den Microsoft Support.
