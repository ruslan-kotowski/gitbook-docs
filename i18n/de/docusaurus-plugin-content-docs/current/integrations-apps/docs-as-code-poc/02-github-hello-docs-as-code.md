---
title: '[GitHub] Hallo, Dokumente-als-Code!'
article_id: 29239655610258
translation_id: 29239655610258
locale: de
sidebar_position: 2
created_at: '2025-09-04T17:11:12Z'
updated_at: '2026-01-23T15:01:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dieser Abschnitt bietet umfassende technische und administrative Details, die für IT- und Sicherheitsexperten unerlässlich sind, die für die Bereitstellung, Sicherheit und kontinuierliche Verwaltung der Trello-Integration innerhalb ihrer Organisation verantwortlich sind.

## Technische Übersicht

Die Trello-Integration wird technisch über eine REST-API implementiert. Für Authentifizierungs- und Autorisierungszwecke nutzt die Integration das weit verbreitete OAuth 2.0-Protokoll. Ein wesentlicher Bestandteil dieser Architektur ist die Nutzung einer einheitlichen API-Plattform als Subprozessor für Drittanbieterdaten. Diese Plattform bietet einheitliche APIs, die für die Authentifizierung, Normalisierung und Synchronisierung von Daten über verschiedene API-Anbieter verantwortlich sind.

## Daten Flows

Ein gründliches Verständnis des Datenflusses ist entscheidend, um die Sicherheit und Compliance innerhalb deines Unternehmens zu verwalten.

### Hochrangiges Sequenzdiagramm

Erstellen eines Trello-Karten-Widgets

![image (7).png](images/32777110671762_image%20(7).png)

Aktualisieren eines Trello-Karten-Widgets

![image (8).png](images/32777110674834_image%20(8).png)

### Trello-Daten in Miro

Wenn Nutzer Trello-Karten auf ein Miro-Board importieren, werden die relevanten Kartendaten zu einem integralen Bestandteil der Miro-Canvas-Daten. Miro speichert die folgenden spezifischen Datenpunkte für importierte Karten, sofern sie in Trello verfügbar sind:

- Titel
- Beschreibung
- Mitglieder (einschließlich Nutzernamen und E-Mail-Adressen)
- Liste
- Labels

Die explizite Aufzählung der gespeicherten Datentypen ist entscheidend für die unternehmensweite Datenverwaltung und Compliance. Sie ermöglicht es den Admins, genau zu beurteilen, welche Informationen, insbesondere potenziell sensible Daten, in die Miro-Umgebung übertragen werden. Diese Transparenz stellt sicher, dass alles mit den internen Datenverwaltungsvorschriften der Organisation übereinstimmt. Es sei auch darauf hingewiesen, dass laut dem Abschnitt „Einschränkungen“ benutzerdefinierte Felder nicht unterstützt werden und daher nicht gespeichert werden, was ein wichtiger Aspekt für die Datenabbildung und Compliance-Bewertungen ist. Miro verwendet einen hybriden Ansatz zur Datenspeicherung, bei dem die direkt auf dem Karten-Widget gespeicherten Daten minimiert werden und zusätzliche Details abgerufen werden, wenn der Nutzer den Bearbeitungsmodus öffnet.

### Datenaufbewahrung der gespeicherten Informationen bei Miro

Alle importierten Trello-Daten, die in Miro gespeichert werden, halten sich streng an Miros Standardrichtlinie zur Datenaufbewahrung. Diese Richtlinie wird konsistent auf alle Kundendaten angewendet, um einen einheitlichen Ansatz für das Management des Datenlebenszyklus zu gewährleisten.

## Authentifizierung und Autorisierung

Die Trello-Integration initiiert einen Authentifizierungsflow, wenn ein Nutzer erstmals mit der Integration interagiert. Die Autorisierung innerhalb von Trello erfolgt durch den Integrationsdienst. Für jeden einzelnen Nutzer erstellt Miro ein Konto beim Integrationsdienst, und diese Anmeldeinformationen werden anschließend für alle Nutzerinteraktionen mit der Integration verwendet.

Die Integration erfordert in der Regel die Genehmigung eines Trello-Admins, um die Integrations-App im Ökosystem ihrer Organisation zu autorisieren. Zusätzlich müssen einzelne Nutzer die Miro Trello-Integration über die OAuth-Autorisierungsseite von Trello autorisieren, wenn sie erstmals versuchen, einen Trello-Link einzubetten.

