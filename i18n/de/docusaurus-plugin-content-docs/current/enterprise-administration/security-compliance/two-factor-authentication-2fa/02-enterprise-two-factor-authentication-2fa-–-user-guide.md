---
title: Enterprise Zwei-Faktor-Authentifizierung (2FA) – Nutzerleitfaden
article_id: 7935469290002
translation_id: 7935469290002
locale: de
sidebar_position: 2
created_at: '2022-10-04T09:00:42Z'
updated_at: '2025-11-06T13:50:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Relevant für: Starter, Business, Education, Enterprise'
---

## Was ist Zwei-Faktor-Authentifizierung (2FA)

Die Zwei-Faktor-Authentifizierung (2FA) bietet mehr Sicherheit für deine Online-Konten. Wenn dein Unternehmens-Admin die Zwei-Faktor-Authentifizierung (2FA) aktiviert, wird jede Anmeldung bei Miro mit deiner E-Mail und deinem Passwort um eine zusätzliche Sicherheitsstufe ergänzt. Dieser zusätzliche Schritt sorgt für einen verbesserten Schutz deines Kontos, da eine Verifizierung über deine regulären Anmeldeinformationen hinaus erforderlich ist.

:::tip
Erfahre, wie du die Zwei-Faktor-Authentifizierung (2FA) für deine Organisation für [Enterprise-Preispläne](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md), und [alle anderen Preispläne](../../../administration/security-compliance/01-two-factor-authentication-2fa.md) aktivierst.
:::

## So richtest du die Zwei-Faktor-Authentifizierung (2FA) ein

