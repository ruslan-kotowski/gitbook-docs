---
title: Zwei-Faktor-Authentifizierung (2FA) – Nutzerleitfaden
article_id: 27601422748434
translation_id: 27601422748434
locale: de
sidebar_position: 2
created_at: '2025-06-24T07:36:23Z'
updated_at: '2025-11-06T13:29:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: 'Relevant für: Starter, Business, Education, Enterprise'
---

## Was ist die Zwei-Faktor-Authentifizierung (2FA)

Die Zwei-Faktor-Authentifizierung (2FA) bietet mehr Sicherheit für deine Online-Konten. Wenn dein Unternehmens-Admin die Zwei-Faktor-Authentifizierung (2FA) aktiviert, wird jede Anmeldung bei Miro mit deiner E-Mail-Adresse und deinem Passwort mit einer zusätzlichen Sicherheitsstufe versehen. Dieser zusätzliche Schritt ist ein weiterer Schutz für dein Konto, denn es wird über die normalen Anmeldeinformationen eine weitere Verifizierung durchgeführt.

:::tip
Erfahre, wie du die Zwei-Faktor-Authentifizierung (2FA) für deine Organisation bei [Enterprise-Preisplänen](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md) sowie [allen anderen Preisplänen](01-two-factor-authentication-2fa.md) aktivierst.
:::

## So richtest du die Zwei-Faktor-Authentifizierung (2FA) ein

**Neue Nutzer:** Bei der ersten [Registrierung](https://miro.com/signup/) mit der E-Mail-Adresse deines Unternehmens wirst du aufgefordert, 2FA zu aktivieren.
**Bestehende Nutzer:** Bei deiner nächsten [Anmeldung](https://miro.com/login/) wirst du, wenn deine Organisation 2FA verlangt und du kein Single Sign-on (SSO) verwendest, aufgefordert, 2FA einzurichten.

1. Lade dir eine Authentifizierungs-App auf dein mobiles Gerät herunter. Authentifizierungs-Apps wie Google Authenticator, Microsoft Authenticator und Authy generieren einen zeitbasierten, einmaligen Code (TOTP) für sichere Anmeldungen bei Miro. Erkundige dich bei deinen Unternehmens- oder IT-Admins nach der passenden App.

2. Klicke auf **Ich habe eine Authentifizierungs-App** im Miro 2FA-Einrichtungsbildschirm.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../docs/administration/security-compliance/images/27601397095698_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *Bestätigung des Downloads der Authentifizierungs-App*
3. Mit der Authentifizierungs-App hast du jetzt zwei Möglichkeiten:


   Den QR-Code scannen

   1. Öffne die Authentifizierungs-App.
   2. Verwende die App, um den QR-Code zu scannen.
   3. Nach dem Scannen klickst du in Miro auf **Ich habe den Code gescannt**

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../docs/administration/security-compliance/images/27601422721298_2FA-setup-step-2-Scan-QR-code.png)*Scannen des QR-Codes*

   Den Miro-Code manuell eingeben

   1. Wenn du den QR-Code nicht scannen kannst, klicke in Miro auf **Kanns’t du den QR-Code nicht scannen?**
   2. Miro stellt dann einen Authentifizierungscode bereit. **Kopiere** diesen Code.
   3. Öffne deine Authentifizierungs-App und füge den kopierten Code ein.
   4. Nachdem du den Code zu der App hinzugefügt hast, klickst du in Miro auf **Ich habe den Code hinzugefügt**.

       ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../docs/administration/security-compliance/images/27601397098898_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*Den Miro-Code kopieren, um ihn in die Authentifizierungs-App einzufügen*
4. Die Authentifizierungs-App generiert einen 6-stelligen Verifizierungscode. Gib diesen Code in Miro ein und klicke auf **Code bestätigen**.

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../docs/administration/security-compliance/images/27601422725906_2FA-setup-step-3-enter-6-digit-code.png)
   *Verifizierung des 6-stelligen Codes*
