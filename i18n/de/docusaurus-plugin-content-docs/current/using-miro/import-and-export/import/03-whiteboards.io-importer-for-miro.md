---
title: "Whiteboards.io Importer f\xFCr Miro"
article_id: 20624350720402
translation_id: 20624350720402
locale: de
sidebar_position: 3
created_at: '2024-08-07T16:30:40Z'
updated_at: '2026-01-19T14:08:30Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
---

Der Whiteboards.io Importer für Miro von ServiceRocket ist eine benutzerfreundliche Lösung, die den Import von Daten aus dem [Whiteboards.io](https://whiteboards.io/) App in [Miro](https://miro.com/app/dashboard/). Lade deine mit dem Whiteboard erstellten Backups schnell und einfach hoch.

Hol dir noch heute deinen Zugriff auf den Importeur. Besuche `https://www.servicerocket.com/miro/whiteboards-io-miro-migration` für weitere Informationen.

## **Boards von Whiteboards.io exportieren**

1. Anmelden bei [Whiteboards.io](https://whiteboards.io/).
2. Klicke auf der Hauptseite in der Warnstatusmeldung auf Boards exportieren.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeiEjTayvBy6uufihIKif-C14REIupCmqvKKU6_DMUVhT6lrGC01PkVkXOVJENoCmA2piy40VIRGxFT4YGIE870A9TSYnIpSDyY37H1euf5ZsiP_dbN3zMpcp5GOCIRAcsaJonD8obCfo-WSOxfax4HVtuN?key=RrckFddS6o4KjRqYlXDbPw)
*Klicke auf Boards exportieren in der Warnstatusmeldung, um zu starten*

3. Führe die folgenden Schritte aus, um das Board zu exportieren.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeyDxMc_ob24RYp6Rne_MAIXICO3JRrSesUAHtsyJ0hsG3DjTC5iiNg6_b-97m97XkgtjWRbX0uDcmbyBqMz6tGEEayg0eLvmVIUzLNwTizSYtlQBQXIP5XSNMQFTX2psIIE6SnbVo74EQABRH9vDwe9SPK?key=RrckFddS6o4KjRqYlXDbPw)
*Bestätige die richtigen Einstellungen, wenn du dein Board exportierst*

1. 1. Wähle nur das .json-Format aus.
   2. Deaktiviere die Option Medien einschließen (Bilder, Videos und andere Dateien).
   3. Klicke auf Exportieren, um die Einstellungen zu bestätigen und das Board zu exportieren.

4. Eine .zip-Datei wird erfolgreich erstellt.

## **Importieren von Whiteboards.io-Boards in Miro**

1. Öffne dein Miro-Board.
2. Klicke in der Symbolleiste auf Weitere Apps > wähle oder suche nach Whiteboards.io Miro Importer.
3. Klicke auf Datei auswählen, um die (.zip) Datei hochzuladen, die aus dem [Whiteboards.io](http://whiteboards.io/) App.
4. Wähle dann das Board aus, das du importieren möchtest, und klicke auf Importieren.
5. Sobald der Import abgeschlossen ist, zeigt das System den Status des Boards als ABGESCHLOSSEN an.
6. Schließe die App und kehre zur Hauptseite von Miro zurück. Die App importiert die ausgewählten Boards in dein Team Konto.

## **Whiteboards.io Daten Mapping in Miro**

Das Mapping von Daten ist wichtig, um die Datenintegrität, die Konsistenz und die Schemaunterschiede beim Übergang von einer App zur anderen zu wahren. In den folgenden Tabellen sind alle entsprechenden Begriffe, Datenstrukturen, Feldnamen, Formate und mehr aufgeführt.

|  |  |  |
| --- | --- | --- |
| **Whiteboards.io** | **Miro** | **Merkzettel** |
| Text | [Text](https://developers.miro.com/docs/text-1) | k. A. |
| Form | [Form](https://developers.miro.com/docs/shape-1) | - Die Herzform wird als Wolkenform importiert. - Die paperTape Form wird als Flussdiagramm_Input_Output Form importiert. - Ein Symbol wird als Bild importiert. |
| Karte | [Notiz](https://developers.miro.com/docs/stickynote-1) | - Die Schriftformatierung geht bei der Umwandlung in eine Karte verloren. - Die Farbe der Karte geht verloren und die Ausrichtung ist falsch. - Die Größe der Notizen kann unterschiedlich sein. |
| Zeile | [Konnektor](https://developers.miro.com/docs/connector_intro) | k. A. |
| Rahmen | [Rahmen](https://developers.miro.com/docs/frame-1) | Untergeordnete Objekte des Rahmens können nicht mit dem übergeordneten Rahmen verknüpft werden. |
| Freie Auslosung | [Bild](https://developers.miro.com/docs/image-1) (.svg) | k. A. |
| Kommentare | k. A. | In Miro gibt es keine Methode, um dies zu mappen. |
| Datei | [Datei](../../troubleshooting-technical-questions/technical-guidelines/03-supported-file-formats.md) | Dateityp und Dateiformat:   - Bilder - Tabellen und Tabellenkalkulationen - Textdokumente - Präsentationen |
| Bild | [Bild](https://developers.miro.com/docs/image-1) | k. A. |
| iFrame einbetten | [Einbetten](https://developers.miro.com/docs/embed-2) | k. A. |
| Karte Tisch | [Karte](https://developers.miro.com/docs/card-1) und [Rahmen](https://developers.miro.com/docs/frame-1) | Ohne den Spalten- und Swimlane-Namen. |
| Mindmap | [Mindmap](https://developers.miro.com/docs/mind-maps) (Experimentell) | Die Farbe der Umrandung wird nicht unterstützt. |
| GitHub Karte | [Karte](https://developers.miro.com/docs/card-1) | k. A. |
| Jira-Karte | Text mit Jira-Vorgangs-URL | k. A. |
