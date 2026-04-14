---
title: Konfigurieren von Google-SSO
article_id: 4716499382546
translation_id: 4716499382546
locale: de
sidebar_position: 6
created_at: '2022-03-18T18:12:44Z'
updated_at: '2025-11-25T16:08:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Erhältlich für: Business-Preisplan, Enterprise-Preisplan Einrichtung durch:
    Unternehmens-Admin'
---

>  Es wird dringend empfohlen, die Funktion SSO in einem separaten Fenster im Inkognito-Modus deines Browsers zu konfigurieren. Auf diese Weise bleibt die Sitzung im Standardfenster und du kannst die SSO-Autorisierung deaktivieren, falls etwas nicht richtig konfiguriert ist.

Die Konfiguration von Miro in deinem Unternehmen ist mit der Integrations-App, die Google in der Google Workspace Admin-Konsole erstellt hat, einfacher als je zuvor. Diese App ermöglicht es dir, Google SSO für die Verwendung mit Miro sowie die [SCIM-Nutzerbereitstellung](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md) zu konfigurieren.

In diesem Artikel geht es um die Konfiguration von Google SSO für die Verwendung mit Miro.

Wenn du eine Testinstanz einrichten möchtest, bevor du SSO für die Produktion aktivierst, fordere sie bitte bei deiner Kontaktperson bei Miro oder bei einem Vertriebsmitarbeitenden an. Es werden nur diejenigen zu dieser Testinstanz hinzugefügt, die SSO konfigurieren.

>  Im Miro [SSO-Artikel](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)  findest du Regeln, unterstützte Funktionen und optionale Konfigurationseinstellungen.