### Erforderliche Autorisierungs-Geltungsbereiche

Der Autorisierungs-Geltungsbereich kann je nach spezifischem Drittanbietersystem variieren. Für Kartenmanagement-Integrationen wie Trello erfordert Miro jedoch im Allgemeinen den Zugriff auf folgende Daten:

| Geltungsbereich | Beschreibung |
| --- | --- |
| Karten (lesen und schreiben) | Erlaubt der Integration, vorhandene Karten zu lesen sowie Karten in Trello zu erstellen oder zu ändern. |
| Mitglieder (lesen) | Erlaubt der Integration, Mitgliederinformationen in Trello zu lesen, typischerweise zum Zuweisen von Karten oder Anzeigen von Mitgliedsnamen. |
| Labels (lesen) | Erlaubt der Integration, Labels, die zu Karten in Trello gehören, zu lesen. |
| Boards (lesen) | Erlaubt der Integration, Boardinformationen und Listen in Trello zu lesen. |

### Was in Miro gespeichert wird und wie

Miro speichert sowohl autorisierungsbezogene als auch unfurling-bezogene Daten für die Trello-Integration sicher:

- **Autorisierungsbezogene Daten:** Dazu gehören Zugriffstoken und Werte für Erneuerungstoken, die für eine begrenzte Dauer von einigen Tagen in der Miro-Datenbank gespeichert werden. Diese Token werden nach Ablauf automatisch mithilfe des Erneuerungstokens aktualisiert, um kontinuierlichen Zugriff zu gewährleisten. Alle in der Datenbank für diese Integration gespeicherten Daten sind mit dem 256-Bit Advanced Encryption Standard verschlüsselt, was eine robuste Sicherheitsschicht bietet.
- **Entfaltungsbezogene Daten:** Dazu gehören Kartentitel, die als Teil der Miro-Boards selbst gespeichert werden. Zusätzlich werden Titel und verschlüsselte Verweise auf diese Elemente in einem internen Dienst gespeichert, der ebenfalls durch Verschlüsselung (Verwaltung von Verschlüsselungsschlüsseln) gesichert ist.

### Widerrufen eines Tokens

Falls erforderlich, können Admins oder einzelne Nutzer die für die Trello-Integration bereitgestellten Tokens widerrufen. Nutzer können entweder den Integrationskarten-Picker öffnen, das Drei-Punkte-Menü in der oberen rechten Ecke anklicken und **Integrations-Einstellungen** auswählen, oder über den **Reiter Apps** in den Miro-Team-Einstellungen auf die Integrationseinstellungen zugreifen, die spezifische Integration finden und darauf klicken. Auf der Einstellungsseite kann die Autorisierung durch Klicken auf die **Trennen**-Schaltfläche widerrufen werden. Nach dieser Aktion wird Miro den Zugriff auf Trello widerrufen und das zugehörige Konto des Nutzers löschen. Für die Team-Ebene-Deinstallation können Admins spezifische Schritte im Abschnitt „Fehlerbehebung & FAQs (Admin)“ befolgen.

## Wie man die Trello-Integration einrichtet

Der Einrichtungsprozess für die Miro + Trello-Integration umfasst unterschiedliche Schritte für Admins und Nutzer, um eine kontrollierte Bereitstellung innerhalb einer Organisation zu gewährleisten.

1. **Aktive Konten sicherstellen:** Vor der Installation sicherstellen, dass sowohl aktive Miro- als auch Trello-Konten verfügbar sind.
2. **Installation auf Team-Ebene (Admin-Aktion):**
   - Administratoren müssen die Trello-Integration möglicherweise explizit für ihr Miro-Team autorisieren. Teammitglieder können die Integration nur nutzen, wenn sie auf Team-Ebene installiert wurde.
   - Ein Miro-Team-Admin kann die App direkt installieren, indem er ein Miro-Board öffnet, **Tools Media & Integrations (+)** auswählt, nach "Trello" sucht und auf **Verbinden** klickt, um die Integration zu autorisieren. Wenn ein Miro-Team-Admin diese Aktion durchführt, wird die App automatisch autorisiert und installiert, ohne dass eine weitere administrative Genehmigung erforderlich ist.
