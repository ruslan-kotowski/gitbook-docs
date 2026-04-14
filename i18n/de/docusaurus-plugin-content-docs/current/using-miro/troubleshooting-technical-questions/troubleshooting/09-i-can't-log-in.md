---
title: Ich kann mich nicht einloggen
article_id: 360020993079
translation_id: 360020993079
locale: de
sidebar_position: 9
created_at: '2021-04-09T06:31:47Z'
updated_at: '2025-11-25T16:04:24Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Befolge diesen Leitfaden, wenn du Probleme beim Einloggen in dein Miro-Profil hast.

## Probleme mit der E-Mail-Adresse und/oder dem Passwort

Meine E-Mail-Adresse/Passwort funktioniert nicht

Es gibt zwei Lösungsmöglichkeiten dafür:

1. Vergewissere dich, dass die E-Mail-Adresse/das Passwort, die/das du zum Einloggen verwendest, keine Tippfehler enthält.
2. Falls die Anmeldedaten richtig sind, kannst du [dein Passwort zurücksetzen](../../managing-your-profile/05-how-to-change-your-password.md).
3. Wenn deine E-Mail-Adresse oder dein Passwort eines der Symbole **& " < >** enthält, [wende dich bitte an das Support-Team.](https://help.miro.com/hc/requests/new?)

:::warning
Beachte, dass dein **Profil** gesperrt wird, wenn du versuchst, deine E-Mail-Adresse und dein Passwort mehr als zehn Mal einzugeben. Möglicherweise musst du zuerst [das Profil entsperren](../../tools/troubleshooting/14-profile-lockout.md) und dann dein Passwort zurücksetzen.
:::

Ich kann mein Passwort nicht zurücksetzen

Solltest du keine E-Mail zum Zurücksetzen deines Passworts erhalten, kann das drei Gründe haben:

1. **Die E-Mail-Adresse ist falsch**
Vergewissere dich, dass in der von dir angegebenen E-Mail-Adresse keine Tippfehler vorhanden sind. Wenn du einen Tippfehler findest, versuche es erneut.

2. **Die E-Mail-Adresse ist noch nicht bei Miro registriert**
In diesem Fall wird der Link zum Zurücksetzen des Passworts nicht an deine E-Mail-Adresse gesendet. Registriere ein neues Profil auf der [Registrierungsseite](https://miro.com/signup/). Wenn deine E-Mail-Adresse registriert ist, siehst du die entsprechende Nachricht:
![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)

3. **Es gibt Probleme bei der E-Mail-Zustellung**

- Öffne deine Ordner **Spam, Werbeaktionen, Junk, Social** und **Updates** und überprüfe, ob die E-Mail mit der Anfrage zum Zurücksetzen dort zu finden ist.
- Möglicherweise verhindert auch eine Firewall, dass die E-Mail dein Postfach erreicht.

  Bitte deinen *System-Admin*, unsere Domains und Subdomains zuzulassen: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) und [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/) und füge das IPS unseres E-Mail-Versandsystems zu deiner Zulassungsliste hinzu.

  Hier ist die Liste der dedizierten IPs: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. [Hier ist ein Artikel](../../tools/troubleshooting/02-allowlist-miro-mailers.md) mit weiteren Informationen zu den Mailern, die auf deiner Zulassungsliste stehen sollten.

Ich habe mein Passwort zurückgesetzt, kann mich aber immer noch nicht einloggen

Falls du immer noch nicht auf dein Profil zugreifen kannst:

1. Stelle sicher, dass du das neue Passwort eingibst.
2. Logge dich im privaten (Inkognito)-Modus deines Browsers ein oder benutze einen anderen Browser.

Ich logge mich mit einer E-Mail-Adresse ein, werde jedoch umgeleitet und bin dann mit einer anderen E-Mail-Adresse eingeloggt

Dieses Problem kann auftreten, wenn du zum Einloggen eine alternative Authentifizierungsmethode verwendest (Google, Slack, Office 365, Apple ID, Facebook).

