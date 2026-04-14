---
title: "Asana f\xFCr dein Team einrichten"
article_id: 28252196453778
translation_id: 28252196453778
locale: de
sidebar_position: 2
created_at: '2025-07-22T13:30:20Z'
updated_at: '2026-02-20T09:00:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dieser Abschnitt bietet umfassende technische und administrative Details, die für IT- und Sicherheitsexperten unerlässlich sind, die für die Implementierung, Sicherheit und laufende Verwaltung der Asana-Integration innerhalb ihrer Organisation verantwortlich sind.

## Technischer Überblick

Die Asana-Integration wird technisch über eine REST-API implementiert. Für Authentifizierungs- und Autorisierungszwecke verwendet die Integration das branchenübliche OAuth 2.0-Protokoll. Ein Schlüsselelement dieser Architektur ist die Nutzung einer einheitlichen API-Plattform als Subprozessor für Drittanbieterdaten. Diese Plattform bietet einheitliche APIs, die für die Authentifizierung, Normalisierung und Synchronisierung von Daten über verschiedene API-Anbieter zuständig sind.

## Datenflüsse

Ein gründliches Verständnis der Datenflüsse ist entscheidend, um die Sicherheit und Compliance innerhalb Ihrer Organisation zu gewährleisten.

### Hochrangiges Sequenzdiagramm

Erstellen einer Asana-Karten-Widget

![image (7).png](images/30597113893138_image%20(7).png)

Aktualisieren einer Asana-Karten-Widget

![image (8).png](images/30597113905042_image%20(8).png)

### Asana-Daten in Miro

Wenn Nutzer Asana-Aufgaben auf ein Miro-Board importieren, werden die relevanten Aufgabendaten zu einem integralen Bestandteil der Miro-Canvas-Daten. Miro speichert folgende spezifische Datenpunkte für importierte Aufgaben, sofern sie in Asana verfügbar sind:

- Titel
- Beschreibung
- Zugewiesen (einschließlich Name und/oder E-Mail-Adresse des Nutzers)
- Status
- Priorität

Die explizite Aufzählung der gespeicherten Datentypen ist entscheidend für die organisatorische Datenverwaltung und Compliance. Sie ermöglicht Admins eine genaue Beurteilung darüber, welche Informationen, insbesondere potenziell sensible Daten, in die Miro-Umgebung repliziert werden. Diese Transparenz sorgt für die Übereinstimmung mit den internen Richtlinien zur Datenverarbeitung der Organisation. Außerdem ist bemerkenswert, dass laut des "Einschränkungen"-Abschnitts benutzerdefinierte Felder nicht unterstützt und daher nicht gespeichert werden, was ein wichtiges Detail für die Datenabbildung und Compliance-Bewertungen ist. Miro verwendet einen hybriden Ansatz zur Datenspeicherung, wodurch die direkt auf dem Karten-Widget gespeicherten Daten minimiert und zusätzliche Details abgerufen werden, wenn der Nutzer die Bearbeitungsansicht öffnet.

### Datenaufbewahrung der gespeicherten Informationen bei Miro

Alle importierten Asana-Daten, die innerhalb von Miro gespeichert sind, unterliegen strikt der standardmäßigen Datenaufbewahrungsrichtlinie von Miro. Diese Richtlinie wird konsequent auf alle Kundendaten angewendet und gewährleistet einen einheitlichen Ansatz für das Datenlebenszyklusmanagement.

## Authentifizierung und Autorisierung

Die Asana-Integration initiiert einen Authentifizierungsflow, wenn ein Nutzer erstmals mit der Integration interagiert. Die Autorisierung innerhalb von Asana wird vom Integrationsdienst gehandhabt. Für jeden einzelnen Nutzer erstellt Miro ein Konto beim Integrationsdienst, und diese Anmeldeinformationen werden anschließend für alle Nutzerinteraktionen mit der Integration verwendet.

Für die Integration ist in der Regel die Genehmigung eines Asana-Admins (oder eines Microsoft Entra-Admins, falls Asana über Azure AD verwaltet wird) erforderlich, um die Integrations-App im Ökosystem ihrer Organisation zu autorisieren. Zusätzlich müssen einzelne Nutzer die Miro-Asana-Integration über die OAuth-Autorisierungsseite von Asana genehmigen, wenn sie zum ersten Mal versuchen, einen Asana-Link einzubetten.