**Neue Nutzer:** Bei der ersten [Registrierung](https://miro.com/signup/) mit der E-Mail-Adresse deines Unternehmens wirst du aufgefordert, 2FA zu aktivieren.
**Bestehende Nutzer:** Wenn deine Organisation 2FA verlangt und du kein Single Sign-on (SSO) verwendest, wirst du bei deiner nächsten [Anmeldung](https://miro.com/login/) aufgefordert, 2FA einzurichten.

1. Lade eine Authentifizierungs-App auf dein mobiles Gerät herunter. Authentifizierungs-Apps wie Google Authenticator, Microsoft Authenticator und Authy generieren einen zeitbasierten, einmaligen Code (TOTP) für sichere Anmeldungen bei Miro. Erkundige dich bei deinen Unternehmens- oder IT-Admins nach der passenden App.

2. Klicke auf **Ich habe eine Authentifizierungs-App** im Miro 2FA-Einrichtungsbildschirm.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653633554_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *Bestätigung des Downloads der Authentifizierungs-App*
3. Mit der Authentifizierungs-App hast du jetzt zwei Möglichkeiten:


   Den QR-Code scannen

   1. Öffne die Authentifizierungs-App.
   2. Verwende die App, um den QR-Code zu scannen.
   3. Nach dem Scannen klickst du in Miro auf **Ich habe den Code gescannt**

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683263122_2FA-setup-step-2-Scan-QR-code.png)*Scannen des QR-Codes*

   Den Miro-Code manuell eingeben

   1. Wenn du den QR-Code nicht scannen kannst, klicke in Miro auf **Kannst du den QR-Code nicht scannen?**.
   2. Miro stellt dann einen Authentifizierungscode bereit. **Kopiere** diesen Code.
   3. Öffne deine Authentifizierungs-App und füge den kopierten Code ein.
   4. Nachdem du den Code zur App hinzugefügt hast, klicke in Miro auf **Ich habe den Code hinzugefügt**.

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653636754_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*Den Miro-Code kopieren, um ihn in die Authentifizierungs-App einzufügen*
4. Die Authentifizierungs-App generiert einen 6-stelligen Bestätigungscode. Gib diesen Code in Miro ein und klicke auf **Code bestätigen**.

   ![2FA-setup-step-3-enter-6-digit-code.png](https://help.miro.com/hc/article_attachments/30847469584146)
   *Verifizierung des 6-stelligen Codes*
5. Nachdem du dein Konto erfolgreich mit dem 6-stelligen Code verifiziert hast, stellt Miro einen Wiederherstellungscode bereit. Klicke auf **Kopieren**, um diesen Code sicher zu speichern. Es ist wichtig, dass du diesen Code hast, denn damit kannst du deine 2FA zurücksetzen, falls du den Zugriff auf deine Authentifizierungs-App verlierst.

   Um zu bestätigen, dass du den Code aufgeschrieben hast, wähle **Ich habe diesen Code notiert**, dann klicke auf **Weiter**, um den Vorgang abzuschließen.

   ![Save-2FA-recovery-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683265554_Save-2FA-recovery-code.png)*Wiederherstellungscode speichern*

## Anmeldung mit Zwei-Faktor-Authentifizierung (2FA)

Sobald du die Zwei-Faktor-Authentifizierung (2FA) für dein Konto erfolgreich eingerichtet hast, wirst du bei jedem Anmeldeversuch von Miro aufgefordert, einen 6-stelligen, zeitbasierten, einmaligen Code (TOTP) einzugeben.

Dieser Code wird von deiner Authentifizierungs-App generiert und bietet eine zusätzliche Sicherheitsebene für dein Konto. Öffne einfach deine Authentifizierungs-App, rufe den aktuellen Code ab und gib ihn auf der Anmeldeseite ein, um Zugriff auf dein Konto zu erhalten.

![2fa-user-guide.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/20847806879634_2fa-user-guide.png)
*Anmeldung bei Miro mit 2FA*

Du hast 3 Versuche, bevor du aufgefordert wirst, den Anmeldevorgang neu zu starten.

![Too-many-attempts.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683267346_Too-many-attempts.png)*Zu viele Anmeldeversuche mit 2FA*

### Zwei-Faktor-authentifizierten (2FA) Geräten vertrauen

Wenn dein Admin es eingerichtet hat, kannst du das Kästchen **Diesem Gerät vertrauen** anklicken, wenn du dich mit einem sicheren Gerät bei deinem Konto mit 2FA anmeldest (verwende **Diesem Gerät vertrauen** nicht, wenn du dich von einem freigegebenen oder öffentlich zugänglichen Computer anmeldest). Wenn du dies tust, kannst du dich anmelden, ohne deinen zweiten Faktor einzugeben, bis eine bestimmte Zeitspanne verstrichen ist. Dieser Zeitraum wird von deinem Admin zwischen 7 und 90 Tagen festgelegt.

![2FA-signin.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/19612606396818_2FA-signin.png)

*Die Dauer der Vertrauenswürdigkeit eines Geräts wird bei der Anmeldung mit Zwei-Faktor-Authentifizierung neben dem Kästchen angezeigt*

Wenn du die Option „Diesem Gerät vertrauen“ nicht siehst, hat dein Administrator sie nicht für deine Organisation aktiviert.

Wenn du dich mit einem neuen Gerät anmeldest – oder nachdem du die Cookies auf deinem vertrauenswürdigen Gerät gelöscht hast –, wird die 2FA erneut verlangt.

## So setzt du die Zwei-Faktor-Authentifizierung zurück

Wenn du Probleme mit deiner Authentifizierungs-App hast, dein Gerät verlierst oder die Zwei-Faktor-Authentifizierung aus einem anderen Grund zurücksetzen musst, gehe wie folgt vor:

### Ich habe einen Wiederherstellungscode

1. Klicke auf **Zwei-Faktor-Authentifizierung zurücksetzen**.
2. Verwende den Wiederherstellungscode, den du bei deiner ersten 2FA-Einrichtung gespeichert hast. Du wirst erneut durch den Einrichtungsprozess geführt, um deine Authentifizierungs-App neu zu konfigurieren.

![Reset-two-factor-authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683268114_Reset-two-factor-authentication.png)*Die Option zum Zurücksetzen der Zwei-Faktor-Authentifizierung*

### Ich habe keinen Wiederherstellungscode

Solltest du deinen Wiederherstellungscode verloren haben oder die Wiederherstellung nicht selbst durchführen kannst, musst du deinen Admin bitten, deine 2FA zurückzusetzen.

Wenn deine E-Mail-Domain nicht zu den von deiner Organisation bestätigten Domains gehört, kann dein Admin keinen Reset für dich durchführen. Du musst selbst einen 2FA-Reset anfordern — dein Admin kann diesen dann genehmigen.

Admins können die Zwei-Faktor-Authentifizierung nur für Nutzer zurücksetzen, deren E-Mail-Domains in ihrer Organisation bestätigt sind, sofern der Admin den Reset initiiert. Wenn der Nutzer einen Reset anfordert, kann jeder Admin in der Organisation diesen genehmigen.

Gehe dazu wie folgt vor:

- Klicke auf **Bitte deinen Admin, das Zurücksetzen durchzuführen**.
  ![2fa-user-reset.png](https://help.miro.com/hc/article_attachments/24650802172434)
  *Bitte deinen Admin um das Zurücksetzen deiner 2FA, wenn du keinen Wiederherstellungscode hast*
- Falls du mehreren Organisationen angehörst, die 2FA nutzen, musst du auswählen, an welchen Admin der Organisation du die Anfrage richten möchtest.
- Du erhältst eine E-Mail mit einem Bestätigungscode.
- Gib den Bestätigungscode ein.
- Eine Bestätigung, dass die Anfrage an den gewählten Admin gesendet wurde, wird angezeigt.
- Wenn der Admin deine 2FA zurücksetzt, musst du beim nächsten Anmelden den 2FA-Einrichtungsprozess durchlaufen.

## Häufige Fragen

Warum muss ich die Zwei-Faktor-Authentifizierung einrichten?

Die Zwei-Faktor-Authentifizierung erhöht die Sicherheit für deine Organisation.
Alle Nutzer, die nicht Single Sign-on (SSO) verwenden, müssen sich mit der Zwei-Faktor-
Authentifizierung anmelden, wenn diese Anforderung von deinem Unternehmens-Admin durchgesetzt wird.

Muss ich die 2FA jedes Mal verwenden, wenn ich mich anmelde?

Ja. Nach der Ersteinrichtung musst du deine Authentifizierungs-App für jede Anmeldung verwenden, damit dein Konto geschützt bleibt.

Ich habe versucht, die 2FA einzurichten, habe aber die Fehlermeldung „Ungültiger Code“ erhalten, obwohl mein Code korrekt ist. Was soll ich tun?

Prüfe, ob Zeitzone, Datum und Uhrzeit deines Geräts korrekt eingestellt sind. Wenn das Problem weiterhin besteht, versuche die 2FA auf einem anderen Gerät einzurichten.

Was ist, wenn ich versehentlich einem freigegebenen Gerät vertraue?

Wenn du versehentlich einem freigegebenen Gerät vertraust, musst du die Cookies für Miro auf diesem Gerät löschen. Das zu tun ist einfach:

1. Klicke auf das Symbol mit dem Schieberegler auf der linken Seite der Adressleiste deines Browsers.
2. Klicke im Menü auf „Cookies und Websitedaten“.
3. Klicke dann auf „Websitedaten auf dem Gerät verwalten“.
4. Klicke auf das Papierkorb-Symbol neben jeder URL, um die Cookies und die Daten der Website zu löschen.

Beachte, dass du dich erneut mit der Zwei-Faktor-Authentifizierung anmelden musst, sobald du die Standortdaten von deinem Gerät gelöscht hast.

Was ist, wenn ich den Zugriff auf ein vertrauenswürdiges Gerät verliere?

Wenn du den Zugriff auf ein vertrauenswürdiges Gerät verlierst, bevor der Vertrauenszeitraum abgelaufen ist, kannst du die **Überall abmelden**-Option verwenden, um den Zugriff auf alle angemeldeten Geräte zu entfernen (außer dem Gerät, das du gerade benutzt). Damit meldest du dich von allen anderen Geräten ab und widerrufst 2FA von allen vertrauenswürdigen Geräten. Den Link **Überall abmelden** findest du in den Einstellungen deines Nutzerprofils. Anschließend musst du den 2FA-Anmeldeprozess auf den Geräten, auf die du Zugriff hast, erneut durchlaufen.
