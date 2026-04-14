---
title: "Verkn\xFCpfen Sie Tools mit Zapier"
article_id: 30124629305106
translation_id: 30124629305106
locale: de
sidebar_position: 2
created_at: '2025-10-10T11:48:03Z'
updated_at: '2025-10-14T12:37:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Verbinden Sie Miro Insights mit Hunderten von Tools über [Zapier](http://zapier.com/), um automatisch Feedback und Daten aus Quellen zu erfassen, die keine direkten Integrationen haben. Damit können Sie Customer Insights zentral aus Ihrem gesamten technischen Umfeld sammeln.

Die Zapier-Integration ermöglicht Ihnen:

- Automatische Erstellung von Feedback-Elementen aus Kundensupport-Tickets, Umfragen oder Chat-Konversationen.
- Erfassung von Daten aus jedem Tool, das von Zapier unterstützt wird, auch wenn Miro Insights keine direkte Integration hat.
- Reduzierung manueller Dateneingaben durch Einrichten automatisierter Workflows.

## Feedback erstellen

Zapier bietet zwei Hauptaktionen zum Erstellen von Feedback-Elementen in Miro Insights an.

### Feedback erstellen

Die Standardaktion zum Erstellen allgemeiner Feedback-Elemente in Miro Insights mit den folgenden Feldern:

- **Feedback-Titel**: Kurze Zusammenfassung des Feedbacks.
- **Inhalt**: Ausführlicher Feedback-Inhalt oder Beschreibung.
- **Name des Meldenden**: Name der Person, die das Feedback gibt.
- **E-Mail-Adresse des Meldenden**: E-Mail-Adresse des Feedbackgebers.
- **E-Mail-Adresse des Eigentümers**: Interner Eigentümer oder Verantwortlicher für das Feedback.
- **Bereitgestelltes Datum und Uhrzeit**: Wann das Feedback ursprünglich gegeben wurde.
- **Ursprungs-URL**: Link zur Originalquelle (Ticket, Umfrageantwort usw.).
- **Unternehmensname**: Organisation, mit der das Feedback verbunden ist.
- **Unternehmensdomain**: Domain der Unternehmenswebsite.

### Feedback erstellen (Anruf)

Eine spezielle Aktion, die speziell für die Erfassung von Feedback aus Anrufen und Gesprächen mit diesen Feldern entwickelt wurde:

- **Anruftitel**: Titel oder Betreff des Anrufs.
- **Anruftranskript**: Vollständiges Transkript oder Merkzettel vom Anruf.
- **Origin-URL**: Link zur Aufzeichnung oder zu den Sitzungsdetails.
- **Teilnehmer**: Informationen über die Anrufteilnehmer.
  - **E-Mail**: E-Mail-Adresse des Teilnehmers.
  - **Name**: Name des Teilnehmers.
- **Besitzer-E-Mail**: Interner Besitzer oder Zuständiger für das Anruf-Feedback.
- **Startdatum und -uhrzeit**: Wann der Anruf stattfand.
- **Firmenname**: Organisation, die mit dem Anruf in Verbindung steht.
- **Unternehmensdomain**: Domain der Firmenwebsite.

## Einrichtung der Zapier-Integration

Um mit Zapier und Miro Insights zu beginnen, gehe wie folgt vor.

### Voraussetzungen

- Aktives Miro Insights-Konto
- Zapier-Konto (Free oder kostenpflichtig)
- Zugang zum Quellwerkzeug, das du verbinden möchtest

### Schnellstart mit Vorlagen

Miro Insights bietet vorgefertigte Zapier-Vorlagen für beliebte Tools zur Gesprächsanalyse, wie Grain, Fathom und Fireflies.

Um ein Zap mit einer Vorlage einzurichten:

1. Gehe zu den Miro Insights Einstellungen > **Integrationen & Automatisierungen**.
2. Wähle dein Gesprächstool aus. Zum Beispiel Grain.
3. Melde dich bei Zapier an, falls erforderlich.
4. Verbinde dein GrainKonto.
5. Führe das Mapping der Felder von Grain zu Miro Insights-Feldern durch.
6. Teste und aktiviere die vorkonfigurierte Integration.

Vorlagen bieten eine schnellere Einrichtungserfahrung mit optimierten Feldzuordnungen für jedes bestimmte Tool, sodass es einfacher ist, Kundenfeedback aus Ihren aufgezeichneten Gesprächen zu erfassen.

### Grundlegende Einrichtung

1. **Erschaffen Sie ein neues Zap** in Ihrem Zapier-Dashboard.
2. Wählen Sie Ihre **Trigger-App**. Das Tool, aus dem das Feedback hervorgeht.
3. Wählen Sie **Miro Insights** als Ihre Aktions-App aus.
4. Wähle dein **Aktionsevent**:
   - **„Feedback erstellen“** für allgemeine Feedback-Elemente.
   - **„Feedback (Anruf) erstellen“** für anrufbezogenes Feedback.
5. Verbinde dein **Miro Insights-Konto** auf Aufforderung.
6. **Felder mappen** von deiner Trigger-App zu Miro Insights-Feldern.
7. Teste die Integration, um sicherzustellen, dass die Daten korrekt fließen.
8. **Aktiviere den Zap**, um die automatische Datensammlung zu starten.

### Beste Praktiken für das Mapping

Beim Mapping von Feldern von deinem Quell-Tool zu Miro Insights solltest du die folgenden Best Practices beachten, um eine hochwertige Datenerfassung zu gewährleisten.

**Erforderliche Felder:**

- **Feedback-Titel**: Verwende klare, beschreibende Titel aus deinen Quelldaten.
- **Inhalt**: Mappe den Hauptinhalt des Feedbacks oder kombiniere mehrere Felder.

**Empfohlene Felder:**

- **Informationen des Berichtenden**: Erfasse Kontaktdaten der Kunden, wenn verfügbar.
- **Firmendaten**: Essenziell für das kontobasierte Produktmanagement.
- **Ursprungs-URL**: Sicherstellen der Rückverfolgbarkeit zu den Originalquellen.
- **Bereitstellungsdatum**: Verwende das tatsächliche Feedbackdatum, nicht das Verarbeitungsdatum.

**Tipps zur Feldabbildung:**

- Verwende die Formatierungstools von Zapier, um mehrere Quellfelder zu kombinieren.
- Füge den Namen des Quelltools im Titel oder Inhalt hinzu, um Klarheit zu schaffen.
- Verwende konsistente Formate für Daten, Firmennamen und Kategorien.
- Setze Standardwerte für optionale Felder.