### Erforderliche Autorisierungs-Geltungsbereiche

Der Geltungsbereich kann je nach spezifischem Drittanbietersystem variieren. Für Ticketing-Integrationen wie Asana benötigt Miro jedoch in der Regel Zugriff auf die folgenden Daten:

| Geltungsbereich | Beschreibung |
| --- | --- |
| Tickets (lesen und schreiben) | Gewährt der Integration die Berechtigung, vorhandene Aufgaben zu lesen sowie Aufgaben in Asana zu erstellen oder zu ändern. |
| Nutzer (lesen) | Gewährt der Integration die Berechtigung, Nutzerdaten innerhalb von Asana zu lesen, typischerweise zur Zuordnung von Aufgaben oder zur Anzeige der Namen der Zuweisungen. |
| Tags (lesen) | Gewährt der Integration die Berechtigung, Tags zu lesen, die mit Aufgaben in Asana verknüpft sind. |
| Sammlungen (lesen) | Gewährt der Integration die Berechtigung, Sammlungen von Aufgaben oder Projekten innerhalb von Asana zu lesen. |

### Was in Miro gespeichert wird und wie

Miro speichert sicher sowohl autorisierungsbezogene Daten als auch Daten zur Entfaltung in Bezug auf die Asana-Integration:

- **Autorisierungsbezogene Daten:** Dies umfasst Zugriffstoken und Aktualisierungstoken-Werte, die für eine begrenzte Dauer von mehreren Tagen in der Miro-Datenbank gespeichert werden. Diese Tokens werden bei Ablauf automatisch mit dem Aktualisierungstoken aktualisiert, um den kontinuierlichen Zugriff sicherzustellen. Alle in der Datenbank für diese Integration gespeicherten Daten sind mittels 256-Bit Advanced Encryption Standard verschlüsselt, was eine robuste Datenschutzeinrichtung bietet.
- **Entfaltungsbezogene Daten:** Dazu gehören Titel von Aufgaben, die als Teil der Miro-Boards selbst gespeichert werden. Zusätzlich werden Titel und verschlüsselte Verweise auf diese Elemente in einem internen Dienst gespeichert, der durch Verschlüsselung (Schlüsselverwaltung) weiter gesichert wird.

### Token widerrufen

Falls erforderlich, können Admins oder individuelle Nutzer die für die Asana-Integration erteilten Tokens widerrufen. Nutzer können die Integrationseinstellungen entweder öffnen, indem sie im Integrationsaufgabenwähler die Dreipunkt-Menüleiste in der oberen rechten Ecke anklicken und **Integrationseinstellungen** auswählen oder indem sie das Tab **Apps** im Miro-Team-Einstellungen aufrufen, die spezifische Integration finden und anklicken. Auf der Einstellungsseite kann die Autorisierung durch Klicken auf die **Trennen**-Schaltfläche widerrufen werden. Nach diesem Vorgang wird Miro den Zugriff auf Asana widerrufen und das zugehörige Konto des Nutzers löschen. Für die Deinstallation auf Teamebene können Admins die spezifischen Schritte im Abschnitt "Problemlösungen & FAQs (Admin)" befolgen.

## Wie man die Asana-Integration einrichtet

Der Einrichtungsprozess für die Miro + Asana Integration umfasst spezifische Schritte sowohl für Admins als auch für Nutzer, um eine kontrollierte Implementierung innerhalb eines Unternehmens sicherzustellen.

1. **Aktive Konten sicherstellen:** Vor Beginn der Installation ist sicherzustellen, dass sowohl aktive Miro- als auch Asana-Konten verfügbar sind.
2. **Installation auf Team-Ebene (Admin-Aktion):**
   - Admins müssen möglicherweise die Asana-Integration für ihr Miro-Team explizit genehmigen. Teammitglieder können die Integration nur nutzen, wenn sie auf Teamebene installiert wurde.
   - Ein Miro-Team-Admin kann die App direkt installieren, indem er ein Miro-Board öffnet, **Tools Media & Integration (+)** auswählt, nach "Asana" sucht und auf **Verbinden** klickt, um die Integration zu genehmigen. Wenn ein Miro-Team-Admin diese Aktion durchführt, wird die App automatisch genehmigt und installiert, ohne dass eine weitere administrative Zustimmung erforderlich ist.
