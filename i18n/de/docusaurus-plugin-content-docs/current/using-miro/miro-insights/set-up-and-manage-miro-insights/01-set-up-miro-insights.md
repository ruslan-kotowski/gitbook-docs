---
title: Einrichtung von Miro Insights
article_id: 30122381753106
translation_id: 30122381753106
locale: de
sidebar_position: 0
created_at: '2025-10-10T10:26:28Z'
updated_at: '2025-11-25T15:54:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Das Verbinden Ihrer Tools mit Miro Insights ist ein entscheidender erster Schritt, um echten Mehrwert zu erzielen. Integrationen ermöglichen es Miro Insights, automatisch Kundenfeedback und relevante Daten aus Ihren Systemen zu importieren. Dieses Handbuch richtet sich an Unternehmens-Admins, die diese Verbindungen aktivieren werden.

Wenn Sie ein Teammitglied sind, das Miro Insights nach der Einrichtung nutzen möchte, sehen Sie sich den Artikel zur [Nutzung von Miro Insights](../../miro-insights/use-miro-insights) an.

## Voraussetzungen

Um Miro Insights-Integrationen einzurichten, müssen Sie die folgenden Anforderungen erfüllen:

- Du musst **Company Admin in Miro** sein.
- Du musst **Admin- oder API-Zugriff auf der externen Plattform** haben, die du verbindest.

:::note
Stelle sicher, dass dein **Miro-Preisplan Miro Insights** umfasst. Wenn Miro Insights ein Add-on oder in begrenzter Veröffentlichung ist, muss dein Konto berechtigt sein. Auch erfordern einige Integrationen möglicherweise spezifische Editionen der externen Software. Beispielsweise ist der Zugriff auf bestimmte CRM-APIs in höherstufigen Plänen verfügbar.
:::

## Datenquellen vorbereiten

Bevor du deine Datenquellen mit Miro Insights verbindest, ist es wichtig, deine Daten vorzubereiten und eine klare Taxonomie zu erstellen. Diese Vorbereitung stellt sicher, dass du die präzisesten und handlungsfähigsten Einsichten von der Plattform erhältst.

### Daten bereinigen und optimieren

Bevor Sie Daten mit Miro Insights synchronisieren, bereinigen und optimieren Sie Ihre Datenquellen:

- Entfernen Sie Duplikate und veraltete Elemente.
- Bereinigen Sie inkonsistentes oder irrelevantes Feedback.
- Sorgen Sie für Datenqualität in Ihren Quellsystemen.
- Beheben Sie größere Dateninkonsistenzen oder Lücken im Vorfeld.

### Ihre Taxonomie etablieren

Obwohl Miro Insights mit grundlegenden, KI-erstellten Kategorien ausgestattet ist, wird empfohlen, vor der Einführung eine eigene standardisierte Taxonomie zu definieren. Dies stellt sicher, dass von Anfang an Konsistenz herrscht und die Qualität der Erkenntnisse verbessert wird.

Berücksichtigen Sie dabei die Aufnahme dieser Standardkategorien:

- Funktionsanfragen
- Fehler
- UX-Problempunkte
- Kundensegmente
- Prioritäten
- Geschäftsbereiche
- Strategische Initiativen

Best Practices für Taxonomie:

- Verwende eine Terminologie, die der Sprache deines Teams entspricht.
- Erstelle klare Richtlinien für wann und wie jede Kategorie verwendet werden soll.
- Teile die Taxonomie deinem Team mit, um eine konsistente Nutzung sicherzustellen.
- Überprüfe und verfeinere die Kategorien regelmäßig nach Bedarf.
- Ziehe in Betracht, sie mit deinen strategischen Initiativen und OKRs abzustimmen.

:::tip
Wende dich an den Miro Insights Support, um Hilfe bei der Definition deiner Taxonomie zu erhalten. Sie können dir Beispiele und Best Practices von anderen Kunden in deiner Branche bereitstellen.
:::

## Eine Integration verbinden

Wenn Ihre Daten bereit sind, können Sie Ihre Integrationen verbinden. Miro Insights unterstützt eine Vielzahl beliebter Tools in den Bereichen CRM, Support, Vertriebsanrufe, Projektmanagement und Chat-Plattformen.

Im Tab **Integrationen & Automatisierungen** können Sie alle verbundenen Integrationen anzeigen und verwalten. Jede Integration wird mit ihrem Verbindungsstatus sowie Optionen zur Konfiguration oder zum Trennen aufgelistet.

So verbinden Sie eine Integration:

