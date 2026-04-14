---
title: So deaktivierst du das Pop-up zur Miro Desktop-App in deinem Browser
article_id: 360019244239
translation_id: 360019244239
locale: de
sidebar_position: 5
created_at: '2021-01-29T12:48:31Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Wenn die [Miro Desktop-App](../../../getting-started/apps-for-devices/05-desktop-app.md) auf deinem Gerät installiert ist und du ein Miro-Board in einem Browser öffnest, wird dir eventuell ein Pop-up angezeigt, das dir vorschlägt, das Board in der App zu öffnen.

browser_pop-up.jpg
Das Browser-Pop-up, das dich zur Miro Desktop-App führt

Wenn du das Pop-up deaktivieren möchtest, gehe wie folgt vor:

- Für Mac-Nutzer
- Für Windows-Nutzer
- Safari-Browser

### Für Mac-Nutzer

**Schritt 1:** Lösche (deinstalliere) die Desktop-App von deinem Computer.

**Schritt 2:** Nimm die Einstellung "URL immer in der Miro App öffnen" in deinem Browser zurück. So funktioniert es in Chrome und Firefox:

*Für Chrome:*

1. Schließe alle Chrome- und Miro-Fenster, bevor du fortfährst (nutze **C****md + Q**, um den Browser zu verlassen).
2. Öffne den Finder auf deinem Mac > drücke **Command + Umschalt + G** > gib den folgenden Pfad in das Suchfeld ein: **~/Library/Application Support/Google/Chrome**. Öffne deinen Chrome-Profilordner und anschließend die Einstellungen.

   Eventuell gibt es mehrere Ordner mit der Datei. Probiere die folgenden Vorschläge aus:

   - Öffne den **Standard**ordner und suche nach **Preferences**, wenn du nur ein Profil in Google Chrome hast
   - Öffne den Ordner **Profile X** und suche nach **Preferences**, wenn du mehrere Google Chrome-Profile hast. **X** ist eine Zahl aus der Profilliste.
   - Öffne jeden der Ordner (Default, Guest Profile, Profile X), sofern sie vorhanden sind, und suche nach **Preferences****.**
3. Öffne **Einstellungen** in einem Texteditor.
4. Suche nach **`https://miro.com":\{"miroapp":true\}`** .
5. Entferne **`https://miro.com":\{"miroapp":true\}`** .
6. Speichere die Änderungen.
7. Starte den Chrome-Browser neu.

Falls du mehrere Google-Profile verwendest, musst du Einstellungen in allen Katalogen bearbeiten. Öffne in Schritt 2 **~/Library/Application Support/Google/Chrome** und ändere **Preferences** in den Ordnern **Profile 1, Profile 2** usw.

*Für Firefox:*

1. Öffne die Browsereinstellungen.
2. Scrolle im Abschnitt **Allgemein** hinunter zu **Anwendungen.**
3. Suche nach **miroapp** und ändere **Miro verwenden** (Standard) zu **Immer fragen**, indem du die Option im Dropdown-Menü auswählst.

### Für Windows-Nutzer

**Schritt 1:** Lösche (deinstalliere) die Desktop-App von deinem Computer.

**Schritt 2: Verwende das über [diesen Link](https://desktop.miro.com/platforms/Miro_DeleteAppSchema.reg) verfügbare Skript, um den Wert aus der Windows-Registrierung zu löschen*. Sobald das erledigt ist, sollte die Benachrichtigung nicht mehr in deinem Browser angezeigt werden. Falls das Pop-up immer noch angezeigt wird, befolge Schritt 3.***

**Schritt 3:** Nimm die Einstellung "URL immer in der Miro App öffnen" in deinem Browser zurück. So funktioniert es in Chrome und Firefox:

*Für Chrome:*

1. Schließe alle Chrome- und Miro-Fenster, bevor du startest.
2. *N*avigiere zu **PC** > **Users > \{current_user\} > AppData > Local > Google > Chrome > UserData > Default > Preferences.**
3. Öffne **Einstellungen** in einem Texteditor.
4. Suche nach **`https://miro.com":\{"miroapp":true\}`** .
5. Entferne **`https://miro.com":\{"miroapp":true\}`** .
6. Speichere die Änderungen.
7. Starte den Chrome-Browser neu.

Falls du mehrere Google-Profile verwendest, musst du Einstellungen in allen Katalogen bearbeiten. Navigiere hierzu zu **PC** > **Users > \{current_user\} > AppData > Local > Google > Chrome > UserData** und ändere **Preferences** in den Ordnern **Profile 1, Profile 2** usw.

*Für Firefox:*

1. Öffne die Browsereinstellungen.
2. Scrolle im Abschnitt **Allgemein** hinunter zu **Anwendungen.**
3. Suche nach **miroapp** und ändere **Miro verwenden** (Standard) zu **Immer fragen**, indem du die Option im Dropdown-Menü auswählst.

### Safari-Browser

Falls du das Pop-up in Safari deaktivieren möchtest, lösche die Miro Desktop-App von deinem Gerät.
