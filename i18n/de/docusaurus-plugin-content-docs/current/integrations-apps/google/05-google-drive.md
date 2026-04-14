---
title: Google Drive
article_id: 360017731253
translation_id: 360017731253
locale: de
sidebar_position: 6
created_at: '2019-02-11T10:14:01Z'
updated_at: '2025-01-13T14:51:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-drive-onedrive
---

Mit **Google Drive** kannst du Dateien sicher online abspeichern, von überall auf sie zugreifen und mit anderen zusammenarbeiten. Mit der Integration für Google Drive erleichtern wir es dir, dich auf deine Aufgaben zu konzentrieren und deine Dokumente direkt auf dem Board zu verfolgen.

![Google_Drive_on_the_Upload_menu.jpg](../../../../../../docs/integrations-apps/google/images/21016121222546_Google%20Drive%20on%20the%20Upload%20menu.jpg)

> **Einrichtung durch:** Jeden Nutzer für sich (Admins können die Installation der App durch Nicht-Admins einschränken)
> **Verfügbar mit:** Browser-Version, [Desktop-App](../../getting-started/apps-for-devices/05-desktop-app.md) (volle Funktionalität und Bearbeiten von Dateien); [Tablet-App](../../getting-started/apps-for-devices/11-tablet-app.md), [mobile App](../../getting-started/apps-for-devices/08-mobile-app.md) (eingeschränkte Funktionalität, Bearbeiten wird nicht unterstützt)

### Google Drive aktivieren

Um mit dem Hinzufügen von Dateien aus Google Drive zu beginnen, musst du das Plug-in installieren und dein Google Drive mit Miro verbinden.

