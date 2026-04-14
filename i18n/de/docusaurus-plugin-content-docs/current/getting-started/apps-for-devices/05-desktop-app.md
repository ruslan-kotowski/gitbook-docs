---
title: Desktop-App
article_id: 360017572854
translation_id: 360017572854
locale: de
sidebar_position: 5
created_at: '2019-02-11T10:15:04Z'
updated_at: '2025-11-25T16:00:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
---

Starte die Miro Desktop-App in wenigen Sekunden direkt von deinem Startbildschirm aus und arbeite an Boards ohne Ablenkung. Die App unterstützt alle grundlegenden Funktionen der Browser-Version.

:::tip
Lade die Miro-App von [unserer Website](https://miro.com/apps/) herunter.
:::

## Lade die Miro Desktop-App herunter

### Windows

- Windows 64-Bit - [App herunterladen](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.exe)

:::note
Windows 32-bit wird nicht mehr unterstützt und ist nicht mehr verfügbar.
:::

### macOS

- Macs mit Apple Silicon Chips - [App herunterladen](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro.dmg)
- Macs mit Intel Chips - [App herunterladen](https://desktop.miro.com/platforms/darwin/Install-Miro.dmg)

Um herauszufinden, welche Art von Prozessor du hast, gehe wie folgt vor:

1. Klicke auf das Apple-Symbol in der oberen linken Ecke deines Macs.
2. Dadurch wird ein Drop-down-Menü angezeigt. Klicke auf die Option **Über diesen Mac**.

Das Fenster sollte dir die Informationen anzeigen, die du brauchst, einschließlich Prozessor-Typ (Intel oder Apple Silicon).

## Miro auf mehreren Geräten installieren

Miro bietet verschiedene Installationsversionen, mit denen IT-Admins Miro auf Tausenden von Rechnern bereitstellen können. Dafür gibt es zwei Möglichkeiten: die Installation pro Nutzer oder pro Rechner. Für jede dieser Varianten gibt es Versionen mit und ohne automatische Updates. Mit der Version mit automatischen Updates erhalten deine Nutzer die aktualisierte Version der App, sobald sie veröffentlicht wird. Die Variante ohne automatische Updates gibt dir mehr Kontrolle über die Version von Miro, die deine Mitarbeiter verwenden.

### Für Windows

#### Miro in den Programmdateien bereitstellen

Miro kann auch im Verzeichnis „Programme“ installiert werden, so dass es jedem Nutzer eines Geräts zur Verfügung steht, während die Profile getrennt bleiben. Eine einzige Installation auf einem Rechner bedeutet einen geringeren Festplattenbedarf bei der Skalierung, während Miro weiterhin für jeden Nutzer dieses Rechners verfügbar ist. Wenn du dich für die Version mit automatischen Updates entscheidest, beachte, dass für die Installation eines Updates Admin-Rechte erforderlich sind.

- Windows MSI 64 bit mit automatischen Updates - [App herunterladen](https://desktop.miro.com/platforms/win-nsis/Miro-setup.msi)
- Windows MSI 64 bit ohne automatische Updates - [App herunterladen](https://desktop.miro.com/platforms/win-nsis/Miro-no-updates.msi)

#### Miro für einen bestimmten Nutzer bereitstellen

Miro bietet verschiedene Installationsversionen, mit denen IT-Admins Miro für einen einzelnen Nutzer bereitstellen können. Diese Version kann ohne administrative Berechtigungen aktualisiert werden und wird nur für den oder die ausgewählten Nutzer installiert.

- Windows MSI 64 Bit mit automatischen Updates - [App herunterladen](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-setup.msi)
- Windows MSI 64 Bit ohne automatische Updates - [App herunterladen](https://desktop.miro.com/platforms/win32-nsis-pu/Miro-no-updates.msi)

### Für macOS

- Apple Silicon Mac ohne Auto-Updates - [App herunterladen](https://desktop.miro.com/platforms/darwin-arm64/Install-Miro-no-updates.dmg)
- Intel Mac ohne Auto-Updates - [App herunterladen](https://desktop.miro.com/platforms/darwin/Install-Miro-no-updates.dmg)

## Systemanforderungen für die App

### Für Windows

|  |  |  |
| --- | --- | --- |
|  | **Minimum** | **Empfohlen** |
| **CPU** | 3 GHz (2 Prozessorkerne/4 Threads) | 2,8 GHz (4 Prozessorkerne/8 Threads) |
| **RAM** | 8 GB | 16 GB (DDR4) |
| **Betriebssystem** | Windows 10 oder höher für die App aus dem Microsoft Store + Microsoft .NET Framework 4.5 (Bitte beachten Sie, dass die ARM-Version von Windows nicht unterstützt wird) | Neuestes Betriebssystem |
| **Netzwerk** | 8 Mbit/s oder schneller | 32 Mbit/s |

### Für macOS

|  |  |  |
| --- | --- | --- |
|  | **Minimal** | **Empfohlen** |
| **CPU** | 64-bit Intel oder Apple M1 |  |
| **OS** | macOS 12 (Monterey) oder höher | Aktuellstes OS |
| **Netzwerk** | 8 Mbit/s oder schneller | 32 Mbit/s |

Bitte beachte, dass die App mehrere Instanzen auf deinem Gerät ausführen wird:

- Hauptprozess
- Fenster-Prozess (UI-Renderer)
- Hardware-Beschleunigung
- Crash Handler
- + 1 Prozess pro geöffnetem Tab (weil jeder Tab eine Webansicht hat)

Wenn du beispielsweise 3 Tabs während deiner Arbeit geöffnet hast, siehst du 7 Instanzen von Miro.exe. Weitere Informationen zu dieser Architektur findest du [hier](https://www.electronjs.org/docs/glossary#process) und [hier](https://www.chromium.org/developers/design-documents/multi-process-architecture).

## App-spezifische Shortcuts

Die Desktop-App verfügt über zusätzliche [Tastenkombinationen](../../using-miro/working-on-the-board/06-shortcuts-and-hotkeys.md):

- **Strg + R** *(für Windows)* / **Cmd + R** *(für Mac)* um den Tab neu zu laden
- **Strg + W** *(für Windows)* / **Cmd +W** *(für Mac)* um den Tab zu schließen
- **Strg + Q** *(für Windows)* / **Cmd + Q** *(für Mac)* um die App zu beenden
- **Strg + Umschalt + L** *(für Windows)* / **Cmd + Umschalt + L** *(für Mac)* um den Board-Link zu kopieren
- **Strg + ~** *(für Windows)* **/ Cmd + ~** *(für Mac)* zum Zoomen

## App-Aktionen

Die folgende Tabelle zeigt, welche Aktionen in der Miro Desktop-App ein anderes Erlebnis als im Browser bieten könnten:

| Aktion | **Win & Mac-Apps von** [**Miro Apps**](https://miro.com/apps/) |
| --- | --- |
| Als Bild speichern (niedrig, mittel, hoch) | ✔ |
| Als Bild speichern (Vektor) | ✔ |
| Als PDF speichern (niedrig) | ✔ |
| Als PDF speichern (Vektor) | ✔ |
| In eine Tabelle exportieren (CSV) | ✔ |
| Videochat | ✔ |
| Aus einer Tabelle einfügen | ✔ |
| Plugin für Confluence | ✔ |

### Nicht verfügbare Aktionen

Die folgenden Aktionen sind in der Miro Desktop-App nicht verfügbar:

- Besucher können sich nicht anmelden.

  > ✏️ Nur registrierte Miro-Nutzer können sich in der Desktop-App anmelden.
- Keine Option zum Kopieren/Einfügen von Sketch
- Für einige Versionen von Jira Server können Sie aus Sicherheitsgründen keine Jira-Karten bearbeiten.

## Rechtschreibprüfung

Wenn du die Funktion für die automatische Rechtschreibprüfung in der Desktop-App deaktivieren möchtest, gehe wie folgt vor:

- Drücke **Alt** (*nur für Windows*)
- Klicke oben in der Haupt-Navigationsleiste auf**Ansicht**
- Deaktiviere die Schaltfläche **Rechtschreibprüfung anzeigen**

Hinweis: Die Option zur Deaktivierung der Rechtschreibprüfung ist in der App aus dem Microsoft Store nicht verfügbar.

## Mögliche Probleme und wie man sie löst

### So setzt du die App-Daten zurück

In vielen Fällen, in denen ein Problem auftritt (vor allem wenn du Schwierigkeiten mit dem Login hast), hilft es, **die App-Daten zurückzusetzen** und den Speicher der App zu löschen.

:::tip
Falls das Problem nach dem Zurücksetzen der Daten weiterhin besteht, solltest du vielleicht auch die App löschen und sie [die neueste Version herunterladen](https://miro.com/apps/) und erneut installieren.
:::

#### Für Windows

Drücke **Alt > Hilfe** und wähle die Option zum Zurücksetzen der App-Daten, wie im Screenshot unten gezeigt:

![reset app data on Windows.png](../../../../../../docs/getting-started/apps-for-devices/images/21016134171922_reset%20app%20data%20on%20Windows.png)
*Zurücksetzen der App-Daten in der Desktop-App für Windows*

Wenn du das Menü nicht finden kannst, verwendest du wahrscheinlich die App, die du aus dem MS Store heruntergeladen hast. In diesem Fall gehe zu Windows **Einstellungen** > **Apps** > **Apps und Features** > finde **Miro** in der Liste > **Erweiterte Optionen** > **Zurücksetzen**, um die App-Daten zurückzusetzen.

Falls dies nicht unmittelbar weiterhilft, lösche alle App-Dateien aus **C:\Users\username\AppData\Roaming\RealtimeBoard** und **C:\Users\username\AppData\Local\Programs\RealtimeBoard**

> **✏️** Wenn der Ordner **Appdata** versteckt ist, sieh [hier](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) nach, wie er sichtbar gemacht werden kann.

#### Für macOS

Klicke im oberen Menü auf Miro und wähle **App-Daten zurücksetzen** , wie im Screenshot unten gezeigt:

![reset app data on Mac.png](../../../../../../docs/getting-started/apps-for-devices/images/21016120799378_reset%20app%20data%20on%20Mac.png)
*Zurücksetzen der App-Daten auf dem Mac*

Versuche danach, dich erneut in der App anzumelden und prüfe, ob der Vorgang gelöst ist.

Sollte das Zurücksetzen nicht unmittelbar weiterhelfen, öffne ein Finder-Fenster > drücke **Command + Shift + G** > füge **~/Library/Application Support/RealtimeBoard**ein und lösche alle App-Dateien.

Bei Verwendung von MDM für Mac

Wenn die App nicht geladen wird und in einer Schleife steckt, vergewissere dich, dass deine Einstellungen es zulassen, dass unser Auto-Updater ausgeführt wird. `https://github.com/Squirrel/Squirrel.Mac` muss folgende Rechte haben:

- Lesen, Schreiben und Ausführen für das Verzeichnis `Application`,
- Lesen und Schreiben für `~/Application Support/Caches/` für die Arbeit mit dem Verzeichnis `com.electron.realtimeboard.ShipIt`. Zudem funktioniert es auch mit dem Verzeichnis `private/var/folders`.

Wenn während des Update-Prozesses etwas schiefgeht, erstellt Squirrel `ShipIt_stderr.log` in `~/Application Support/Caches/com.electron.realtimeboard.ShipIt`. Dort findest du weitere Informationen zum Problem.
Bitte beachte, dass Skype und Slack einen ähnlichen Update-Prozess verwenden. Wenn du also bereits MDM dafür konfiguriert hast, kannst du die gleichen Einstellungen für die Miro Desktop-App anwenden.

## Häufige Fragen

1. *Wo kann ich die Desktop-App herunterladen?*
   - Lade sie von [unserer Website](https://miro.com/apps/) herunter.
2. *Wie kann ich das Pop-up zum Öffnen der Desktop-App entfernen, wenn ich Miro in einem Browser starte?*
   - Versuche es mit den Schritten aus [diesem Artikel](../../using-miro/troubleshooting-technical-questions/technical-guidelines/04-how-to-disable-miro-desktop-app-pop-up-in-your-browser.md).
3. *Gibt es eine Desktop-App für Linux?*
   - Nein, im Moment haben wir keine Version dafür.
4. *Wie kann ich in der Desktop-App den Link eines geöffneten Boards kopieren?*
   - Du kannst das **Freigabe**-Menü des Boards öffnen und den Board-Link von dort kopieren. Oder du klickst auf **Datei** in der rechten oberen Ecke > **Board-Link kopieren**. Du kannst auch die Tastenkombination **Strg + Umschalt + L** *(für Windows) /* **Cmd + Umschalt + L** *(für Mac)* verwenden.
5. *Wenn ich in meiner Windows Desktop-App auf **Alt** drücke, erscheint das Menü nicht. Wie kann ich es aufrufen?*
   – Bitte beachte, dass das Menü in der App aus dem Microsoft Store nicht unterstützt wird. Du kannst die App-Daten über die Windows-Einstellungen zurücksetzen (**System > Apps & Features > Miro suchen > Erweiterte Optionen > Zurücksetzen**) oder die [Originalversion der App installieren](https://miro.com/apps/).
6. *Werden meine Boards gelöscht, wenn ich die Desktop-App entferne?*
   - Nein, deine Inhalte sind mit deinem Miro-Profil verknüpft. Du kannst auch über einen Browser, die [Tablet-App](11-tablet-app.md) oder die [mobile App](08-mobile-app.md) darauf zugreifen.
