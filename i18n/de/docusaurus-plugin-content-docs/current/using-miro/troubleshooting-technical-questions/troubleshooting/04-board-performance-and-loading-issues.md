---
title: Board-Performance und Probleme beim Laden
article_id: 360013588560
translation_id: 360013588560
locale: de
sidebar_position: 4
created_at: '2020-05-06T08:17:24Z'
updated_at: '2025-04-01T16:57:11Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Entdecke Tipps zur Verbesserung der Board-Performance während gemeinsamer Sitzungen und bei großen Boards und behebe Probleme wie langsame Performance und Navigation, Einfrieren des Boards und endloses Laden.

## So kannst du die Board-Performance verbessern

Die Leistung des Boards kann sich während **kollaborativer Sitzungen** mit vielen Nutzern sowie bei **großen Boards** mit viel Inhalt verlangsamen.

Tipps für kollaborative SitzungenTipps für große Boards

Die steigende Anzahl von Nutzern auf einem Board und ihre intensive Aktivität können die Performance des Boards beeinflussen.  Nutzer mit älteren und weniger leistungsfähigen Geräten haben ein höheres Risiko für Leistungseinbußen./span>

**Wenn du an einer kollaborativen Sitzung teilnimmst, solltest du Folgendes beachten:**

- alle überflüssigen Tabs und Fenster zu schließen oder zu minimieren, wenn du in einem Desktop-Browser arbeitest [Browser arbeitest](../technical-guidelines/02-supported-browsers-browser-restrictions.md)
- Blende die Cursor der Mitwirkenden aus und schließe alle Seitenleisten
- Vermeide das gleichzeitige Auswählen und Ändern mehrerer Board-Objekte
- Minimiere die Navigation auf dem Board
- Wenn du von einem Laptop aus auf Miro zugreifst, stelle sicher, dass du dich im Hochleistungsmodus und nicht im Energiesparmodus befindest.

**Wenn du eine kollaborative Sitzung in Miro planst:**

- Lade Nutzer ein, die als Betrachter keinen Bearbeitungszugriff benötigen.  Erfahre, wie du die [Zugriffsrechte auf Boards](../../sharing-boards/01-board-access-rights.md) einrichtest.
- Achte darauf, dass die Board-Inhalte gut organisiert sind. Richtlinien dazu findest du unter **Tipps für große Boards** auf dem zweiten Tab oben.

Die maximale Anzahl von Objekten, die du zu einem Board hinzufügen kannst, beträgt 100.000.  Allerdings kann die Leistung ab 1.000 Objekten beeinträchtigt werden. Wir empfehlen, die Anzahl der Objekte auf dem Board unter 5.000 zu halten.
So findest du heraus wie viele Objekte auf deinem Board sind:

- Wähle alle Objekte auf dem Board aus (Strg+A für Windows, cmd+A für Mac, oder ziehe ein Auswahlfeld um alle deine Objekte).
- Das Kontextmenü wird dort angezeigt, wo du die Gesamtzahl der Objekte siehst.
- Klicke auf **Filter**, um die Anzahl der Objekte nach Typ anzuzeigen.

![Anzahl-der-Objekte.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/25736281544466_number-of-objects.gif)
*Die Anzahl der Objekte auf einem Board messen*

Neben der Anzahl der Objekte können auch schwerere oder komplexere Objekte (insbesondere hochgeladene Dateien und Dokumente) dein Board verlangsamen.

Damit ein großes Board möglichst schnell bleibt, solltest du es aufgeräumt halten:

- Lösche unnötige Inhalte, insbesondere große, hochgeladene Dateien und Dokumente (z. B. Vektor-PDFs mit vielen Details oder hochauflösenden Bildern).
- Konvertiere große PDFs und Bilder in hoher Auflösung in PNG/JPG-Dateien und lade sie erneut auf das Board hoch.
- Verkleinere den Inhalt deines Boards, wenn er auf einer Zoomstufe von 100 % zu groß aussieht:
  - Geh zur Map rechts unten und stelle den Zoom auf 100 %.
  - Wenn dein Inhalt auf dieser Zoomstufe zu groß aussieht, wähle ihn mit **Strg + A** (für Windows) oder **Cmd + A** (für Mac) aus und verkleinere ihn.
  - Erwäge auch die Verkleinerung großer Bilder
    **![Größe-der-Boards-Objekte-ändern.gif](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/25736308553874_resize-board-objects.gif)**
    *Downscaling von Inhalten*