3. **Nutzeranfrage und Admin-Freigabefluss (falls zutreffend):**
   - In Organisationen, in denen eine strikte administrative Zustimmung erforderlich ist, kann ein Nicht-Admin-Nutzer in einem für die Trello-Integration konfigurierten Miro-Team einen Trello-Link auf ein Miro-Board einfügen. Diese Aktion könnte ein Dialogfeld mit der Aufforderung zur "App-Installationsanfrage" für den Nutzer auslösen, sodass er administrative Zustimmung einholt.
   - Die zugewiesenen Admins können diese ausstehende Anfrage dann über ihre Miro- oder Trello-Administrationskonsolen prüfen und genehmigen, abhängig vom spezifisch konfigurierten Zustimmungsfluss.
4. **Individuelle Nutzerverbindung:**
   - Nachdem die Integration erfolgreich auf Teamebene von einem Admin installiert und autorisiert wurde, klicken die einzelnen Nutzer auf **Verbinden** im Trello-Widget, das auf dem Miro-Board erscheint.
   - Die Nutzer werden dann zu einer Trello-Autorisierungsseite weitergeleitet, auf der sie Miro den Zugriff auf ihr persönliches Trello-Konto gewähren und so ihre persönliche Autorisierung zum Einbetten und Interagieren mit dem Inhalt bestätigen.

## Sicherheits- und Compliance-Erwägungen

### Zugriffsbeschränkung auf Quelldatei

Um sicherzustellen, dass der Zugang zu eingebetteten Trello-Daten auf dieselben Personen beschränkt bleibt wie auf dem ursprünglichen Trello-Board, müssen die Admins der Miro-Organisation strenge Kontrollen über die Board-Freigabe und den Export von Inhalten aufrechterhalten. Während die Kernintegration von Trello individuelle Berechtigungen für die Live-Interaktion respektiert, könnte jeder Export oder statische Snapshot von Board-Inhalten potenziell Daten für unbefugte Personen zugänglich machen, wenn das Miro-Board nicht sicher verwaltet wird.

### Fehlerbehandlung

Die Integration ist mit einer stabilen UI-Fallback-Option und Fehlerbehandlung ausgestattet, falls es zu Ablehnungen von Drittanbietern bei Karten-Datenaktualisierungen kommt.

### Zusatz zur Datenverarbeitung bei Miro (DPA)

Für umfassende rechtliche und Compliance-Details zu Miros Datenverarbeitungspraktiken sollten Admins das [Miro Data Processing Addendum](https://miro.com/legal/customer-data-processing-addendum/) konsultieren.

## Fehlerbehebung & FAQs

### Wie kann die Integration deaktiviert werden (Deinstallation auf Team-Ebene)?

Ein Miro-Team-Admin kann die Trello-Integration auf Team-Ebene deinstallieren. Diese Aktion deaktiviert die Integration für alle Teammitglieder. Dazu gehen Sie zu **Integrationen & Apps** in den Team-Einstellungen. Finden Sie "Trello" oder "Trello Kartenmanagement" in der Liste der installierten Apps, scrollen Sie nach unten und klicken Sie auf **Für das Team deinstallieren**.

### Wie kann die Integration deaktiviert werden (individuelle Deinstallation)?

Einzelne Nutzer können die Integration für sich selbst deinstallieren. Gehe in deinen Miro-Einstellungen zu **Apps & Integrations**. Suche "Trello" oder "Trello Card Management" und klicke auf **Für mich deinstallieren**.

### Welche Admins können die Trello-Integration für ihr Team installieren?

Nur Miro-Team-Admins können die App direkt installieren. Wenn ein Miro-Team-Admin eine Trello-URL auf ein Miro-Board einfügt, wird die App automatisch autorisiert und installiert, ohne dass weitere Schritte erforderlich sind.

### Welche Verfügbarkeitsanforderungen gibt es für die Trello-Integration?

Die Trello-Integration ist für Miros Business- und Enterprise-Preispläne verfügbar. REST API

### Müssen Admins die Trello-Integration für ihr Team autorisieren?

Ja, Admins müssen möglicherweise die Trello-Integration für ihr Miro-Team genehmigen. Teammitglieder können die Trello-Integration nur nutzen, wenn sie auf Teamebene installiert wurde.