Lies mehr über die [Einrichtung von Google SSO mit Miro](https://support.google.com/a/answer/14100608#zippy=%2Cstep-set-up-google-as-saml-identity-provider) im Hilfecenter von Google.

## Einrichten von Google SSO für Miro mit SAML

Die Einrichtung von Google SSO zur Authentifizierung bei Miro kann in vier Schritten abgeschlossen werden:

1. Einrichten von Google als SAML-Identitätsanbieter
2. Einrichten von Miro als SAML-Dienstanbieter
3. Aktivieren von Miro für Nutzer
4. Testauthentifizierung

Einrichten von Google als SAML-Identitätsanbieter

1. Klicke in deiner Google Workspace Admin-Konsole auf **Apps > Web- und mobile Apps**
2. Klicke im Panel „Apps“ auf das Dropdown-Menü **App hinzufügen**, wähle „Nach Apps suchen“ und gib „Miro“ ein.
3. Wähle „Miro Web (SAML)“ aus und klicke auf **Auswählen**
4. Stelle unter „Google-Identitätsanbieterdetails“ unter Option 2 sicher, dass „SSO-URL“, „Entity-ID“ und „Zertifikat“ ausgefüllt sind, und klicke dann auf **Weiter.**  Diese Werte wirst du später kopieren, wenn du Miro konfigurierst
5. Füge in den "Details zum Dienstanbieter" die folgenden Werte hinzu:
   **ACS URL:** https://miro.com/sso/saml
   **Entity-ID:** https://miro.com
   **Start-URL:** leer
   **Unterzeichnete Antwort:** nicht ankreuzen
   Name ID EMAIL
6. Klicke auf **Weiter**
7. Wähle unter „Attribut-Mapping“ unter „Google Directory-Attribute“ die Option **Vorname** und dann **Nachname** aus. Stelle dabei sicher, dass sie den App-Attributen zugeordnet werden
8. Klicke auf **Fertigstellen**. Du siehst jetzt, dass deine Miro App dem Google Arbeitsbereich hinzugefügt wurde.
   ![google_sso_configuring_google_settings.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515989394_google_sso_configuring_google_settings.gif)*Einrichten des Google SAML Identitätsanbieters*

Einrichten von Miro als SAML-Dienstanbieter

1. Öffne einen Tab für Inkognito in deinem Browser und melde dich beim Miro-Dashboard an (miro.com/app/dashboard)
2. Klicke auf deinen Avatar in der oberen rechten Ecke und auf **Einstellungen**
3. Klicke in deinen Unternehmenseinstellungen auf **Authentifizierung.**  Wenn du Kunde des Business-Preisplans bist, befindet sich diese Einstellung in der Kategorie Sicherheit.
4. Klicke auf die Umschalttaste für „SSO aktivieren, um die SCIM-Bereitstellung einzurichten“
5. Du wirst zum Abschnitt Authentifizierung in den Unternehmenseinstellungen weitergeleitet. Klicke auf die **SSO/SAML**-Umschalttaste. Du wirst aufgefordert, auf **Aktivieren** zu klicken, um SSO für deine Organisation zu aktivieren
6. Kehre für die **SAML-Anmeldungs-URL** zu deiner Google Workspace Admin-Konsole zurück und klicke in der Miro-App auf **METADATEN HERUNTERLADEN.**  Dieses Panel gibt dir die Option, die erforderlichen Werte zu kopieren
7. Klicke unter **SSO-URL** auf die Schaltfläche **Kopieren**. Gehe zurück zu Miro und kopiere den Wert in die **SAML-Anmeldungs-URL**
8. Wiederhole diesen Vorgang für das **X.509-Zertifikat** mit dem Zertifikat in Google
9. Füge die Informationen deiner **Domain** hinzu. Vergewissere dich, dass du [deine Domain bereits eingerichtet und verifiziert hast](../../canvas-25-admin-features/domain-control/01-domain-control.md)
10. Klicke auf **Speichern![google_sso_configuring_miro_authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515990802_google_sso_configuring_miro_authentication.png)***Konfigurieren der SSO-Authentifizierungseinstellungen in Miro*

Aktivieren von Miro für Nutzer

1. Kehre zur Google Workspace Admin-Konsole zurück
2. Klicke bei Bedarf im Menü „Apps“ auf **Web- und mobile Apps** und wähle **Miro** aus
3. Klicke auf **Nutzerzugriff**
4. Klicke auf **EIN für alle** und dann auf **Speichern![google_sso_turning_on_miro.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528995474_google_sso_turning_on_miro.gif)***Einschalten der Miro-App für alle Nutzer*

Wenn du Miro für bestimmte Organisationseinheiten aktivieren möchtest, klicke zuerst auf die Gruppe in den Organisationseinheiten und dann auf **EIN.**  Möglicherweise musst du zusätzlich auf ÜBERSCHREIBEN oder ÜBERNEHMEN/strong> klicken.

Testauthentifizierung

1. Starte bei Bedarf in der Google Workspace Admin-Konsole die Miro-App
2. Klicke im Abschnitt Miro auf **SAML-ANMELDUNG TESTEN**
3. Es sollte ein neuer Tab mit den Optionen für die Anmeldung bei Google SSO erscheinen
   .GIF
4. Um die Authentifizierung in Miro zu testen, öffne einen neuen Tab für Inkognito-Dateien und starte das Miro-Dashboard (miro.com/app/dashboard)
5. Du solltest eine Anmeldeseite sehen. Klicke auf **Anmeldung mit Single Sign On** und melde dich mit deinen Anmeldeinformationen für das Konto an.
   ![google_sso_testing_authentication.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528996882_google_sso_testing_authentication.gif)*Testen der Google SSO-Authentifizierung mit Miro*

Alternativ kannst du auch in Miro testen:

1. Führe die obigen Schritte aus, um deine SSO-Einstellungen zu konfigurieren.
2. Klicke auf die Schaltfläche **SSO-Konfiguration testen**.
3. Überprüfe die Ergebnisse:
   1. Wenn keine Probleme gefunden werden, wird die Meldung **SSO Konfigurationstest war erfolgreich** angezeigt.
   2. Wenn Probleme gefunden werden, wird die Meldung **SSO-Konfigurationstest fehlgeschlagen** angezeigt, gefolgt von detaillierten Fehlermeldungen, die dir zeigen, was behoben werden muss.![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*SSO-Konfiguration von Miro testen*

> **⚠️** Wenn du zuvor SSO für deine Organisation konfiguriert hast und es neu konfigurieren musst, empfehlen wir dringend, SSO in Miro zu **deaktivieren**, bevor du in der Google Admin-Konsole fortfährst. Andernfalls könntest du dich aus Miro aussperren.  Um eine Profilsperre zu verhindern, erstelle ein provisorisches Nutzerkonto mit einer E-Mail-Adresse, die eine Domain hat, die nicht in den SSO-Einstellungen aufgeführt ist, wie provisorischernutzer@gmail.com. Andernfalls kannst du dich an den Support wenden, der SSO für die gesamte Organisation deaktivieren kann.

Wenn du die Nutzerbereitstellung mit Google konfigurieren möchtest, findest du die Anweisungen im Artikel „[Einrichten der automatisierten Bereitstellung mit Google](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md)“.