1. Wählen Sie in der **Miro Insights** App das **Einstellungs** Symbol oben in der linken Seitenleiste aus.
2. Gehen Sie im **Einstellungs** Feld zum **Integrationen & Automatisierungen** Tab.
3. Wählen Sie **Verbinden** neben der Integration aus, die Sie hinzufügen möchten.
4. **Zugriff autorisieren**. Ein Pop-up wird dich auffordern, Miro Insights die Zugriffsberechtigung für dieses Tool zu erteilen.
   Dies erfordert in der Regel, dass du dich bei dem externen Dienst anmeldest und Berechtigungen erteilst. Beispielsweise musst du dich beim Verbinden mit Salesforce mit deinem Salesforce-Admin-Konto anmelden und die Integration genehmigen. Bei Slack wählst du einen Workspace aus und autorisierst die Miro Insights Slack-App. Befolge die Anweisungen auf dem Bildschirm für jeden Fall.
5. **Importeinstellungen konfigurieren**. Sobald verbunden, wird die Integration als „Verbunden“ angezeigt, mit zusätzlichen Einstellungsmöglichkeiten. Hier kannst du festlegen:
   - **Gespräche importieren von**: Für gesprächsbasierte Quellen wie Gong oder Zendesk kann ein Datum gewählt werden. Dies verhindert das Einziehen alter Daten, es sei denn, dass dies gewünscht wird.
   - **Automatische Importregeln**: Schalte ein, ob neue Elemente automatisch importiert werden sollen. Du kannst dies aktivieren, damit neue Anrufe oder Tickets kontinuierlich einfließen. Wenn es deaktiviert bleibt, kannst du Elemente manuell oder selektiv importieren.
   - **Wenn die KI Anfragen erkennt mit**: Einige Quellen lassen sich nach KI-Erkennungssicherheit filtern.
   - **Probleme erkennen**: Ermöglicht Miro Insights, automatisch Probleme aus Kundenfeedback zu identifizieren und zu extrahieren. Diese Probleme können Nutzungsprobleme, Leistungsprobleme, Sicherheitsbedenken usw. umfassen.

Andere Optionen können je nach Integration variieren. In Jira kannst du beispielsweise auswählen, aus welchem Projekt oder Projekten Funktionen gezogen werden sollen oder benutzerdefinierte Felder zuordnen.

### AI-Filterung

Einige Integrationen ermöglichen es dir, nach **AI-Erkennung** zu filtern. Das bedeutet, dass Insights ein Transkript eines Gesprächs scannt und nur dann ein Feedback-Element erstellt wird, wenn sicher ist, dass eine Produktanfrage erwähnt wurde. Das reduziert das Rauschen durch themenfremde Gespräche. Du kannst die Vertrauensschwelle anpassen oder diese Funktion deaktivieren, um alles zu importieren.

### Tag- oder Feldfilter

In Tools wie Zendesk kannst du einen Tag festlegen. Zum Beispiel „feature_request“, dann werden nur Tickets mit diesem Tag aufgenommen. In Jira kannst du ein bestimmtes Projekt oder einen Vorgangstyp auswählen, um ihn als Funktion zu importieren.

### Synchronisierung von Vorgängen

Für Projekt-Tools wie Jira kannst du eventuell Felder zuordnen. Der obige Screenshot zeigt ein Beispiel „Feature-Wert in benutzerdefiniertes Feld schieben“ – du könntest ein benutzerdefiniertes Feld in Jira auswählen, das mit der berechneten Dollarauswirkung aus Miro Insights gefüllt wird, um den Bogen zurück zur Technik zu schließen. Dieser Schritt ist optional, kann aber sehr leistungsstark sein.

Verbinde alle relevanten Systeme. Wir empfehlen, mindestens ein CRM und eine Support- oder Feedbackquelle zu verbinden, um sowohl Kontokontext als auch Feedback zu erhalten. Du kannst später immer noch mehr hinzufügen.

Sobald du fertig bist, hast du deine Integrationen erfolgreich mit Miro Insights verbunden. Das System beginnt jetzt mit der Datensynchronisation. Die anfängliche Synchronisation kann etwas Zeit in Anspruch nehmen, wenn es viele verlaufsbezogene Daten gibt (du wirst die zuletzt synchronisierten Zeitstempel neben jeder Integration sehen). Du kannst den Synchronisierungsstatus in der Integrationsliste überwachen – sie zeigt die letzte Synchronisierungszeit an und bietet die Option zum Trennen der Verbindung bei Bedarf.

## Elemente manuell importieren

Du kannst Features und Feedback-Elemente auch manuell über eine CSV-Datei importieren. Dies ist nützlich für einmalige Importe oder wenn du eine Liste von Funktionsanfragen oder Feedback aus einer anderen Quelle hast.

Um Features über CSV zu importieren:

1. Gehe in Miro Insights zur **Backlog**-Ansicht.
2. Klicke oben rechts auf die **Import**-Schaltfläche.
3. Wähle **CSV hochladen** aus.
4. Wähle die Spalte in deiner CSV-Datenquelle, die am besten zu den Eigenschaften von Miro Insights passt.
5. Wähle **Feature importieren**, um den Vorgang abzuschließen.

Deine importierten Features erscheinen nun im [Backlog](../../tools/use-miro-insights/05-backlog.md)-Bereich.

Um Feedback-Elemente per CSV zu importieren:

