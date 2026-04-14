---
title: So findest und meldest du einen Fehler
article_id: 360017731413
translation_id: 360017731413
locale: de
sidebar_position: 7
created_at: '2019-02-11T10:14:28Z'
updated_at: '2025-11-25T16:03:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Wenn du Probleme mit der Leistung hast oder Miro nicht verwenden kannst, erfährst du hier, wie du dem Miro-Support den Fehler meldest.

## Bevor du einen Fehler meldest

1. Auf der [Miro-Statusseite](https://status.miro.com/) kannst du nachsehen, ob es Meldungen über mögliche Leistungsbeeinträchtigungen gibt
2. Überprüfe, ob das Problem auch im [Inkognito-Modus](https://support.google.com/chrome/answer/95464) **(privat)** und in einem **anderen Browser** besteht
3. [Deaktiviere die Browser-Erweiterungen](https://support.box.com/hc/articles/360044196613-How-To-Disable-Plugins-Add-Ons-Extensions-In-Multiple-Browsers). Manchmal kollidieren sie mit den Miro-Prozessen (z. B. bei die Grammatik mit den Text-Widgets).
4. Wenn du in der Desktop-App arbeitest, [setze die App-Daten zurück](../../../getting-started/apps-for-devices/05-desktop-app.md)
5. Wenn du Leistungsprobleme auf einem bestimmten Board hast, versuche es zu [duplizieren](../../managing-boards/03-how-to-duplicate-a-board.md) und überprüfe dann, ob das Problem auch auf dem kopierten Board auftritt
6. Überprüfe unsere Leitfäden zur Fehlerbehebung:

- [Board-Performance und Probleme beim Laden](../../tools/troubleshooting/04-board-performance-and-loading-issues.md)
- [Ich kann mich nicht anmelden](../../tools/troubleshooting/09-i-can't-log-in.md)
- [Ich kann nicht auf ein Miro-Board zugreifen oder es bearbeiten](../../tools/troubleshooting/08-i-can't-access-or-edit-a-miro-board.md)
- [Probleme beim Exportieren des Boards](../../tools/troubleshooting/03-board-export-issues.md)
- [Ich finde mein Board oder meinen Inhalt nicht mehr](../../tools/troubleshooting/11-i-lost-my-board-or-content.md)
- Andere Leitfäden

## So meldest du einen Fehler

Gib so viele Details wie möglich an – dies hilft uns, dein Problem schneller zu verstehen, damit wir dir besser helfen können.

1. Füge eine Beschreibung des Problems hinzu und sende uns Screenshots, GIFs oder ein [kurzes Video](https://chrome.google.com/webstore/detail/openvid-screen-recorder-c/liecbddmkiiihnedobmlmillhodjkdmb). Zusätzlich:

- Wenn das Problem auf einem bestimmten Board auftritt, [gib das Board](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) für [support@help.miro.com](mailto:support@help.miro.com) mit Bearbeitungsrechten frei, wenn möglich.
- Wenn das Problem mit einer bestimmten hochgeladenen Datei verbunden ist, schicke uns die Datei bitte zu

2. Gib dein Gerät, das Betriebssystem und deine Browserversion an
3. Stelle deine Browserkonsolen- und Netzwerkprotokolle oder die Desktop-App-Protokolle zur Verfügung

### So zeichnest du Konsolenprotokolle auf

**So zeichnest du Protokolle der Browser-Konsole auf**

1. Wenn du dich im Miro-Board befindest, **klicke auf die Adressleiste** deines Browsers (führe diesen Schritt aus, wenn das Problem auf einem der Boards auftritt und nicht auf der Einstellungsseite oder dem Dashboard)​![mceclip1.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264821010_mceclip1.png)
2. Drücke **F12** oder **fn + F12**, um die Entwicklertools des Browsers zu öffnen
3. Gehe zum Tab **Netzwerk** aus und markiere **Protokolle aufbewahren**
4. Lade die Seite neu
5. Versuche, das Problem erneut zu reproduzieren
6. Klicke auf das Pfeil-Symbol zum Herunterladen und **exportiere** die Netzwerk-HAR-Protokolle
   ![network_console_logs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264822418_network%20console%20logs.jpg)
7. Wechsele zum Tab **Konsole**, klicke mit der rechten Maustaste auf die Datensätze und wähle **Speichern als**​![save_console_logs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253821970_save%20console%20logs.jpg)
8. Sende uns die  .*log-* und .*har-*Dateien. Wenn die Datei aufgrund ihrer Größe nicht an dein Ticket angehängt werden kann, lade sie in einen beliebigen Cloud-Speicher hoch und schicke uns den Link (erlaube, dass jeder mit dem Link die Dateien herunterladen kann)

**So zeichnest du Protokolle der Desktop-App auf dem Mac auf**

Wenn du einen Fehler in der Desktop-App auf dem Mac feststellst, schicke uns bitte die Protokolldateien.

1. Klicke in der Desktop-App oben links auf **Hilfe**. Wähle **Entwicklertools für Tabs öffnen**​​​​​​​​
   ![open_developer_tools_for_tabs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253822866_open%20developer%20tools%20for%20tabs.jpg)
2. ​Wechsele zum Tab **Netzwerk**.​​​​ Aktiviere das Kontrollkästchen **Protokolle beibehalten**
3. Öffne das Board, das du beheben möchtest (überspringe diesen Schritt, wenn du nicht auf Boards zugreifen kannst)
4. Lade die Seite mit der Tastenkomnination **Strg + R** neu
5. Reproduziere das Problem
6. Klicke auf das Pfeilsymbol zum Herunterladen, um die Netzwerk-HAR-Protokolle zu exportieren:
   ![preserve_logs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253823250_preserve%20logs.jpg)
7. Wechsele zum Tab Konsole, klicke mit der rechten Maustaste auf die Datensätze und wähle **Speichern als.**​![save_as_.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253825042_save%20as%20.jpg)
8. Klicke erneut auf **Hilfe** > wähle **Entwicklertools öffnen** aus und wiederhole die Schritte 2 bis 7. Dadurch wird eine andere Art von Protokoll erfasst, das uns andere Daten liefert, um das Problem für dich weiter zu untersuchen
9. Schicke uns die .log- und .har-Dateien. Wenn die Datei aufgrund ihrer Größe nicht an dein Ticket angehängt werden kann, lade sie in einen beliebigen Cloud-Speicher hoch und schicke uns den Link (gestatte jedem, die Dateien über den Link herunterzuladen).

**So zeichnest du Protokolle der Desktop-App unter Windows auf**

Wenn du einen Fehler in der Desktop-App unter Windows feststellst, schicke uns bitte die Protokolldateien.

1. Wenn du dich in der Desktop-App befindest, drücke die Taste **Alt** > klicke auf **Hilfe** > **Entwicklertools für Tabs öffnen![open_developer_tools_for_tabs_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020264830994_open%20developer%20tools%20for%20tabs%20on%20Windows.jpg)**
2. ​Wechsele zum Tab **Netzwerk**.​​​​ Markiere das Kästchen **Protokolle beibehalten**
3. Öffne das Board, bei dem der Fehler auftritt (überspringe diesen Schritt, wenn du nicht auf Boards zugreifen kannst)
4. Drücke **Strg + R**, um die Seite neu zu laden  **Strg + R**
5. Reproduziere das Problem
6. Klicke auf das Symbol Herunterladen, um die Netzwerk-HAR-Protokolle zu exportieren
   ![preserve_logs.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253823250_preserve%20logs.jpg)
7. Wechsele zum Tab Konsole, klicke mit der rechten Maustaste auf die Datensätze und wähle **Speichern als**​
   ![save_as_.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21020253825042_save%20as%20.jpg)
8. Öffne erneut die **Hilfe** > wähle **Entwicklertools öffnen** aus und wiederhole die Schritte 2 bis 7. Dadurch wird eine andere Art von Protokoll erfasst, das uns andere Daten liefert, um das Problem für dich weiter zu untersuchen
9. Schicke uns die .log- und .har-Dateien. Wenn die Datei aufgrund ihrer Größe nicht an dein Ticket angehängt werden kann, lade sie in einen beliebigen Cloud-Speicher hoch und schicke uns den Link (gestatte jedem, die Dateien über den Link herunterzuladen).

### So erfasst du einen Browserbericht

Wenn du Lade- oder Leistungsprobleme meldest, hilft die Weitergabe von Informationen für erweiterte Browserversionen dem Miro-Support, das Problem zu diagnostizieren. Du findest diese Informationen, indem du einen bestimmten Befehl in die **Adressleiste** deines Browsers eingibst. Im Folgenden findest du, wie du in verschiedenen Browsern auf diese Informationen zugreifen kannst.

- **Chrome**: chrome://version
- **Microsoft Edge**: edge://version
- **Firefox**: about:support (or about:version in some versions)
- **Opera**: opera://about
- **Yandex Browser**: browser://version

> **✏️** Siehe [Miro-Support kontaktieren](../../tools/troubleshooting/06-contacting-miro-support.md).