3. **Nutzeranfrage und Admin-Freigabefluss (falls zutreffend):**
   - In Organisationen, in denen eine strikte Admin-Genehmigung erforderlich ist, kann ein Nicht-Admin-Nutzer eines für die Asana-Integration konfigurierten Miro-Teams einen Asana-Link in ein Miro-Board einfügen. Diese Aktion könnte ein "App-Installationsanfrage"-Dialogfeld für den Nutzer auslösen, das ihn auffordert, eine Admin-Genehmigung einzuholen.
   - Die benannten Admins können dann diese ausstehende Anfrage über ihre Miro- oder Asana-Admin-Konsolen prüfen und freigeben, je nach dem spezifischen Freigabefluss, der konfiguriert wurde.
4. **Individuelle Nutzerverbindung:**
   - Nachdem die Integration auf Teamebene erfolgreich von einem Admin installiert und autorisiert wurde, klicken die einzelnen Nutzer auf **Verbinden** im Asana-Widget, das auf dem Miro-Board erscheint.
   - Die Nutzer werden dann auf eine Autorisierungsseite von Asana weitergeleitet, wo sie Miro Zugriff auf ihr individuelles Asana-Konto gewähren und damit ihre persönliche Autorisierung zur Einbettung und Interaktion mit Inhalten bestätigen.

## Sicherheits- und Compliance-Überlegungen

### Zugriffsbeschränkung auf die Quelldatei

Um sicherzustellen, dass der Zugriff auf eingebettete Asana-Daten auf dieselben Personen beschränkt bleibt wie in der ursprünglichen Asana-Datei, müssen die Miro-Organisationsadministratoren strikte Kontrolle über das Teilen von Boards und den Export von Inhalten aufrechterhalten. Während die Kernfunktion der Asana-Integration individuellen Berechtigungen für Live-Interaktionen Rechnung trägt, könnte jeder Export oder statische Snapshot von Board-Inhalten Daten potenziell unbefugten Personen zugänglich machen, wenn das Miro-Board selbst nicht sicher verwaltet wird.

### Fehlerbehandlung

Die Integration ist so konzipiert, dass sie eine elegante UI-Notlösung und Fehlerbehandlung bietet, falls Karten-Datenaktualisierungen aufgrund der Ablehnung durch Dritte fehlschlagen.

### Miro-Zusatz zur Datenverarbeitung (DPA)

Für umfassende rechtliche und Compliance-Details zu Miros Datenverarbeitungsverfahren werden Admins gebeten, das [Miro Data Processing Addendum](https://miro.com/legal/customer-data-processing-addendum/) zu konsultieren.

## Fehlerbehebung & FAQs

### Wie kann man die Integration deaktivieren (Deinstallation auf Teamebene)?

Ein Miro Team-Admin kann die Asana-Integration auf Teamebene deinstallieren. Diese Aktion deaktiviert die Integration für alle Teammitglieder. Gehe dazu zu **Team-Einstellungen Integrationen & Apps**. Finde "Asana Ticketing" in der Liste der installierten Apps, scrolle nach unten und klicke auf **Deinstallieren für Team**.

### Wie kann man die Integration deaktivieren (individuelle Deinstallation)?

Einzelne Nutzer können die Integration für sich selbst deinstallieren. Gehe zu **Apps & Integrationen** in deinen Miro-Einstellungen. Finde "Asana Ticketing" und klicke auf **Für mich deinstallieren**.

### Welche Administratoren können die Asana-Integration für ihr Team installieren?

Nur Miro-Team-Administratoren können die App direkt installieren. Wenn ein Miro-Team-Administrator eine Asana-URL auf ein Miro-Board einfügt, wird die App automatisch autorisiert und installiert, ohne dass weitere Maßnahmen erforderlich sind.

### Welche Verfügbarkeitsanforderungen bestehen für die Asana-Integration?

Die Asana-Integration ist für die Business- und Enterprise-Pläne von Miro verfügbar.

### Müssen Administratoren die Asana-Integration für ihr Team autorisieren?

Ja, Admins müssen möglicherweise die Integration von Asana für ihr Miro-Team autorisieren. Teammitglieder können die Asana-Integration nur nutzen, wenn sie auf Teamebene installiert ist.
