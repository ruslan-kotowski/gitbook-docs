---
title: "Probleme mit dem Best\xE4tigungscode oder E-Mails, um das Passwort zur\xFC\
  ckzusetzen"
article_id: 360017731373
translation_id: 360017731373
locale: de
sidebar_position: 12
created_at: '2019-02-11T10:14:22Z'
updated_at: '2024-10-25T14:25:54Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Wenn du keinen Bestätigungscode oder keine E-Mail zum Zurücksetzen des Passworts erhalten hast, kann dies mehrere Gründe haben. Du kannst die folgenden Optionen ausprobieren, um zu versuchen, die Situation zu lösen.

## Häufige Gründe, warum Codes oder E-Mails nicht ankommen

Zwei der häufigsten Gründe, warum du keine E-Mails zum Zurücksetzen des Passworts bekommst oder keinen neuen Bestätigungscode anfordern kannst:

1. Dein Unternehmen verwendet eine Firewall, die E-Mails von miro.com-Domains blockiert. Bitte deinen IT-Admin, E-Mails von [miro.com](http://miro.com/) Domains zuzulassen.  Wenn du der Administrator bist, findest du im folgenden Abschnitt Anweisungen zur Allowlist der Miro-Domains.
2. Dein Unternehmen verwendet SSO. Im folgenden Abschnitt findest du Anweisungen dazu, wie du dies beheben kannst.

## So behebst du Probleme mit verloren gegangenen E-Mails/Bestätigungscodes

1. Wenn dein Unternehmen SSO verwendet, musst du dich mit deinen SSO-Anmeldeinformationen anmelden. Wenn du versuchst, dein Passwort mit Miro zurückzusetzen, wirst du einfach zurück zur SSO-Anmeldeseite geleitet. Versuche in diesem Fall, dich mit den SSO-Anmeldedaten für dein Unternehmen einzuloggen. Wenn das nicht funktioniert, fahre mit der unten aufgeführten Fehlerbehebung fort.
2. Eine Firewall kann verhindern, dass die E-Mail dein Postfach erreicht. Bitte deinen Systemadministrator, unsere Domains und Subdomains in die Zulassungsliste aufzunehmen: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com und realtimeboard.com*, *.realtimeboard.com.

   Hier ist die Liste der dedizierten IPs: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. Hier findest du mehr zum Thema [Zulassen von Miro E-Mails.](../../tools/troubleshooting/02-allowlist-miro-mailers.md)
3. Vergewissere dich, dass in der von dir angegebenen E-Mail keine Tippfehler vorhanden sind. Wenn du einen Tippfehler findest, [registriere das Profil erneut](../../../getting-started/start-here/02-how-to-register-with-miro.md)/setze dein Passwort zurück und verwende dafür die richtige E-Mail-Adresse.
4. Überprüfe die **Spam-, Werbe-,** **Junk-, Social-** und **Updates-**Ordner deines E-Mail-Anbieters.
5. Du kannst dich auch registrieren oder dich mit alternativen Optionen registrieren/anmelden: mit Google, Slack, Office 365, Apple oder Facebook.
   > ⚠️ Beachte, dass alternative Anmeldungen **nicht** mit SSO-Anmeldungen des Unternehmens verbunden sind. Wenn du Miro in einer Unternehmensumgebung verwendest, verwende bitte die Anmeldeinformationen, die dein Miro-Admin für dich eingerichtet hat.

   ![](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)altnew-sing-in-Thir-party.png
   Verfügbare Authentifizierungsmethoden

Wenn du dich nicht registrieren oder dich nicht mit anderen Authentifizierungsmethoden einloggen kannst:

- Überprüfe, ob dein Posteingang voll ist und das Speicherlimit deines E-Mail-Kontos erreicht ist. Wenn das Postfach voll ist, musst du möglicherweise einige E-Mails löschen, um neue zu erhalten. Gehe nach dem Löschen der E-Mails zurück zu unserer Registrierungsseite und klicke auf **Code erneut senden.**
- Du solltest die E-Mail umgehend erhalten. Wenn nicht, musst du möglicherweise bis zu 24 Stunden warten.
- Wenn du die SSO-Anmeldeinformationen deines Unternehmens verwendest und dich nicht anmelden kannst, solltest du dir die Informationen über [häufige SSO-Fehler durchlesen und wie du sie beheben kannst](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

### Andere Probleme im Zusammenhang mit der Bestätigung

Mein Code ist ungültig

Wenn der von dir eingegebene Code **ungültig** ist:

1. Schau in deinem Posteingang nach und stelle sicher, dass du den zuletzt erhaltenen Code eingibst. Wenn der Code immer noch ungültig ist, klicke auf **Code erneut senden** und gib den Code aus der neuen E-Mail ein.
2. Alternativ kannst du in der E-Mail mit dem Bestätigungscode auf **Deine E-Mail-Adresse bestätigen** klicken, um die Registrierung abzuschließen. In diesem Fall brauchst du keinen Bestätigungscode.
   confirm email button.png
   *Die Option, deine E-Mail zu bestätigen*

Ich habe die maximale Anzahl der E-Mail-Bestätigungsversuche überschritten

Wenn du deine E-Mail nach 4 Versuchen nicht bestätigen konntest, erhältst du die Nachricht  **Anzahl der E-Mail-Bestätigungsversuche überschritten** auf der Registrierungsseite.

Warte 60 Sekunden und klicke dann auf **Code erneut senden** – dadurch wird ein neuer Code generiert. Gib den Code ein und schließe die Registrierung ab.

Ich habe versehentlich das Tab geschlossen, in der ich den Bestätigungscode einfügen soll

[Melde dich](https://miro.com/login/) mit der E-Mail-Adresse und dem Passwort an, das du bei der Registrierung eingegeben hast, und du wirst zurück zur [Bestätigungsseite](https://miro.com/email-confirm/) geleitet.

:::note
Wenn du deine E-Mail-Adresse nicht bestätigst, erhältst du nach 12 und 24 Stunden Erinnerungen. Wenn deine E-Mail-Adresse nicht innerhalb von 7 Tagen bestätigt wurde, wird dein **Profil gelöscht**. Du kannst dich jedoch mit derselben E-Mail-Adresse mit einem neuen Profil registrieren.
:::

:::note
Bestätigungscodes können nur per E-Mail gesendet werden.
:::

:::note
Wenn du immer noch Probleme hast, [wende dich an den Miro-Support](https://miro.com/contact/recover/).
:::