![new-sing-in-Thir-party.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
*Alternative Anmeldeoptionen auf der Anmeldeseite*

Möglicherweise hast du versehentlich deine Google/Office 365/etc.-E-Mail-Adresse mit deinem Miro-Profil verknüpft, das unter einer anderen E-Mail-Adresse registriert ist. Falls dies der Fall ist, versuche Folgendes:

1. Entferne die falsche E-Mail-Zuordnung, indem du zu deinen **Profileinstellungen** > **Integrationen** gehst und neben Google/Office 365/etc. auf **Abmelden** klickst.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Die Verknüpfung mit dem Google-Login entfernen*
2. Logge dich aus und logge dich erneut mit deiner E-Mail-Adresse ein.

:::note
Stelle eine Verknüpfung mit der E-Mail-Adresse von Google/Office 365/Slack her, die mit der E-Mail-Adresse deines Miro-Profils übereinstimmt, um das Problem zu vermeiden.
:::

## SSO-Anmeldung funktioniert nicht

Hier findest du den Artikel: [Mögliche Probleme bei der SSO-Anmeldung](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Endloses Laden beim Einloggen

Wir empfehlen Nutzern, die nach der Eingabe ihrer Miro-Anmeldedaten Probleme in Bezug auf endloses Laden haben, Folgendes:

1. Melde dich in einem **anderen Browser** an.
2. Melde dich im **privaten Modus (inkognito) deines Browsers an.** Falls das Problem im Inkognito-Modus/einem anderen Browser nicht auftritt, lösche deinen Browser-Cache.

   Chrome-Cache löschen

   1. Gehe auf `https://miro.com/` und öffne die **Entwicklertools**von Chrome (**Befehlstaste + Option + J** *auf dem Mac*, **Strg + Umschalttaste + J***auf Windows*).
   2. Gehe zum Tab **App > Speicher**. Dort siehst du die blaue Schaltfläche **Website-Daten löschen.**​  Klicke auf die Schaltfläche und dies sollte alle in deinem Chrome-Browser gespeicherten Daten aus Miro entfernen. Jetzt kannst du eine neue Arbeitssitzung starten.
   ![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
   *Die Option zum Löschen von Website-Daten in Chrome*
3. Wenn du ein **VPN** verwendest, kannst du es aus/einschalten.
4. Erkundige dich bei deiner IT-Abteilung, ob dein Unternehmen Firewalls oder einen Proxy verwendet, die Miro möglicherweise blockieren. Befolge [diese Richtlinien](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md), um **Miro auf die Zulassungsliste** zu setzen oder eine Umgehung zu ermöglichen.
5. Überprüfe deine Internetverbindung. Wenn deine Netzwerkbandbreite das Minimum von 8 Mbit/s nicht erreicht, **wechsle zu einem anderen, vorzugsweise** **schnellerem Netzwerk**.
6. Versuche, eine Verbindung mit einem **mobilen Hotspot** herzustellen, falls verfügbar. Verbinde dich dann erneut mit deinem ursprünglichen Netzwerk.
7. Wenn das nicht hilft, [sende eine Anfrage](https://miro.com/contact/recover/) und [schicke die Protokolle deiner Browser-Konsole an den Support](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).

## Probleme beim Einloggen mit der Miro-Desktop-App

1. Falls du über die Desktop-App nicht auf Miro zugreifen kannst, logge dich über deinen Browser ein. Wenn du dich immer noch nicht anmelden kannst, befolge die oben genannten Schritte. Falls du über den Browser auf Miro zugreifen kannst, führe die nachfolgenden Schritte aus.
2. Setze die App-Daten zurück.

App-Daten auf Windows zurücksetzen

Drücke **Alt > Hilfe** und wähle die Option zum Zurücksetzen der App-Daten, wie im Screenshot unten gezeigt:

​​![reset_app_data_on_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
*Die App-Daten in der Desktop-App für Windows zurücksetzen*

Wenn du das Menü nicht finden kannst, verwendest du wahrscheinlich die App, die du aus dem MS Store heruntergeladen hast. Um in diesem Fall die App-Daten zurückzusetzen, öffne die **Windows-Einstellungen** > **Apps** > **Apps und Features** > suche in der Liste nach **Miro** > **Erweiterte Optionen > Zurücksetzen.**

Falls dies nicht unmittelbar weiterhilft, lösche alle App-Dateien aus **C:\Benutzer\Benutzername\AppData\Roaming\RealtimeBoard** und **C:\Benutzername\AppData\Local\RealtimeBoard**

> **✏️** Wenn der **Appdata** Ordner nicht sichtbar ist, kannst du dir [hier](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) ansehen, wie du ihn anzeigen kannst.

App-Daten auf einem Mac zurücksetzen

Klicke im oberen Menü auf Miro und wähle **App-Daten zurücksetzen**, wie im Screenshot unten gezeigt:

![reset_app_data_on_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
*Die App-Daten auf dem Mac zurücksetzen*

Versuche danach, dich erneut in der App einzuloggen und prüfe, ob das Problem behoben ist.

Sollte das Zurücksetzen nicht unmittelbar weiterhelfen, öffne ein Finder-Fenster > drücke **Command + Shift + G**> füge **~/Library/Application Support/RealtimeBoard** ein und lösche alle App-Dateien.

3. Wenn das Problem weiterhin besteht, stelle sicher, dass du die neueste Version der App verwendest, die du [von unserer Website heruntergeladen hast.](https://miro.com/apps/)

## Über Google/Office 365/Slack/etc. anmelden

Ich kann mich nicht über Google/Office/Slack/etc. einloggen.

1. Logge dich mit deinen üblichen Anmeldeinformationen (E-Mail-Adresse und Passwort) bei Miro ein. Falls du dich nicht mehr an das Passwort erinnerst oder es nicht mehr parat hast, [setze es zurück](../../managing-your-profile/05-how-to-change-your-password.md).
2. Gehe zu **Profileinstellungen** > **Integrationen**, klicke neben Google/Office 365/etc. auf **Abmelden** und konfiguriere die Verknüpfung neu.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Die Verknüpfung mit dem Google-Login entfernen*

Ich kann mich in der Desktop-App nicht über Google/Office/Slack etc einloggen

Schau dir diese Schritte zur Fehlerbehebung an.

Bisher habe ich mich bei Miro über Google/Office 365 etc. eingeloggt, aber mein E-Mail-Anbieter hat sich geändert. Wie kann ich mich jetzt einloggen?

Melde dich mit den neuen Anmeldedaten deines Anbieters (E-Mail-Adresse und Passwort) bei Miro an. Falls du dich nicht mehr an das Passwort erinnerst oder es nicht parat hast, [setze es zurück](../../managing-your-profile/05-how-to-change-your-password.md).

## Probleme beim Einloggen auf Tablet/Mobiltelefon

1. Überprüfe, ob du dich in der Browserversion anmelden kannst. Wenn nicht, empfehlen wir dieseSchritte zur Fehlerbehebung.
2. Falls das Einloggen im Browser funktioniert, kann es sein, dass die Authentifizierungsdaten deines Geräts beschädigt sind. Gehe zu **App-Einstellungen > Speicher > Speicher löschen** oder installiere die Miro-App auf deinem Gerät neu.

## Tipps zur Fehlerbehebung

Falls du bisher noch keine Lösung finden konntest, logge dich bitte mit **einem anderen Browser** oder **im Inkognito-Modus** bei Miro ein. Falls im Inkognito-Modus deines Browsers alles funktioniert, lösche den Cache und die Cookies deines Browsers und logge dich im Standardmodus bei Miro ein.

Chrome-Cache löschen

1. Gehe auf `https://miro.com/` und öffne die **Entwicklertools**von Chrome (**Befehlstaste + Option + J** *auf dem Mac*, **Strg + Umschalttaste + J***auf Windows*).
2. Gehe zum Tab **App > Speicher**. Dort siehst du die blaue Schaltfläche **Website-Daten löschen.**​  Klicke auf die Schaltfläche und dies sollte alle in deinem Chrome-Browser gespeicherten Daten aus Miro entfernen. Jetzt kannst du eine neue Arbeitssitzung starten.

![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
*Die Option zum Löschen von Website-Daten in Chrome*

Wenn das nicht hilft, [wende dich an den Miro-Support](https://miro.com/contact/recover/). Bitte beschreibe das Problem ausführlich.

:::note
Wenn du Probleme mit der Registrierung bei Miro hast, schaue unter[Probleme mit dem Bestätigungscode](../../tools/troubleshooting/12-issues-with-confirmation-code-or-password-reset-emails.md) nach.
:::
