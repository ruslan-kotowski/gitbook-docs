---
title: "Probleme mit mobilen und Tablet-Ger\xE4ten beheben"
article_id: 360021113559
translation_id: 360021113559
locale: de
sidebar_position: 16
created_at: '2021-04-16T08:25:42Z'
updated_at: '2025-11-25T16:04:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Wenn du Probleme mit Miro auf deinem Handy oder Tablet hast, versuche zuallererst, *die App neu zu installieren und dein Gerät neu zu laden*.  Wenn das nicht hilft, suche unten nach möglichen Ursachen.

| **Probleme auf dem Handy** | | |
| --- | --- | --- |
| **Vorgang** | **Mögliche Ursache** | **Lösung** |
| Die mobile App auf iOS stürzt ab oder funktioniert nicht richtig. | Die iOS-Version ist zu alt. | Bitte aktualisiere deine iOS-Version oder verwende ein anderes Gerät. Unsere mobile App für iOS wird ab Version 12 unterstützt. |
| Ich kann mich erfolgreich bei der Desktop-App anmelden, aber auf dem Handy bleibe ich beim Miro-Logo stecken. | Authentifizierungsdaten sind beschädigt (schlechter Cache) | Gehe zu **App-Einstellungen > Speicher > Speicher löschen** oder installiere die Miro-App neu auf deinem Gerät. |
| Ich erhalte den Fehler „Something went wrong“ (Etwas ist schiefgelaufen) bei der Authentifizierung über SSO in der mobilen App. | 1. 1. Die Netzwerkverbindung ist gesichert und irgendetwas blockiert die Anfragen  2. 2. Chrome wird der Liste der WIAsupportedUserAgents von ADFS hinzugefügt und leitet Nutzer falsch weiter./span>  3. 3. Es ist möglich, dass dieses spezifische Gerät nicht auf die SSO-Umgebung des Unternehmens zugreifen kann | 1. 1. Versuche die Autorisierung der Verbindung über ein anderes Netzwerk  2. 2. Wende dich an deinen Systemadmin und bitte darum, dass Chrome aus der Liste entfernt wird.  3. Erkundige dich bei deiner IT-Abteilung, ob es Einschränkungen bezüglich bestimmter Geräte gibt, die SSO verwenden dürfen. |
| Ich kann die aus den Boards importierten Dateien nicht im mobilen Dateisystem finden. | Wenn du eine Datei aus dem Board auf das Handy herunterlädst, wird sie für dich einige Zeit lang ausgeblendet. | Bitte warte, bis die Datei im Ordner der heruntergeladenen Dateien erscheint. |
| Wenn ich mich bei Miro einlogge, sehe ich die Nachricht „Keine Konten verfügbar“ und kann nicht auf mein Profil zugreifen. | Du wurdest aus allen Teams entfernt oder hast diese [verlassen](../../managing-your-profile/06-how-to-leave-a-team.md). | Bitte logge dich auf deinem Handy oder Tablet bei Miro ein und erstelle ein neues Team oder bitte eine andere Person, dich zu einem Miro-Team einzuladen. |
| Ich kann Miro-Boards im Browser auf dem Handy nicht bearbeiten. | Das ist derzeit eine bekannte Einschränkung. | Bitte wechsle zur [mobilen App](../../../getting-started/apps-for-devices/08-mobile-app.md), dem Tablet oder Desktop. |
| Ich kann das Board nicht über die mobile App exportieren. | Das ist derzeit eine bekannte Einschränkung. | Bitte wechsle auf ein anderes Gerät.  Weitere Informationen über den Miro-Export erfährst du auf [dieser Seite](../../import-and-export/export/03-how-to-export-your-board.md). |

| **Probleme auf dem Tablet** | | |
| --- | --- | --- |
| **Vorgang** | **Mögliche Ursache** | **Lösung** |
| Wenn ich Miro auf dem iPad verwende, verschwindet die Symbolleiste und das Programm verhält sich seltsam. | Unsere App verwendet zum Rendern visueller Elemente WebView. Eine der Regeln für die Arbeitsspeicherverwaltung ist, dass der Renderingvorgang nicht mehr als 25 % des RAM-Speichers des Geräts beanspruchen darf. Danach funktioniert die App nur noch eingeschränkt und lädt nicht mehr richtig, ohne eine Fehlermeldung anzuzeigen oder abzustürzen. | - Schließe alle unnötigen Hintergrundanwendungen, bevor du Miro verwendest. - Arbeite auf *kleineren*Boards. - Versuche sonst, auf einem *anderen Gerät* (Desktop) mit besserem Arbeitsspeicher zu arbeiten. |
| Ich kann mich erfolgreich bei der Desktop-App anmelden, aber auf dem Tablet bleibe ich beim Miro-Logo stecken. | Die Authentifizierungsdaten sind beschädigt | Gehe zu **App-Einstellungen > Speicher > Speicher löschen** oder installiere die Miro-App erneut auf deinem Gerät. |
| Fehlermeldung „Leider ist das Kopieren so vieler Objekte auf einmal nicht möglich“ beim Einfügen von Objekten auf dem iPad. | Du hast die Menge an Daten überschritten, die in einem Puffer auf dem iPad gespeichert werden können. | Bitte kopiere weniger Widgets auf einmal. |
| Ich kann [auf mein Board hochgeladene Google-Dokumente](../../../integrations-apps/google/05-google-drive.md) nicht auf dem Tablet bearbeiten. | Das ist derzeit eine bekannte Einschränkung. | Als Problemumgehung kannst du das Dokument über die Google-Doc-App öffnen, wenn du auf das Symbol **Quelle** klickst. |
| Ich verwende Apple Pencil auf dem iPad.  Wenn ich doppeltippe, um zwischen Stift und Radiergummi zu wechseln, passiert nichts. | Der Wechsel zwischen Stift und Radiergummi durch Doppeltippen ist eine native Funktion, die von der zweiten Generation von Apple Pencils unterstützt wird, und ist keine spezifisch von Miro entwickelte Funktion.  Dies wird nur in der Tablet-App unterstützt. | Bitte stelle sicher, dass dein Apple Pencil die Funktion unterstützt, und wechsle zur [Tablet-App](../../../getting-started/apps-for-devices/11-tablet-app.md). |
| Auf dem iPad funktionieren die folgenden beiden Dinge nicht:   - Zoomen bei Betätigung über das Mausrad - Board-Navigation durch Wischen mit zwei Fingern auf dem Trackpad | Das ist eine bekannte Einschränkung in Zusammenhang mit den OS-Beschränkungen des iPads. | Leider gibt es dafür noch keine Lösung. |
