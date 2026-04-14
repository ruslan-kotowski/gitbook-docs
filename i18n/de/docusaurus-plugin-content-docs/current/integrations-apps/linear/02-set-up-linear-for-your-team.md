---
title: "Linear (Beta) f\xFCr dein Team einrichten"
article_id: 30630697364626
translation_id: 30630697364626
locale: de
sidebar_position: 2
created_at: '2025-10-29T14:09:41Z'
updated_at: '2026-02-23T11:23:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Die Linear-Integration wird technisch über eine REST-API umgesetzt. Für Authentifizierungs- und Autorisierungszwecke wird das branchenübliche OAuth 2.0-Protokoll verwendet. Ein wesentlicher Bestandteil dieser Architektur ist eine einheitliche API-Plattform, die als Subprozessor für Drittanbieterdaten fungiert und Authentifizierung, Normalisierung und Synchronisierung über verschiedene API-Anbieter hinweg verwaltet.

## Daten Fluss

Das Verständnis des Datenflusses ist entscheidend für die Verwaltung von Sicherheit und Compliance.

### Hochrangiges Sequenzdiagramm

Erstellen eines Linear Karten-Widgets

![Asana Cards (BETA) (1).jpg](images/30631701394962_Asana%20Cards%20(BETA) (1).jpg)

Aktualisieren eines Linear Karten-Widgets

![Asana Cards (BETA) (1).jpg](images/30631701394962_Asana%20Cards%20(BETA) (1).jpg)

### Lineardaten in Miro

Wenn Nutzer Lineare Vorgänge auf ein Miro-Board importieren, sind die folgenden Daten integraler Bestandteil der Miro-Canvas:

- Titel
- Beschreibung
- Zugewiesener (Name/E-Mail-Adresse)
- Status
- Priorität

Diese Auflistung ist entscheidend für die Datenverwaltung und bestätigt, welche sensiblen Daten in die Miro-Umgebung gelangen. Beachten Sie, dass benutzerdefinierte Felder nicht unterstützt werden.

### Datenaufbewahrung

Alle importierten Linear-Daten unterliegen strikt der Standard-Datenaufbewahrungsrichtlinie von Miro, die konsequent auf alle Kundendaten angewendet wird.

## Authentifizierung und Autorisierung

Bei der ersten Interaktion initiiert die Linear-Integration einen Authentifizierungsablauf. Für jeden Nutzer erstellt Miro Anmeldeinformationen mit dem Integrationsdienst für nachfolgende Interaktionen.

Die Integration erfordert in der Regel eine Genehmigung durch einen Linear-Admin.

### Erforderliche Autorisierungs-Geltungsbereiche

| Geltungsbereich | Beschreibung |
| --- | --- |
| Sammlungen | Zugriff auf Sammlungen von Vorgängen. |
| Nutzer | Nutzerinformationen zur Zuordnung/Anzeige lesen. |
| Vorgänge | Vorgänge in Linear lesen, erstellen, modifizieren. |

## Was wird in Miro gespeichert und wie

- **Autorisierungsbezogene Daten:** Tokens werden für mehrere Tage verschlüsselt mit AES-256 in der Miro-Datenbank gespeichert.
- **Entfaltungsbezogene Daten:** Vorgangs-Titel werden mit verschlüsselten Referenzen gespeichert.

### Widerrufen eines Tokens

Das Widerrufen von Tokens kann über die **Integrations-Einstellungen** oder die **Apps**-Tabs erfolgen, indem **„Trennen“** ausgewählt wird. Diese Aktion entfernt den Zugriff auf Linear und löscht die Anmeldeinformationen des Nutzers.

## Wie man die Linear-Integration einrichtet

Schritte für sowohl Admins als auch Endnutzer gewährleisten eine kontrollierte Bereitstellung.

1. **Stelle aktive Konten sicher:** Miro- und Linear-Konten müssen aktiv sein.
2. **Installation auf Teamebene (Admin-Aktion):**
   - Admins müssen die Linear-Integration auf Teamebene genehmigen.
   - Installation über **Tools Media & Integrations**, „Linear“ suchen und verbinden.
3. **Nutzeranfrage und Admin-Genehmigung:**
   - In Organisationen mit striktem Zustimmungserfordernis kann das Einfügen eines Linear-Links eine Anfrage zur Admin-Genehmigung auslösen.
   - Admins können die Genehmigung über die Miro- oder Linear-Konsole erteilen.
4. **Individuelle Nutzungsverbindung:**
   - Nutzer verbinden sich über das Linear-Widget und die OAuth-Autorisierung.

## Sicherheit und Compliance

### Zugriffsbeschränkung auf Quelldatei

Das Aufrechterhalten strenger Board-Freigabekontrollen stimmt die Linear-Berechtigungen mit Miro ab.

### Fehlerbehandlung

Die Integration verfügt über einen eleganten UI-Fallback für Ablehnungen von Drittanbietern.

### Datenverarbeitungszusatz von Miro (DPA)

Sieh dir [Miros Datenverarbeitungszusatz](https://miro.com/legal/customer-data-processing-addendum/) für detaillierte rechtliche und Compliance-Informationen an.

## Fehlerbehebung & FAQs

### Integration deaktivieren (Team-Ebene)

Administratoren können in den **Teameinstellungen Apps & Integrationen** "Linear" auswählen und auf **Für Team deinstallieren** klicken.

### Integration deaktivieren (Einzelperson)

Nutzer können zu **Apps & Integrationen** navigieren und "Für mich deinstallieren" für Linear auswählen.

### Admin-Berechtigungen

Nur Miro-Team-Admins können die App direkt installieren. Automatische Setups erfolgen, wenn eine Linear-URL auf ein Board eingefügt wird.

### Verfügbarkeitsanforderungen

Die Integration mit Linear ist für Business- und Enterprise-Preispläne verfügbar.

### Anforderung der Admin-Autorisierung

Ja, eine Autorisierung auf Teamebene durch Admins ist notwendig, um Teamzugriff zu ermöglichen.