- [Löse Kommentare auf](../../facilitation-tools/asynchronous-tools/01-comments.md)
- Wandle [Handschrift](../../essential-tools/10-pen.md) in Bilder um:
  - Mache einen Screenshot von einer Zeichnung
  - Lade ihn auf das Board hoch
  - Lösche die Zeichnung
- Wenn möglich, teile das Board in mehrere Boards auf:
  - Kopiere einen Teil des Board-Inhalts, indem du ihn markierst und **Strg +C** (für Windows) oder **Cmd + C** (für Mac) drückst
  - [Erstelle ein neues Board](../../../getting-started/start-here/your-first-board/01-create-a-miro-board.md) und füge den Inhalt in das Board ein.
  - Lösche den kopierten Inhalt aus dem ursprünglichen Board.

## So behebst du Probleme in Bezug auf schlechte Performance oder endloses Laden

Dein Gerät, die Internetverbindung, dein Browser und andere Faktoren können die Board-Performance und die Ladegeschwindigkeit beeinflussen.  Wenn du eine schlechte Performance feststellst oder dein Board oder dein Dashboard in einem Browser, einer Desktop-App, auf einem Tablet oder einem mobilen Gerät nicht lädt, probiere unsere Schritte zur Fehlerbehebung aus.

:::warning
Bevor du die unten aufgeführten Lösungen ausprobierst, schaue auf der [Miro-Statusseite](https://status.miro.com/) nach Meldungen über eine Leistungsbeeinträchtigung.
:::

Browser Desktop-App Tablet, Mobilgerät

1. 1. Öffne Miro im Inkognito/span>[-Modus (privat)](https://support.google.com/chrome/answer/95464) **und/oder in einem** anderen BrowserWenn Miro im Inkognito-Modus oder in einem anderen Browser funktioniert, lösche den Cache und die Cookies deines Browsers.

**So löschst du die Daten der Miro-Website in Chrome**

1, Gehe auf https://miro.com/ und öffne die /span>[Developer Tools](https://miro.com/) von Chrome (**Befehl + Option + J****auf Mac***,* Strg + Umschalt + J **auf Windows***)* Wähle den Tab **App > Speicher**. Klicke auf **Websitedaten löschen**.​ Dadurch sollten alle Miro-Daten, die in deinem Chrome-Browser gespeichert sind, entfernt werden und du kannst eine neue Sitzung starten. Bitte beachte, dass du von deinem Miro Profil abgemeldet wirst![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)*Die Option zum Löschen der Website-Daten in Chrome*

Möglicherweise musst du auch den Browser auf die neueste Version aktualisieren oder bestimmte Erweiterungen deaktivieren. Bitte sieh dir die Liste der [unterstützten Browser](../technical-guidelines/02-supported-browsers-browser-restrictions.md) an.

2. Überprüfe deine Internetverbindung. Wenn die Bandbreite deines Netzwerks nicht das Minimum von 8 Mb/s erreicht, wechsle zu einem anderen, möglichst schnelleren Netzwerk.

3. Stelle sicher, dass dein Gerät die [**Systemanforderungen**](../technical-guidelines/01-system-requirements.md) erfüllt:

- CPU – 3 GHz (2 Kerne/4 Threads)
- RAM-Speicher – 8 GB

4. Wenn du mit einem Laptop auf Miro zugreifst, stelle sicher, dass du es **im** Hochleistungsmodus/span> und nicht im Energiesparmodus verwendest.

5. 5. Wenn du ein Problem mit bestimmten Boards hast, versuche, [sie zu duplizieren](../../managing-boards/03-how-to-duplicate-a-board.md)/span> **und prüfe, ob das Problem auf dem kopierten Board weiterhin besteht.**Für Personen, die Miro nicht laden und aufrufen können:

6. 6. Überprüfe, ob deine Verbindung WebSockets unterstützt. /span> Mehr über WebSockets und Schritte zur Fehlerbehebung findest du unter Miro zu erlaubten Apps hinzufügen

7. Prüfe, ob dein Browser **WebAssembly** unterstützt. Miro nutzt WebAssembly, um den Inhalt von Boards zu erstellen. Wenn dein Browser, deine Erweiterungen oder deine Sicherheitseinstellungen WebAssembly blockieren, können Boards möglicherweise nicht geladen werden. Um zu überprüfen, ob dein Browser WebAssembly unterstützt, kannst du [diese Testseite](https://wasm.joway.io/) öffnen. Wenn das nicht der Fall ist, erkundige dich bei deinem IT-Team oder überprüfe deine Browsereinstellungen, um sicherzustellen, dass WebAssembly **erlaubt** ist.

8, Erkundige dich bei deiner IT-Abteilung, ob dein Unternehmen Firewalls oder einen Proxy verwendet, die Miro möglicherweise blockieren. Folge den Anweisungen im folgenden Artikel, um Miro in die Zulassungsliste aufzunehmen oder eine Umgehung einzurichten: Miro zu erlaubten Apps hinzufügen.

Wenn das Problem weiterhin besteht, [wende dich an den Miro-Support](../../tools/troubleshooting/06-contacting-miro-support.md) und sende uns [die Protokolle der Browser-Konsole](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

1. Überprüfe, ob es bei einer [**Webversion**](https://miro.com/app/dashboard/) zu langen Ladezeiten und einer langsamen Leistung kommt. Wenn du über die Webversion nicht auf Miro zugreifen kannst, versuche es mit der Anleitung zur Fehlerbehebung für Browser
2. Wenn du keine Probleme in deinem Browser hast, kannst du die **App-Daten zurücksetzen**.

   **App-Daten auf Windows zurücksetzen**

   Drücke Alt, klicke in der oberen rechten Ecke auf **Hilfe** und wähle **Anwendungsdaten zurücksetzen** aus:

   ![reset_app_data_on_Windows.jpg](https://help.miro.com/hc/article_attachments/12305900586898)
   *Die App-Daten in der Desktop-App für Windows zurücksetzen*

   Wenn du das Menü nicht finden kannst, verwendest du wahrscheinlich die App, die du aus dem MS Store heruntergeladen hast. Um in diesem Fall die App-Daten zurückzusetzen, öffne die **Windows-Einstellungen**> **Apps**>Apps und Features > suche in der Liste nach Miro > Erweiterte Optionen > Zurücksetzen.

   **So setzt du die App-Daten für macOS zurück**

   Klicke in der Miro-App im oberen Menü auf **Hilfe** und wähle **Anwendungsdaten zurücksetzen** aus:

   ![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
   *Die App-Daten auf dem Mac zurücksetzen*
   {
3. Wenn das Problem weiterhin besteht, versuche die App zu löschen und sie [**erneut zu installieren**](https://miro.com/apps/).

Wenn du weiterhin Probleme hast, [wende dich an den Miro-Support](../../tools/troubleshooting/06-contacting-miro-support.md) und sende uns [die Konsolenprotokolle der App](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md) zu.

1. Überprüfe deine Internetverbindung. Wenn die Bandbreite deines Netzwerks nicht das Minimum von 8 Mb/s erreicht, wechsle zu einem anderen, möglichst schnelleren Netzwerk.
2. Stelle sicher, dass dein Gerät diese **technischen Anforderungen** erfüllt:

- Miro auf Tablets:– 6 GB RAM– iOS 12.0 oder höher, Android 6.0 oder höher, Windows 10-Version 1607 oder höher– Bildschirmauflösung von 768 × 1024 Pixeln oder höher
- Miro auf dem Handy:- iOS 12.0 oder höher- Android 6.0 oder höher

Lösche die App und **installiere sie erneut** auf deinem Gerät.

**Für iPad-Nutzer:**Beachte, dass die Leistungsverschlechterung des Boards auf dem iPad durch die RAM-Beschränkungen des iPads verursacht werden kann. Probiere dann Folgendes aus:

1. Schließe alle unnötigen Hintergrundanwendungen, bevor du Miro verwendest – dies sollte die Performance verbessern.
2. Arbeite auf kleineren Boards – dies sollte die Systembelastung durch die App verringern.
3. Wechsle auf ein anderes Gerät (Laptop oder Computer) mit besserem RAM und verwende die Browserversion von Miro.

## So behebst du typische Probleme

Wird synchronisiert ... Bitte warten Verbindung wird wiederhergestellt/span>

Die Pop-up-Benachrichtigung **Wird synchronisiert …**  Bitte warten bedeutet normalerweise, dass eine große Menge verarbeitet wird und die erforderliche Leistung fehlt, um den Vorgang in der erwarteten Zeit abzuschließen. Die Nachricht kann erscheinen, wenn du auf einem extrem großen Board arbeitest und beispielsweise viele Dinge, wie Objekte, verschiebst oder wenn es zu einem Paketverlust kommt. Auch wenn dein Board relativ einfach aussieht, können große Objekte wie hochauflösende Bilder, PDF-Dateien, Stift-Zeichnungen (denn dies sind Vektorgrafiken, die schwer zu rendern sind) oder Tabellen zu einer Leistungsabnahme führen, die diese Nachricht auslöst.

Teile dein Board in mehrere kleinere Boards auf, indem du deinen Inhalt kopierst und in ein neues Board einfügst – das könnte das Problem beheben.  Wenn das nicht hilft:

- Vergewissere dich, dass dein Gerät die Mindestanforderungen erfüllt und dass dein Browser die aktuellste Version hat.
- Wenn du viele Tabs im Browser offen hast, schließe sie oder friere sie ein, bevor du in Miro arbeitest, damit dein Browser seine gesamte Rechenleistung der Miro-App widmen kann, anstatt sie auf mehrere Tabs aufteilen zu müssen.
- Teste Miro im Inkognito-Modus (privat) (um die Möglichkeit einer Beeinträchtigung durch Browser-Erweiterungen auszuschließen) und in einem anderen Browser. Schließe bei Bedarf alle Browser-Tabs und Anwendungen, die im Hintergrund ausgeführt werden.
- Leere den Cache und die Cookies deines Browsers, starte deinen Browser neu und aktualisiere die Seite, indem du mehrmals auf F5 (oder Strg/Cmd + R) klickst.
- Wenn du Probleme mit spezifischen Boards hast, versuche, sie zu duplizieren, und prüfe dann, ob das Problem weiterhin dort besteht. Außerdem kannst du versuchen, ein Board mit weniger Elementen oder ein kleineres Board zu öffnen, um zu sehen, ob das Problem weiterhin auftritt.
- Wenn du ein VPN verwendest, schalte es aus und schau, ob das Problem weiterhin besteht.
- Dupliziere das Board und überprüfe, ob der Fehler auf dem neuen Board reproduziert wird.

Im Allgemeinen kann der Fehler **Verbindung wird wiederhergestellt …**, **Verbindung wiederhergestellt** in folgenden Fällen auftreten:

- Wenn es auf deiner Seite Probleme mit der Verbindung gibt.  Stelle sicher, dass deine Netzwerkverbindung die Mindestanforderungen erfüllt. Versuche eventuell zu einem schnelleren Netzwerk zu wechseln.
- Wenn du auf mehreren großen Boards arbeitest, die im selben Browser geöffnet sind.  Wenn das der Fall zu sein scheint, schließe alle anderen Tabs und Anwendungen, die gerade ausgeführt werden, in deinem Browser und aktualisiere die Browser-Seite.

Überprüfe auch deine WebSocket-Verbindung (vor allem, wenn du Probleme bei allen Boards hast, selbst bei den kleinsten).  Kontaktiere deine IT-Abteilung und bitte sie, die WebSocket-Verbindungen auf den Ports 80 und 443 (SSL) zu aktivieren und [zu überprüfen, ob es einen anderen Grund geben kann](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)/span>.

## Häufige Fragen

*Hängt die Board-Performance vom Preisplan ab, den ich verwende (kostenlos/kostenpflichtig)?*

Nein, dein Preisplan hat nichts mit der Board-Performance zu tun.

*Wirken sich die Freigabeeinstellungen des Boards auf die Performance aus?*

Die Freigabeeinstellungen sollten die Board-Performance nicht beeinflussen, aber die Anzahl der Nutzer in deinem Board kann sie beeinflussen.  Wende die oben genannten „Tipps für kollaborative Sitzungen“ an.