1. Gehe in Miro Insights zur **Feedback**-Ansicht.
2. Klicke oben rechts auf die **Importieren**-Schaltfläche.
3. Wähle **CSV hochladen** aus.
4. Ordne die Spalten in deiner CSV den Feedback-Eigenschaften von Miro Insights zu (z. B. Titel, Beschreibung, Quelle).
5. Wähle **Feedback importieren** aus, um den Prozess abzuschließen.

Die importierten Feedback-Elemente erscheinen jetzt im [Feedback](../../tools/use-miro-insights/07-feedback.md)-Bereich.

## Nicht unterstützte Tools mit Zapier verbinden

Falls du ein Tool hast, das nicht direkt unterstützt wird, kannst du oft [Zapier](http://zapier.com/) verwenden, um Daten in Miro Insights weiterzuleiten. Du könntest zum Beispiel den folgenden Zapier-Workflow erstellen: Wenn ein Google-Formular eingereicht wird oder ein neuer Eintrag in einer benutzerdefinierten Datenbank erscheint, wird ein Feedback-Element in Miro Insights erstellt.

Ausführliche Schritte findest du im Artikel über [die Verwendung von Zapier mit Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/03-connect-tools-with-zapier.md).

## Zusätzliche Schritte

Nachdem du deine Integrationen verbunden hast, kannst du einige optionale Schritte durchführen, um sicherzustellen, dass alles korrekt eingerichtet ist:

### Features importieren oder überprüfen

Wenn du ein Task-Tracking-Tool wie Jira verbunden hast, überprüfe das Backlog in Miro Insights, um zu sehen, ob deine vorhandenen Features oder Epics erschienen sind. Falls nicht, kannst du die Schaltfläche „Importieren“ in der Backlog-Ansicht verwenden, um eine CSV hochzuladen oder einen Abruf von Jira auszulösen. Stelle sicher, dass jede importierte Funktion einen klaren Titel und eine klare Beschreibung hat; die KI ist auf diesen Text angewiesen, um relevantes Feedback zuzuordnen.

### Slack-Befehle oder E-Mail-Weiterleitung einrichten

Wenn du Slack hinzugefügt hast, informiere dein Team darüber, wie man Nachrichten an Insights senden kann. Zum Beispiel: Rechtsklicke auf eine Nachricht > „An Miro Insights senden“.

Für E-Mail oder andere Kanäle kannst du die Weiterleitung einrichten. Einige Teams richten eine spezifische E-Mail-Adresse ein, die automatisch in ein Tool wie Intercom oder einen Zapier-Hook zur Verarbeitung weiterleitet.

> **Tipp**: Es ist sinnvoll, die Integrationseinstellungen regelmäßig zu überprüfen. Wenn zum Beispiel zu viele belanglose Rückmeldungen von einer Quelle eingehen, sollten Sie die Filter anpassen oder die AI-Erkennungsschwelle erhöhen. Wenn Ihnen hingegen erwartete Daten fehlen, stellen Sie sicher, dass die Integration mit dem richtigen Geltungsbereich verbunden ist (z. B. das korrekte Projekt oder Tag). Eine gut abgestimmte Integration hält das Signal hoch und das Rauschen niedrig.

## Eine Integration trennen

Wenn Sie eine Integration trennen müssen:

1. Gehe zu **Einstellungen** > **Integrationen & Automatisierungen**.
2. Suche die Integration, die du entfernen möchtest.
3. Wähle **Trennen** daneben aus.
4. Bestätige die Trennung im Pop-up-Prompt.

Dies stoppt alle zukünftigen Datensynchronisationen von dieser Quelle.

> **Wichtig**: In einigen Fällen, zum Beispiel bei Gong, kann das Trennen auch zuvor importierte Rückmeldungen entfernen. In anderen Fällen, wie bei Jira, bleiben bestehende Funktionen erhalten, werden jedoch nicht mehr aktualisiert. Überprüfe das spezifische Verhalten jeder Integration in der Dokumentation oder kontaktiere den Support, wenn du unsicher bist.

Stelle sicher, dass du mit deinem Team kommunizierst, wenn du eine wichtige Quelle trennst, da dies die Vollständigkeit des Backlogs und des Feedbacks in Miro Insights beeinträchtigen kann.

## Wie geht es weiter?

Indem du Integrationen verbindest, hast du die Grundlage für Miro Insights gelegt, um reichhaltige und kontinuierliche Produkt-Insights zu liefern. Die Daten werden einfließen und die KI wird beginnen, Verbindungen herzustellen.

Du kannst nun fortfahren mit dem [Verwenden von Miro Insights](../../miro-insights/use-miro-insights) oder mehr über laufende administrative Aufgaben erfahren, einschließlich allgemeiner Einstellungen, Teamverwaltung, Benachrichtigungen und API-Zugriff im [Miro Insights Verwaltungshandbuch](../../miro-insights/set-up-and-manage-miro-insights/02-manage-miro-insights.md).