5. Nachdem du dein Konto erfolgreich mit dem 6-stelligen Code verifiziert hast, stellt Miro einen Wiederherstellungscode bereit. Klicke **Kopieren**, um diesen Code sicher zu speichern. Es ist wichtig, dass du diesen Code hast, denn damit kannst du deine 2FA zurücksetzen, falls du den Zugriff auf deine Authentifizierungs-App verlierst.

   Um zu bestätigen, dass du den Code notiert hast, wähle **Ich habe diesen Code notiert**, dann klicke auf **Weiter**, um den Vorgang abzuschließen.

   ![Save-2FA-recovery-code.png](../../../../../../docs/administration/security-compliance/images/27601422727314_Save-2FA-recovery-code.png)*Wiederherstellungscode speichern*

## Anmeldung mit Zwei-Faktor-Authentifizierung (2FA)

Sobald du die Zwei-Faktor-Authentifizierung (2FA) für dein Konto erfolgreich eingerichtet hast, wirst du bei jedem Versuch, dich anzumelden, von Miro aufgefordert, einen 6-stelligen, zeitbasierten Einmal-Code (TOTP) einzugeben.

Dieser Code wird von deiner Authentifizierungs-App generiert und bietet eine zusätzliche Sicherheitsebene für dein Konto. Öffne einfach deine Authentifizierungs-App, rufe den aktuellen Code ab und gib ihn auf der Anmeldeseite ein, um Zugriff auf dein Konto zu erhalten.

![2fa-user-guide.png](../../../../../../docs/administration/security-compliance/images/27601397105298_2fa-user-guide.png)
*Mit 2FA bei Miro anmelden*

Du hast 3 Versuche, bevor du aufgefordert wirst, den Anmeldevorgang neu zu starten.

![Too-many-attempts.png](../../../../../../docs/administration/security-compliance/images/27601397107474_Too-many-attempts.png)*Zu viele Anmeldeversuche mit 2FA*

### Mit der Zwei-Faktor-Authentifizierung (2FA) Geräten vertrauen

Wenn dein Admin es eingerichtet hat, kannst du das Kästchen **Diesem Gerät vertrauen** anklicken, wenn du dich mit einem sicheren Gerät bei deinem Konto mit 2FA anmeldest (verwende **Diesem Gerät vertrauen** nicht, wenn du dich von einem freigegebenen oder öffentlich zugänglichen Computer anmeldest). Wenn du dies tust, kannst du dich anmelden, ohne deinen zweiten Faktor einzugeben, bis eine bestimmte Zeitspanne verstrichen ist. Dieser Zeitraum wird von deinem Administrator zwischen 7 und 90 Tagen festgelegt.

![2FA-signin.png](../../../../../../docs/administration/security-compliance/images/27601397108882_2FA-signin.png)

*Die Dauer der Vertrauenswürdigkeit eines Geräts wird bei der Anmeldung mit Zwei-Faktor-Authentifizierung neben dem Kästchen angezeigt*

Wenn du die Option „Diesem Gerät vertrauen“ nicht siehst, hat dein Administrator sie nicht für deine Organisation aktiviert.

Wenn du dich mit einem neuen Gerät anmeldest – oder nachdem du die Cookies auf deinem vertrauenswürdigen Gerät gelöscht hast –, wird die 2FA erneut verlangt.

## So setzt du die Zwei-Faktor-Authentifizierung zurück

Wenn du Probleme mit deiner Authentifizierungs-App hast, dein Gerät verlierst oder die Zwei-Faktor-Authentifizierung aus einem anderen Grund zurücksetzen musst, führe folgende Schritte aus:

### Ich habe einen Wiederherstellungscode

1. Klicke auf **Zwei-Faktor-Authentifizierung zurücksetzen**.
2. Verwende den Wiederherstellungscode, den du bei deiner ersten 2FA-Einrichtung gespeichert hast. Du wirst erneut durch den Einrichtungsprozess geführt, um deine Authentifizierungs-App neu zu konfigurieren.

![Reset-two-factor-authentication.png](../../../../../../docs/administration/security-compliance/images/27601422733714_Reset-two-factor-authentication.png)*Die Option zum Zurücksetzen der Zwei-Faktor-Authentifizierung*

### Ich habe keinen Wiederherstellungscode

