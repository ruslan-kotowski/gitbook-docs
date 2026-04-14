---
title: "Trello f\xFCr dein Team einrichten"
article_id: 30634093325842
translation_id: 30634093325842
locale: de
sidebar_position: 2
created_at: '2025-10-29T15:59:48Z'
updated_at: '2026-02-23T11:40:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Die Trello-Integration wird technisch über eine REST-API implementiert. Für Authentifizierungs- und Autorisierungszwecke nutzt die Integration das branchenübliche OAuth 2.0-Protokoll. Ein wichtiger Bestandteil dieser Architektur ist die Nutzung einer einheitlichen API-Plattform als Subprozessor für Daten von Drittanbietern. Diese Plattform stellt einheitliche APIs bereit, die für die Authentifizierung, Normalisierung und Synchronisierung von Daten über verschiedene API-Anbieter verantwortlich sind.

## Datenflüsse

Ein gründliches Verständnis des Datenflusses ist entscheidend, um Sicherheit und Compliance in Ihrer Organisation zu verwalten.

### Sequenzdiagramm auf hoher Ebene

Erstellen eines Trello-Karten-Widgets

![Trello (BETA) 2.jpg](images/30635007776658_Trello%20(BETA) 2.jpg)

Aktualisieren eines Trello-Karten-Widgets

![Trello (BETA) 2.jpg](images/30635007776658_Trello%20(BETA) 2.jpg)

### Trello-Daten in Miro

Wenn Nutzer Trello-Karten auf ein Miro-Board importieren, werden die relevanten Kartendaten zu einem integralen Bestandteil der Miro-Canvas-Daten. Miro speichert die folgenden spezifischen Datenpunkte für importierte Karten, sofern sie in Trello verfügbar sind:

- Titel
- Beschreibung
- Mitglieder (einschließlich Nutzernamen und E-Mail-Adressen)
- Liste
- Labels

Die explizite Auflistung der gespeicherten Datentypen ist entscheidend für die Datenverwaltung und Compliance der Organisation. Sie ermöglicht es Admins, genau zu beurteilen, welche Informationen, insbesondere potenziell sensible Daten, in die Miro-Umgebung repliziert werden. Diese Transparenz stellt sicher, dass die internen Datenrichtlinien der Organisation eingehalten werden. Außerdem ist es bemerkenswert, dass laut dem Abschnitt "Limitations" benutzerdefinierte Felder nicht unterstützt werden und daher nicht gespeichert sind, was ein wichtiger Punkt für die Datenabbildung und Compliance-Bewertungen ist. Miro verfolgt einen hybriden Ansatz zur Datenspeicherung, der die direkt auf dem Karten-Widget gespeicherten Daten minimiert und zusätzliche Details abruft, wenn der Nutzer den Bearbeitungsmodus öffnet.

### Aufbewahrung der gespeicherten Informationen bei Miro

Alle importierten Trello-Daten, die innerhalb von Miro gespeichert werden, unterliegen strikt der standardmäßigen Datenaufbewahrungsrichtlinie von Miro. Diese Richtlinie wird für alle Kundendaten einheitlich angewendet, um einen einheitlichen Ansatz für das Datenlebenszyklusmanagement zu gewährleisten.

## Authentifizierung und Autorisierung

Die Trello-Integration startet einen Authentifizierungsablauf, wenn ein Nutzer erstmals mit der Integration interagiert. Die Autorisierung innerhalb von Trello wird vom Integrationsdienst gehandhabt. Für jeden einzelnen Nutzer erstellt Miro ein Konto beim Integrationsdienst, und diese Anmeldedaten werden anschließend für alle Nutzerinteraktionen mit der Integration verwendet.

Die Integration erfordert in der Regel die Zustimmung eines Trello-Admins, um die Integrations-App innerhalb des Unternehmenssystems zu autorisieren. Darüber hinaus müssen auch einzelne Nutzer die Miro Trello-Integration über die OAuth-Autorisierungsseite von Trello autorisieren, wenn sie das erste Mal versuchen, einen Trello-Link einzubetten.

### Erforderliche Berechtigungsbereiche