Installation der App über den [Miro Marketplace](https://miro.com/marketplace/google-drive/?backUrl=%2Fmarketplace%2F). Nachdem du auf **Get app** geklickt hast, wird dir vorgeschlagen, ein Team auszuwählen, für das du das Plugin installieren möchtest.![install_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016134562450_install%20Google%20Drive.jpg)*Auswahl eines Teams bei der Installation des Google Drive-Plugins*

Ebenso kannst du das Plug-in von einem Board aus installieren. Wähle in der Erstellungsleiste **Tools, Medien und Integrationen****(+**). Ein Bereich öffnet sich. Suche auf dem Tab **Tools** nach Google Drive. Wähle " **Hochladen"** und dann " **Google Drive"**.

![Google_Drive_on_the_toolbar.jpg](../../../../../../docs/integrations-apps/google/images/21016121227026_Google%20Drive%20on%20the%20toolbar.jpg)

Verbinde daraufhin Google Drive mit Miro. Es gibt dafür zwei einfache Wege.

1.  In den Einstellungen deines Profils. Wähle in der Board-Leiste das Dreistrich-Symbol aus. Die Seitenleiste öffnet sich. Wähle deinen Avatar aus und wähle dann **Einstellungen**. Deine Profileinstellungen werden in einem neuen Fenster geöffnet. Wähle den Tab **Integrationen** . Für **Google Drive** wählst du **Verbinden**.

![connect_Google_Drive.jpg](../../../../../../docs/integrations-apps/google/images/21016121228306_connect%20Google%20Drive.jpg)*Google Drive auf der Integrationsseite*

2. Verbinde dein Miro-Profil vom Board aus mit Google Drive, indem du im **Upload-Menü** in der Symbolleiste auf **Google Drive** klickst:

![Google_Drive_on_the_Upload_menu.jpg](../../../../../../docs/integrations-apps/google/images/21016121222546_Google%20Drive%20on%20the%20Upload%20menu.jpg)*Das Google Drive-Symbol in der Symbolleiste*

Bestätige die Autorisierung für das erforderliche Google-Konto und klicke auf **Erlauben**, damit die App auf deine Dateien zugreifen kann:

![permissions.jpg](../../../../../../docs/integrations-apps/google/images/21016121229586_permissions.jpg)
*Google Drive-Berechtigungen*

Bitte beachte, dass dies die Standardberechtigungen für Google Drive sind.

- **Sieh dir alle deine Google Drive-Dateien an und lade sie herunter** – für einen Google Drive-Datei-Picker auf einem Board. Er ermöglicht den Import von Dokumenten aus Google Drive nach Miro

- **Du kannst nur jene Google Drive-Dateien anzeigen, bearbeiten, erstellen und löschen, die du im Zusammenhang mit dieser App verwendest**, um ein Miro-Board in Google Drive speichern zu können.

Die Google Drive-App verwaltet nur die Dateien, die wir auf Drive erstellen (Links zu Boards, etc.).  Miro hat keine Möglichkeit, Inhalte auf deinem Google Drive zu verwalten. Zur Implementierung der Integration verwenden wir **Google Drive API v3**. In dieser API werden die Bereiche so gruppiert, dass Schreibzugriffsberechtigungen nicht getrennt von den vollen Festplattenzugriffsberechtigungen angefordert werden können. Wenn du einen Blick darauf werfen möchtest, sieh dir die Berechtigungen in Googles Artikel [Scopes for Google APIs](https://developers.google.com/identity/protocols/googlescopes) an.

Falls du das mit Miro verbundene Google-Konto ändern musst, gehe zu **Profileinstellungen** > **Integrationen**, klicke neben **Google Drive** **auf Abmelden** und verbinde dich mit einem anderen Konto.

![Google_Drive_log_out_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*Google Drive-Verbindung in den Profileinstellungen*

### Hinzufügen von Dateien aus Google Drive und freigegebenen Laufwerken

> **Verfügbar mit:** Browser-Version, [Desktop-App](../../getting-started/apps-for-devices/05-desktop-app.md), [Tablet-App](../../getting-started/apps-for-devices/11-tablet-app.md), [mobiler App](../../getting-started/apps-for-devices/08-mobile-app.md) (begrenzte Funktionalität)

:::warning
Jeder, der Zugriff auf ein Miro-Board hat , kann die darin importierten Dokumente extrahieren, auch wenn der Zugriff auf sie auf der Google-Seite eingeschränkt sind. Um deine Dateien zu schützen, ist es wichtig, das Board nicht für Personen freizugeben, die keinen Zugriff auf die Dokumente haben sollten.
:::

So fügst du eine Datei aus Google Drive hinzu:

1. Füge die URL des Dokuments direkt auf das Board ein (beachte, dass beim Einfügen einer URL in eine [Form](../../using-miro/essential-tools/11-shapes.md) oder eine [Notiz](../../using-miro/essential-tools/14-sticky-notes.md) das Dokument nicht im Board eingebettet wird, sondern der Link als einfacher Text hinzugefügt wird). Wenn du einen Link zu einem bestimmten Tabellenblatt aus Google Tabellen kopierst und in das Miro-Board einfügst, wird die eingefügte Tabelle trotzdem auf der ersten Seite in Miro gestartet.

   oder:
2. Klicke auf die Schaltfläche **Hochladen** in der Symbolleiste (siehe Screenshot oben) und wähle **Google Drive**. Du siehst dann das Auswahlmenü. Wähle alle Dokumente aus, die du hinzufügen möchtest, und klicke auf **Auswählen**. Du kannst auch die Suchleiste verwenden, um Dokumente in deinem Google Drive zu finden.

:::tip
Um in der [mobilen App](../../getting-started/apps-for-devices/08-mobile-app.md) ein Google Drive-Dokument auf ein Board hochzuladen, füge die URL des Dokuments über das Upload-Menü ein.
:::

![select_a_file_in_Google_Drive.gif](../../../../../../docs/integrations-apps/google/images/21016121231122_select%20a%20file%20in%20Google%20Drive.gif)*Auswählen eines Dokuments in Google Drive*

Dokumente hinzufügen von **gemeinsam genutzten Drives** – wechsle zum entsprechenden Tab und wähle Dateien.

![team_drive.jpg](../../../../../../docs/integrations-apps/google/images/21016134572434_team%20drive.jpg)*Team Drive in der Google Drive-Auswahl*

### Bearbeiten von Google-Dokumenten

> **Verfügbar mit:** Browser-Version, [Desktop-App](../../getting-started/apps-for-devices/05-desktop-app.md)

Du kannst Google Documents, Spreadsheets und Slides direkt auf dem Board einbetten, sie verschieben und in der Größe verändern und auch durch die Seiten der Dokumente blättern.

Wenn du auf das Dokument klickst, erscheint ein Kontextmenü mit den Optionen Seiten wechseln, eine Seite **anheften**, **Seiten extrahieren**, Inhalt bearbeiten, **neu laden**, **aktualisieren** oder zur **Quelle** gehen.

Um die Bearbeitung des Dokuments zu starten, klicke auf das Stiftsymbol im Kontextmenü oder doppelklicke auf das Dokument. Das Dokument wird in einem Pop-up geöffnet und du kannst es wie in deinem Google Drive bearbeiten. Klicke auf **Schließen** oder den grauen Bereich, um die Bearbeitung zu beenden. Alle Änderungen werden automatisch gespeichert und sind auf dem Board und in den Google-Dokumenten sichtbar.

![google_drive_edit_docs.gif](../../../../../../docs/integrations-apps/google/images/21016121248274_google_drive_edit_docs.gif)*Bearbeitung eines eingebetteten Google-Dokuments*

Wenn du möchtest, kannst du auch auf **Quelle** klicken und das Dokument wird im nächsten Tab zur Bearbeitung geöffnet.

Wenn du Änderungen direkt in deinem Google Drive vorgenommen hast (vor allem, wenn du offline arbeitest), aktualisiere die Einbettung auf dem Board über die Schaltfläche **Aktualisieren** im Kontextmenü. Eingebettete Google Drive-Dateien werden auf Miro-Boards nicht automatisch aktualisiert (es sei denn, die Datei wird von Miro aus bearbeitet).

![update_button.jpg](../../../../../../docs/integrations-apps/google/images/21016121232274_update%20button.jpg)*Schaltfläche zum Aktualisieren*

### Verwalten von Zugriffsrechten

Bitte beachte, dass die Zugriffsrechte in Google Drive und in Miro *separat* festgelegt werden. Wenn du jemanden ein Google-Dokument im Board bearbeiten lassen willst, musst du das Dokument in Google Drive mit *Bearbeitungsrechten* freigeben und die Person [mit *Bearbeitungsrechten* zum Board einladen](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

Wenn du jemandem erlaubst, das Dokument in Google zu bearbeiten, die Person aber nur mit [Ansichts- oder Kommentarrechten](../../using-miro/sharing-boards/01-board-access-rights.md) zum Board einlädst, kann sie den Bearbeitungsmodus des Dokuments nicht aktivieren. Umgekehrt gilt: Wenn du eine Person mit Bearbeitungszugriff zum Board einlädst, aber das Dokument nicht für sie in Google Drive freigibst, kann sie es nicht bearbeiten.

Bitte vergewissere dich, dass du und deine Teammitglieder über die Zugriffsebene verfügen, die für eine erfolgreiche Zusammenarbeit erforderlich ist.

### Speichern deines Boards in Google Drive

> **Einrichtung durch:** Board-Eigentümer

Wähle in der Board-Leiste die vertikalen drei Punkte aus. Das **Hauptmenü** wird geöffnet. Wähle **Board** > **Exportieren** > **In Google Drive speichern**.

In Google Drive kannst du jetzt auf das gespeicherte Board klicken und es wird in einem eigenen Tab im Browser geöffnet. Wenn du das Board aus Google Drive löschst, ist es trotzdem noch in Miro verfügbar. Wenn du das Board jedoch in Miro löschst, kannst du nicht mehr über Google Drive darauf zugreifen.

:::warning
Wenn du nicht Board-Eigentümer bist, bekommst du die folgende Fehlermeldung.
:::

![Google_Drive_error.jpg](../../../../../../docs/integrations-apps/google/images/21016121236882_Google%20Drive%20error.jpg)*Fehlermeldumg über unzureichende Speicherrechte*

### Deinstallation des Plugins

Um das Plugin für ein Team zu deinstallieren, suche es im Abschnitt **Apps & Integrationen** in den Teameinstellungen und klicke auf **Für Team deinstallieren**.

![deinstallieren_Google_Drive_app.jpg](../../../../../../docs/integrations-apps/google/images/21016134575122_uninstall%20Google%20Drive%20app.jpg)*Deinstallation von Google Drive für ein Team*

Um Miro von Google Drive zu trennen, öffne die Seite **Integrationen** in deinen Profileinstellungen und klicke auf**Abmelden** neben dem Google Drive-Symbol.

![Google_Drive_log_out_in_settings.jpg](../../../../../../docs/integrations-apps/google/images/21016121230610_Google%20Drive%20log%20out%20in%20settings.jpg)*Trennen von Google Drive von Miro*

### Funktionen, die für eingebettete Google Drive-Dateien nicht verfügbar sind

**Allgemein**

- Google Drive Startseite
- Dateien zwischen Ordnern verschieben
- Freigabe
- Hilfe suchen

**Google Präsentationen**

- Präsentationsmodus

### Mögliche Probleme und wie man sie löst

**Fehler „Hochladen nicht möglich“**

Wenn du die Fehlermeldung **erhältst, hast du anscheinend keine Berechtigung zum Hochladen dieser Datei oder die Datei wurde gelöscht. Bitte überprüfe die Zugriffsrechte und versuche es erneut.** Wenn du versuchst, eine Google Drive-Datei auf ein Miro-Board hochzuladen, bitte deinen Google-Administrator, den Nutzern den Zugriff auf Google Drive mit der Drive SDK API zu erlauben:

1. Melde dich bei der [Google Admin-Konsole](https://admin.google.com/) an.
2. Klicke auf **Home > Apps > Google Workspace**. Stelle sicher, **dass Drive und Docs** **für alle aktiviert sind**.
3. Klicke auf **Laufwerk und Dokumente > Funktionen und Apps**. Vergewissere dich im AbschnittDrive SDK, dass die Option **Nutzern den Zugriff auf Google Drive mit der Drive SDK API erlauben** auf **EIN** steht.

![unable_to_upload.png](../../../../../../docs/integrations-apps/google/images/21016134575634_unable%20to%20upload.png)
*Warnmeldung „Hochladen nicht möglich“*

**Autorisierungsproblem**

Wenn du dein Google Drive nicht mit Miro verbinden kannst, stelle bitte sicher, dass  du Miro Zugriff darauf gibst, **alle deine Google Drive-Dateien  anzusehen und herunterzuladen**und **nur die spezifischen Google Drive-Dateien anzusehen, zu bearbeiten, zu erstellen und zu löschen, die du mit dieser App** **verwendest** , wenn du dein Google Drive verbindest. Gehe dazu zu den [Einstellungen](../../using-miro/managing-your-profile/01-profile-settings.md) deines [Miro Profils](../../using-miro/managing-your-profile/01-profile-settings.md) > **Integrationen**, entferne die Verbindung mit Google Drive und richte sie erneut ein.

![Permissions.png](../../../../../../docs/integrations-apps/google/images/21016121246994_Permissions.png)
*Miro-Zugang zum Google Drive Konto*

### Häufige Fragen

1. *Kann ich eine eingebettete Datei in Google Drive öffnen?*
   - Ja, wähle das Dokument aus und klicke auf die Schaltfläche **Quelle** im Kontextmenü.
2. *Kann ich den Inhalt eines Miro-Boards in eine Google Drive-Datei einfügen?*
   - Du kannst [Board-Inhalte als Text oder Bild kopieren](../../using-miro/working-on-the-board/09-copy-as-text-or-as-an-image.md) und in eine Google Drive-Datei einfügen.
