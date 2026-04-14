---
title: Jira-Karten FAQ
article_id: 360013463739
translation_id: 8247550662674
locale: de
sidebar_position: 17
created_at: '2022-10-24T14:57:22Z'
updated_at: '2025-10-14T19:23:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Dieser Artikel beantwortet die häufigsten Fragen dazu, wie unsere Integration für Jira-Karten aufgebaut ist.

**Sicherheit**

**Wie funktioniert die Jira-Miro-Authentifizierung?**

Siehe die Hilfecenter-Artikel für

- **Jira-Server vor Ort**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Drittanbieter) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira-Datencenter On-Prem**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Drittanbieter) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira-Cloud**
  Wählen Sie auf der Jira-Karteneinstellungsseite aus.
  - [OAuth 2.0](https://help.miro.com/hc/articles/8588617184402) (3LO)

**Werden Daten bei der Übertragung zwischen Jira und Miro gesichert?**

Wir verwenden das TLS-Sicherheitsprotokoll. Es verschlüsselt HTTP-Nachrichten vor der Übertragung und entschlüsselt Nachrichten bei Eintreffen. Wir unterstützen auch gegenseitiges TLS für den [Enterprise-Preisplan](https://help.miro.com/hc/articles/360017730433).

**Wird gegenseitiges TLS unterstützt?**

Ja, [erfahre mehr](https://help.miro.com/hc/articles/4410562720658).

**Bewahrt Miro irgendwelche Jira-Daten des Kunden auf?**

Ja, Miro bewahrt die Daten der Karte auf, die dem Board hinzugefügt werden.

**Wie lange ist die Aufbewahrungsfrist und wie sind die Daten gesichert?**

Für OAuth 1.0 (Jira-Server oder -Datencenter) werden die Daten ebenfalls aktualisiert, wenn die Webhooks während der Einrichtung des Jira-Karten-Plug-ins konfiguriert werden. Die Aufbewahrungsfrist ist unbegrenzt. Es werden nur die allgemeinen Sicherheitsprotokolle von Miro angewendet.

**Können wir die Informationen einschränken, die von Miro abgerufen werden?**

Wir konnten in der [Dokumentation von Atlassian](https://developer.atlassian.com/server/jira/platform/webhooks/) keinen Hinweis finden, wie die Informationen auf nur wenige Felder beschränkt werden können.

**Können wir ein Diagramm mit dem Datenfluss zwischen Jira und Miro haben?**

Detaillierte Informationen finden Sie in [diesem Artikel für Jira-Entwickler](https://developer.atlassian.com/server/jira/platform/oauth/). Wir implementieren unsere Integration gemäß der Atlassian-Dokumentation.

**Wie wird das Token gehandhabt?**

Oauth 1.0: Es wird nur das Zugriffstoken verwendet. Das Zugriffstoken bleibt [5 Jahre lang aktiv, es sei denn,](https://developer.atlassian.com/server/jira/platform/oauth) es wird widerrufen (keine Option zur Anpassung, da diese Richtlinie auf der Atlassian-Seite definiert ist). Du kannst das Jira-seitige Token über die Web-UI widerrufen. Bedenke dabei, dass jedes neue Token die Integration stoppt und eine erneute [Verknüpfung](https://help.miro.com/hc/articles/360019501754#Step_2_-_Connection) erforderlich macht.

OAuth 2.0: Das Zugriffstoken ist 1 Stunde gültig. Das Aktualisierungs-Token ist 90 Tage lang gültig (wenn du die Integration 90 Tage nicht verwendest, musst du dich erneut authentifizieren).

**Wird ein einzelnes Zugriffstoken für den gesamten Jira-Zugriff des Kunden verwendet?**

Alle Miro-Nutzenden, die Jira-Karten importieren, erstellen oder bearbeiten möchten, müssen ihre individuellen Jira-Zugangsdaten verknüpfen. Alle oben genannten Aktionen können nur im Auftrag der individuellen Jira-Zugangsdaten durchgeführt werden.

**Wie werden die Anfragetoken, Zugriffstoken, privaten Schlüssel und anderen OAuth-Geheimnisse/Zugangsdaten gesichert?**

Während der Integration werden nur Zugriffstoken verwendet. Sie sind sicher in der Datenbank gespeichert und werden nur serverseitig verwendet.

Für OAuth 1.0. (Jira-Server und -Datencenter) wird das authToken nur für den Webhook verwendet. Es ist nicht das eigentliche Authentifizierungstoken von OAuth. Anfragen werden über eine verschlüsselte Verbindung gesendet. Der geheime Schlüssel wird automatisch generiert und dem jeweiligen Team zugeordnet.

**Welche Endpunkte nutzt Ihre Integration?**

```
POST /rest/api/2/issue - neuen Vorgang erstellen
```

```
PUT /rest/api/2/issue/id - Vorgang aktualisieren
```

```
GET /rest/api/2/user/picker?query=xx
```

```
GET /rest/api/2/myself
```

```
GET /rest/api/2/filter/favourite
```

```
GET /rest/api/2/issue/picker
```

```
GET /rest/api/2/serverInfo
```

```
GET /rest/api/2/issue/$key
```

```
GET /rest/api/2/issue/createmeta
```

```
GET /rest/api/2/issue/$key/editmeta
```

```
GET /rest/api/2/priority
```

```
GET /rest/api/2/issuetype
```

```
GET /rest/api/2/mypermissions
```

Für OAuth 1.0. (Jira-Server und -Datencenter) verwenden wir zusätzlich:

```
POST /rest/webhooks/1.0/webhook
```

**Funktionieren die Karten mit dem Jira Datacenter?**

Ja. Wir wurden von Atlassian zugelassen und haben bereits viele Kundinnen und Kunden, die Jira-Karten erfolgreich mit dem Datencenter verwenden. Der Installationsprozess ist identisch.

**Welche IPs verwendet ihr, um mit dem Jira-System zu kommunizieren?**

Die Liste unserer statischen IP-Adressen findest du [hier](https://help.miro.com/hc/articles/360017572694).

Beachte, dass diese Adressen nur zur Kommunikation mit dem Jira-System verwendet werden. Die IPs der Miro-App sind dynamisch. Um sicherzustellen, dass alle Funktionalitäten auf den Miro-Boards (einschließlich einiger, die zu den Jira-Karten gehören) erfolgreich ausgeführt werden, bitten wir, [unsere Domains in die Zulassungsliste aufzunehmen](https://help.miro.com/hc/articles/360017572694).

**Können wir Jira mit Miro integrieren, aber die Jira-Vorgänge mit der Sicherheitsstufe „Privat“ blockieren?**

Nein, das ist nicht möglich. Sicherheitsstufen in Jira korrelieren nicht mit Miro.

**Allgemein**

**Können wir Miro mit einem Jira-Server verbinden?**

Da Miro ein Online-Tool ist, kannst du nur eine Verbindung zu Jira herstellen, wenn deine Instanz für das öffentliche Internet zugänglich ist.

**Können wir mehrere Jira-Instanzen gleichzeitig verbinden?**

Ja. Allerdings ist es wichtig zu beachten, dass das Verbinden einer Jira-Instanz die erstmalige Erstellung der Verbindung bedeutet, während eine aktive Verbindung die verlinkte Instanz bezeichnet, die momentan genutzt wird. Eine aktive Verbindung definiert, woher Jira-Karten importiert werden, wenn du die Jira-Karten-App öffnest, und für welche Instanz Nutzer autorisiert sind. Für einen bestimmten Nutzer kann es jeweils nur eine (1) aktive Verbindung geben. Mit OAuth 2.0 kann ein Nutzer jede Jira-Karte bearbeiten, die mit einer verlinkten Instanz verbunden ist, für die er bereits authentifiziert ist. Bei jedem anderen Authentifizierungsprotokoll teilt ein ganzes Team eine aktive Instanz und kann nur Karten von dieser Instanz importieren und mit diesen interagieren. Du kannst mehrere organisationale Einstellungen definieren und zwischen aktiven Verbindungen auf Teamebene wechseln.

**Wie sieht der Migrationsprozess vom Server in die Cloud aus?**

Da sich deine Jira-Basis-URL während der Migration in die Cloud zwangsläufig ändert, wird die Integration ohne Änderungen auf unserer Seite nicht funktionieren. Bitte wende dich an den [Miro-Support](https://help.miro.com/hc/articles/360020185799) für Unterstützung.

**Erstellt Miro einen Webhook pro Team, pro Projekt oder pro Miro-Instanz?**

Wenn du in deinen Miro-Einstellungen den automatischen Webhook aktivierst, erfolgt die Erstellung der Webhooks automatisch. Wenn du die Team-Ebene Autorisierung mit Jira verwendest, erstellt Miro Webhooks pro Team. Wenn du die Organisational-Ebene Autorisierung verwendest, erstellt Miro Webhooks pro Organisation.

**Unterstützt das Jira-Karten-Plugin Next-Gen-Projects?**

Ja, das tut es.

Bitte beachte, dass es derzeit kein Epic Link/Feld gibt, wenn du für ein Next-Gen-Projekt auf Miro eine Jira-Karte erstellst.

**Werden benutzerdefinierte Jira-Felder unterstützt?**

Ja, wir unterstützen fast alle benutzerdefinierten Felder der *Basistypen*. Wenn du ein *komplexes* Datentypfeld hast, wird es möglicherweise nicht unterstützt und verursacht unerwartetes Verhalten bei der Aktualisierung oder Einrichtung von Jira-Karten auf dem Board.

**Was passiert mit bestehenden Jira-Karten, wenn wir auf eine andere Jira-Instanz wechseln?**

Derzeit werden Jira-Vorgänge in Miro nicht mehr aktualisiert, wenn du Jira-Vorgänge in Jira von einem Projekt zu einem anderen verschiebst.

Als Lösung empfehlen wir dir, die URL des Jira-Vorgangs zu kopieren (Strg/Befehl+C) und sie in das Miro-Board einzufügen (Strg/Befehl+V). Somit zeigt die Jira-Karte neue Werte und wird automatisch aktualisiert.

**Was passiert mit den Jira-Karten auf dem Board, wenn ein Board in ein anderes Miro-Team verschoben wird?**

Die Jira-Karten bleiben auf dem Board, aber niemand wird sie noch ändern können (selbst wenn die gleiche Jira-Instanz für das Team konfiguriert ist).

Wenn du eine Karte anklickst, siehst du die Meldung: *„Die JIRA-Karte wurde aus einem anderen Konto importiert“*. Wenn du die Karten bearbeitbar machen möchtest, importiere sie bitte neu in das Board.

**Gibt es zusätzliche Kosten für die Integration der Jira-Karten?**

Jira-Karten sind für alle kostenpflichtigen Preispläne und den Education-Preisplan ohne zusätzliche Kosten verfügbar (Starter-, Business-, Education- und Enterprise-Preispläne).

**Kann ein Nutzer auf alle Jira-Karten im Board zugreifen?**

Die Berechtigungen für die Integration der Jira-Karten stellen sicher, dass Nutzer nur Karten in Jira-Projekten erstellen und bearbeiten können, auf die sie Zugriff haben.

Da alle Widgets auf einem Miro-Board für alle zugriffsberechtigten Personen sichtbar sind, sehen jene ohne Jira-Anmeldeinformationen oder nicht angemessene Anmeldeinformationen die minimierte Jira-Karte auf dem Miro-Board (mit Titel und einigen anderen Feldern), sind aber nicht in der Lage, die Karte aufzurufen, um den gesamten Inhalt zu sehen oder sie zu ändern.

**Hat Atlassian den Support für den Jira Server eingestellt?**

Ja, Atlassian hat den Support für Jira Server ab Februar 2024 eingestellt.

**Unterstützt Miro Planer/Jira-Karten die benutzerdefinierten Jira-Felder: Benutzerdefinierte Vorgangstypen und benutzerdefinierte Abhängigkeiten?**

Ja, beide werden unterstützt. Wenn die Felder **Benutzerdefinierte Vorgangstypen** und **Benutzerdefinierte Abhängigkeiten** in Jira eingerichtet sind *und* der Miro Planer für diese Jira-Instanz authentifiziert ist, sind diese benutzerdefinierten Felder im Planer verfügbar.

**Unterstützt Miro OAuth 2.0 für Jira Data Center?**

Ja. Siehe [Verbinden mit Jira Data Center über OAuth 2.0.](https://help.miro.com/hc/articles/25753304280466)

**Jira-Karten in Tabellen & Zeitachsen**

**Wie kann ich Jira-Vorgänge in Tabellen und Zeitachsen importieren?**

Du kannst eine oder mehrere Jira-Karten direkt in eine Tabelle oder Zeitachse ziehen. Dies ist derzeit die einzige Möglichkeit.

**Werden alle Felder in der Tabelle mit Jira verknüpft?**

Nein, nur fünf Felder in der Tabelle synchronisieren mit Jira in der ersten Version:

Drei systembedingte Jira-Felder:

- Titel
- Beschreibung
- Enddatum (erscheint als Fälligkeitsdatum in Jira)

Zwei benutzerdefinierte Jira-Felder:

- Startdatum
- Schätzung

**Welche Felder in der Tabelle werden nicht mit Jira synchronisiert?**

Die Felder für die zugewiesene Person (Assignee) und den Status werden nicht mit Jira synchronisiert und sind in den Tabellen und in der Zeitachse deaktiviert. Diese Felder und deren Inhalte existieren, sind aber in den Tabellen und auf der Zeitachse weder sichtbar noch editierbar.

Du kannst diese Felder weiterhin direkt in den Jira-Karten im seitlichen Feld bearbeiten. Ziehe einfach die Zeile von der Tabelle oder Zeitachse auf die Arbeitsfläche, um deine Jira-Karte erneut erscheinen zu lassen.

Alle anderen Felder außer den fünf oben genannten (Titel, Beschreibung, Enddatum, Startdatum und Schätzung) werden ausschließlich in Miro gespeichert und nicht mit Jira synchronisiert.

**Warum kann ich ein Feld in der Tabelle oder Zeitachse aus den oben genannten fünf Jira-Feldern nicht bearbeiten?**

Das Feld ist möglicherweise nicht im Bearbeitungsmodus in Jira vorhanden.

Eine einfache Möglichkeit zu überprüfen, ob das Feld im Bearbeitungsbildschirm vorhanden ist oder nicht:

Öffne auf Miro das seitliche Feld der Jira-Karte. Prüfe, ob das Feld im seitlichen Feld vorhanden ist. Ist das Feld nicht vorhanden, musst du es dem Bearbeitungsbildschirm in Jira hinzufügen.

Es gibt einige seltene Fälle, in denen die Felder in Jira bearbeitbar sind, aber nicht im Bearbeitungsbildschirm angezeigt werden. In diesem Fall können diese Felder nicht in Miro bearbeitet werden.

Ist das Feld, das du nicht bearbeiten kannst, **Startdatum** oder **Schätzung**? Falls ja:

Das Feld ist möglicherweise nicht in Jira vorhanden oder fehlt im Bearbeitungsbildschirm (siehe vorheriger Punkt).

Es könnte ein Abbildungsproblem für das Startdatum oder die Schätzung geben, da dies benutzerdefinierte Jira-Felder sind.

Wir bilden diese Felder nach folgender Logik ab:

- **Startdatum**: Wir prüfen Felder mit folgenden Namen: Start Date, StartDate, Target Start
- **Schätzung**: Wir prüfen Felder mit folgenden Namen: Story Points, Story point estimate, Story Point, StoryPoints, StoryPoint
- Wenn das Startdatum- oder Schätzungsfeld nicht einen der oben genannten Namen trägt, kann dies erklären, warum das Bearbeiten nicht funktioniert.

**Warum funktioniert das Bearbeiten des Anfangsdatums oder des Schätzfelds in der Miro-Tabelle oder -Zeitachse entweder nicht oder aktualisiert das falsche Feld in Jira?**

Wir verlassen uns derzeit auf die automatische Zuordnung für die Startdatum- und Schätzfelder in Jira. Da diese in Jira benutzerdefiniert sind, kann es vorkommen, dass mehrere Felder in deiner Jira-Konfiguration den oben genannten Kriterien entsprechen.

Wir wählen den ersten Treffer gemäß der Reihenfolge der oben genannten Feldnamen:

Zum Beispiel, wenn ein Jira-Ticket sowohl das "Story Points"- als auch das "Story point estimate"-Feld enthält, wird das erstgenannte Feld "Story Points" entsprechend der obigen Liste zugeordnet. Daher werden Änderungen im Schätzfeld in der Tabelle das "Story Points"-Feld in Jira aktualisieren und nicht das "Story point estimate".

Im Moment gibt es dafür keine Umgehungsmöglichkeit. Falls dieses Problem auftritt, schicke bitte Feedback an dein Support-Team, damit wir deine Bedürfnisse besser verstehen können, während wir fortschrittlichere Zuordnungsfähigkeiten entwickeln.

**Warum kann ich keine Jira-Karten aus zwei verschiedenen Instanzen in eine Tabelle oder Zeitachse importieren?**

Derzeit unterstützen wir nur eine Jira-Instanz pro Tabelle/Zeitachse. Sobald eine Jira-Karte in eine Tabelle/Zeitachse importiert wird, ist die Tabelle/Zeitachse mit dieser spezifischen Jira-Instanz verknüpft.

Selbst wenn alle Jira-Einträge gelöscht werden, bleibt die Verknüpfung mit der ursprünglichen Jira-Instanz bestehen. Um Karten aus einer anderen Jira-Instanz zu importieren, musst du eine neue Tabelle/Zeitachse erstellen.

**Warum kann ich die Felder Status und Zuständiger für meine Jira-Einträge in einer Tabelle oder Zeitachse nicht sehen oder bearbeiten?**

Derzeit werden die Jira-Status- und Zuständigkeitsfelder in Tabellen und Zeitachsen nicht unterstützt. Wir haben beschlossen, diese Felder in Tabellen und Zeitachsen zu deaktivieren, um Erwartungen zu managen, Verwirrung zu vermeiden und potenziellem Datenverlust vorzubeugen. Die Jira-Status- und Zuständigkeitsfelder und deren Inhalte existieren, erscheinen jedoch nicht in Tabellen oder Zeitachsen.

Du kannst diese Felder weiterhin direkt in den Jira-Karten über das seitliche Feld bearbeiten. Ziehe einfach die Zeile von der Tabelle oder der Zeitachse zurück auf das Canvas, um deine Jira-Karte wieder erscheinen zu lassen.

**Weitere Informationen:**

- [Jira-Karten](https://help.miro.com/hc/articles/360017572434)
- [Wie man Jira-Karten einrichtet und deinstalliert](https://help.miro.com/hc/articles/360019501754)
- [Wie man Webhooks für Jira-Karten einrichtet](https://help.miro.com/hc/articles/360017731113)
- [Mögliche Probleme mit Jira-Karten und dem Jira-Add-on](https://help.miro.com/hc/articles/360017572654)