Der Berechtigungsbereich kann je nach Drittanbietersystem variieren. Für Kartenverwaltungs-Integrationen wie Trello benötigt Miro jedoch in der Regel Zugriff auf folgende Daten:

| Geltungsbereich | Beschreibung |
| --- | --- |
| Karten (lesen und schreiben) | Gewährt der Integration die Berechtigung, bestehende Karten (Tickets) zu lesen sowie Karten innerhalb von Trello zu erstellen oder zu ändern. |
| Nutzer (lesen) | Gewährt der Integration die Berechtigung, Nutzerinformationen innerhalb von Trello zu lesen, typischerweise für die Zuweisung von Karten oder die Anzeige von Mitgliedsnamen. |
| Sammlungen (lesen) | Gewährt der Integration die Berechtigung, Sammlungen, Boards und Listen innerhalb von Trello zu lesen. |

### Was wird in Miro gespeichert und wie

Miro speichert sowohl autorisierungsbezogene als auch unfurling-bezogene Daten für die Trello-Integration sicher:

- **Autorisierungsbezogene Daten:** Dies umfasst Zugriffstoken und Aktualisierungstoken, die in der Miro-Datenbank für eine begrenzte Dauer von mehreren Tagen gespeichert werden. Diese Tokens werden automatisch mit dem Aktualisierungstoken erneuert, sobald sie ablaufen, um den kontinuierlichen Zugang zu gewährleisten. Alle diese Daten, die in der Datenbank für diese Integration gespeichert sind, werden mit dem 256-Bit Advanced Encryption Standard verschlüsselt, wodurch eine robuste Sicherheitsschicht geschaffen wird.
- **Entfaltungsbezogene Daten:** Dazu gehören die Titel der Karten, die als Teil der Miro-Boards selbst gespeichert werden. Zusätzlich werden Titel und verschlüsselte Referenzen zu diesen Elementen in einem internen Dienst gespeichert, weiter gesichert durch Verschlüsselung (Schlüsselverwaltung).

### Ein Token widerrufen

Falls erforderlich, können Admins oder einzelne Nutzer die für die Trello-Integration erteilten Tokens widerrufen. Die Nutzer können über die Integrationseinstellungen zu diesem Punkt gelangen, indem sie entweder einen Integrationen-Karten-Auswahldialog öffnen, das Drei-Punkte-Menü oben rechts anklicken und **Integrationseinstellungen** auswählen, oder über den **Apps**-Tab in den Miro-Teameinstellungen, die spezifische Integration finden und darauf klicken. Auf der Einstellungsseite kann die Autorisierung durch Klicken auf die **Trennen**-Schaltfläche widerrufen werden. Nach dieser Aktion wird Miro den Zugriff auf Trello widerrufen und das damit verbundene Konto des Nutzers löschen. Zur Deinstallation auf Team-Ebene können Admins die spezifischen Schritte im Abschnitt "Fehlerbehebung & FAQs (Admin)" befolgen.

## So richten Sie die Trello-Integration ein

Der Einrichtungsprozess für die Miro + Trello Integration umfasst für Admins und Endnutzer unterschiedliche Schritte, um eine kontrollierte Implementierung innerhalb einer Organisation zu gewährleisten.

1. **Aktive Konten sicherstellen:** Vor der Installation muss sichergestellt werden, dass sowohl aktive Miro- als auch Trello-Konten vorhanden sind.
2. **Installation auf Teamebene (Admin-Aktion):**
   - Admins müssen möglicherweise die Trello-Integration für ihr Miro-Team explizit autorisieren. Teammitglieder können die Integration nur nutzen, wenn sie auf Teamebene installiert wurde.
   - Ein Miro-Team-Admin kann die App direkt installieren, indem er ein Miro-Board öffnet, **Tools Media & Integrations (+)** auswählt, nach „Trello“ sucht und auf **Verbinden** klickt, um die Integration zu autorisieren. Wenn ein Miro-Team-Admin diese Aktion durchführt, wird die App automatisch autorisiert und installiert, ohne dass eine weitere administrative Genehmigung erforderlich ist.