Wenn du deinen Wiederherstellungscode verloren hast oder die Wiederherstellung nicht selbst durchführen kannst, musst du deinen Admin bitten, deine 2FA zurückzusetzen.

Admins können die Zwei-Faktor-Authentifizierung nur für Nutzer zurücksetzen, deren E-Mail-Domains in ihrer Organisation bestätigt sind, wenn der Admin die Zurücksetzung initiiert. Wenn der Nutzer eine Zurücksetzung anfragt, kann jeder Admin in der Organisation diese freigeben.

1. **Bitte deinen Admin um ein Zurücksetzen** anklicken.
   ![2fa-user-reset.png](../../../../../../docs/administration/security-compliance/images/27601397113106_2fa-user-reset.png)
   *Bitte deinen Admin, deine 2FA zurückzusetzen, wenn du keinen Wiederherstellungscode hast*
2. Wenn du zu mehr als einer Organisation gehörst, die 2FA verwendet, musst du auswählen, für welche Organisation du die Anfrage an den Admin richten möchtest.
3. Du erhältst eine E-Mail mit einem Bestätigungscode.
4. Gib den Bestätigungscode ein.
5. Eine Bestätigung, dass die Anfrage an deinen gewählten Admin gesendet wurde, wird angezeigt.
6. Wenn der Admin deine 2FA zurücksetzt, musst du beim nächsten Anmelden den 2FA-Einrichtungsprozess erneut durchlaufen.

## Häufige Fragen

Warum muss ich die Zwei-Faktor-Authentifizierung einrichten?

Die Zwei-Faktor-Authentifizierung erhöht die Sicherheit für deine Organisation.
Alle Nicht-SSO-Nutzer müssen die Zwei-Faktor-Authentifizierung verwenden, um sich anzumelden, wenn diese Anforderung von deinem Unternehmens-Admin vorausgesetzt wird.

Muss ich die 2FA jedes Mal verwenden, wenn ich mich anmelde?

Ja. Nach der Ersteinrichtung musst du deine Authentifizierungs-App für jede Anmeldung verwenden, damit dein Konto geschützt bleibt.

Ich habe versucht, die Zwei-Faktor-Authentifizierung einzurichten, habe aber die Fehlermeldung „Ungültiger Code“ erhalten, obwohl mein Code korrekt ist. Was soll ich tun?

Prüfe, ob Zeitzone, Datum und Uhrzeit deines Geräts korrekt eingestellt sind. Wenn das Problem weiterhin besteht, versuche die Zwei-Faktor-Authentifizierung auf einem anderen Gerät einzurichten.

Was ist, wenn ich versehentlich einem freigegebenen Gerät vertraue?

Wenn du versehentlich einem freigegebenen Gerät vertraust, musst du die Cookies für Miro auf diesem Gerät löschen. Das zu tun ist einfach:

1. Klicke auf das Symbol mit dem Schieberegler auf der linken Seite der Adressleiste deines Browsers.
2. Klicke im Menü auf „Cookies und Websitedaten“.
3. Klicke dann auf „Websitedaten auf dem Gerät verwalten“.
4. Klicke auf das Papierkorb-Symbol neben jeder URL, um die Cookies und die Daten der Website zu löschen.

Beachte, dass du dich erneut mit der Zwei-Faktor-Authentifizierung anmelden musst, sobald du die Standortdaten von deinem Gerät gelöscht hast.

Was ist, wenn ich den Zugriff auf ein vertrauenswürdiges Gerät verliere?

Wenn du den Zugriff auf ein vertrauenswürdiges Gerät verlierst, bevor der Vertrauenszeitraum abgelaufen ist, kannst du die **Überall abmelden** Option verwenden, um den Zugriff auf alle angemeldeten Geräte zu entfernen (außer dem Gerät, das du gerade benutzt). Damit meldest du dich von allen anderen Geräten ab und widerrufst 2FA von allen vertrauenswürdigen Geräten. Den Link **Überall abmelden** findest du in den Einstellungen deines Nutzerprofils. Anschließend musst du den 2FA-Anmeldeprozess auf den Geräten, auf die du Zugriff hast, erneut durchlaufen.