3. **Nutzeranfrage und Admin-Freigabeflow (falls zutreffend):**
   - In Organisationen, in denen eine strenge administrative Zustimmung erforderlich ist, kann ein Nicht-Admin-Nutzer eines für die Trello-Integration konfigurierten Miro-Teams einen Trello-Link auf ein Miro-Board einfügen. Diese Aktion könnte ein "App-Installationsanfrage"-Dialogfeld für den Nutzer auslösen, das ihn zur Einholung einer administrativen Genehmigung auffordert.
   - Die zuständigen Admins können diese ausstehende Anfrage dann über ihre Miro- oder Trello-Administrationskonsolen überprüfen und genehmigen, abhängig von dem spezifischen Zustimmungsflow, der konfiguriert wurde.
4. **Individuelle Nutzerverbindung:**
   - Nachdem die Integration auf Teamebene erfolgreich installiert und von einem Admin autorisiert wurde, klicken individuelle Nutzer auf **Verbinden** im Trello-Widget, das auf dem Miro-Board erscheint.
   - Die Nutzer werden dann zu einer Trello-Autorisierungsseite weitergeleitet, auf der sie Miro Zugriff auf ihr persönliches Trello-Konto gewähren, womit sie ihre persönliche Autorisierung zur Einbettung und Interaktion mit Inhalten bestätigen.

## Sicherheits- und Compliance-Überlegungen

### Zugriffsbeschränkung auf die Quelldatei

Um sicherzustellen, dass der Zugriff auf eingebettete Trello-Daten auf dieselben Personen beschränkt bleibt wie im ursprünglichen Trello-Board, müssen Miro-Organisations-Admins strenge Kontrollen über das Teilen von Boards und den Export von Inhalten aufrechterhalten. Während die Kernintegration von Trello individuelle Berechtigungen für die Live-Interaktion respektiert, könnte jeder Export oder statische Snapshot von Board-Inhalten Daten potenziell unbefugten Personen zugänglich machen, wenn das Miro-Board selbst nicht sicher verwaltet wird.

### Fehlerbehandlung

Die Integration ist so gestaltet, dass sie eine ansprechende UI-Fallback- und Fehlerbehandlung bietet, wenn Karten-Datenaktualisierungen aufgrund von Drittanbieterablehnungen fehlschlagen.

### Miro-Datenverarbeitungszusatz (DPA)

Für umfassende rechtliche Angaben und Details zur Compliance bezüglich der Datenverarbeitungspraktiken von Miro werden Administratoren gebeten, das [Miro Data Processing Addendum](https://miro.com/legal/customer-data-processing-addendum/) zu konsultieren.

## Fehlerbehebung & FAQs

### Wie kann man die Integration ausschalten (Deinstallation auf Teamebene)?

Ein Miro-Team-Admin kann die Trello-Integration auf Teamebene deinstallieren. Diese Aktion deaktiviert die Integration für alle Teammitglieder. Gehe dazu zu **Teameinstellungen Apps & Integrationen**. Suche "Trello" oder "Trello Card Management" in der Liste der installierten Apps, scrolle nach unten und klicke auf **Für Team deinstallieren**.

### Wie kann man die Integration ausschalten (individuelle Deinstallation)?

Einzelne Nutzer können die Integration für sich selbst deinstallieren. Gehe dazu in deinen Miro-Einstellungen zu **Apps & Integrationen**. Suche nach "Trello" oder "Trello Card Management" und klicke auf **Deinstallieren für mich**.

### Welche Administratoren können die Trello-Integration für ihr Team installieren?

Nur Miro-Teamadmins können die App direkt installieren. Wenn ein Miro-Teamadmin eine Trello-URL auf ein Miro-Board einfügt, wird die App automatisch autorisiert und installiert, ohne dass weitere Schritte erforderlich sind.

### Welche Verfügbarkeitsanforderungen gibt es für die Trello-Integration?

Die Trello-Integration ist für die Business- und Enterprise-Pläne von Miro verfügbar.

### Müssen Administratoren die Trello-Integration für ihr Team autorisieren?

Ja, Admins müssen möglicherweise die Trello-Integration für ihr Miro-Team genehmigen. Teammitglieder können die Trello-Integration nur nutzen, wenn sie auf Teamebene installiert wurde.
