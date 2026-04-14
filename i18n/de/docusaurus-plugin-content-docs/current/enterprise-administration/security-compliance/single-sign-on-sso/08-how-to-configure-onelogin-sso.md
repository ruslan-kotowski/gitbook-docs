---
title: So konfigurierst du OneLogin SSO
article_id: 360022547134
translation_id: 360022547134
locale: de
sidebar_position: 8
created_at: '2019-05-07T13:32:16Z'
updated_at: '2025-02-26T11:22:04Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Erhältlich für: Enterprise-, Business-Preisplan** Einrichtung durch: Unternehmens-Admin'
---

>  Es wird dringend empfohlen, die Funktion SSO in einem separaten Fenster im Inkognito-Modus deines Browsers zu konfigurieren. Auf diese Weise bleibt die Sitzung im Standardfenster und du kannst die SSO-Autorisierung deaktivieren, falls etwas nicht richtig konfiguriert ist.

Wenn du eine Testinstanz einrichten möchtest, bevor du SSO für die Produktion aktivierst, fordere sie bitte bei deiner Kontaktperson bei Miro oder bei einem Vertriebsmitarbeitenden an. Es werden nur diejenigen zu dieser Testinstanz hinzugefügt, die SSO konfigurieren.

> **⚠️ In unserem Hauptartikel über SSO** [**hier**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **findest du Regeln, unterstützte Funktionen und die optionale Konfiguration auf der Miro-Seite.**

## Einrichten von Onelogin

### Hinzufügen und Konfigurieren der App

Die Konfiguration von OneLogin in Miro ist einfach, da OneLogin über eine vorkonfigurierte funktionierende Miro-Anwendung im **App**-Katalog verfügt.

Miro_in_OneLogin_apps.jpg
Miro im OneLogin App-Katalog.

Klicke auf die Schaltfläche **Speichern**.

save_button.jpg
Registerkarte für die Anwendungskonfiguration in OneLogin.

## Miro einrichten

Nach dem Speichern der Konfiguration wirst du direkt zu den Anwendungseinstellungen weitergeleitet. Wechsle zur Registerkarte **SSO**, um deine **Login URL** und dein **x509 Certificate** zu erhalten.

sso_tab.jpg
Registerkarte „SSO“

Im Folgenden siehst du eine Liste von URLs. Kopiere die URL **SAML 2.0 Endpoint (HTTP)**:

SAML_endpoint.jpg

und ***füge*** sie in das Feld **SAML Sign-In URL** in Miro ein:

sign-in_URL.jpg
**Das Feld SAML Sign-In URL in Miro.**

Gehe zurück zur Registerkarte „SSO“ der Anwendung OneLogin und klicke auf **Details anzeigen**, um das **x509 Certificate** zu kopieren.

view_details.jpg
Schaltfläche „Details anzeigen“

copy_certificate.jpg
**Kopieren des x509 Certificate**

Füge das Zertifikat in das Feld **x509 Certificate** in Miro ein.

certificate_in_Miro_SSO_settings.jpg
**Feld x509 Certificate in den SSO-Einstellungen von Miro.**

Füge als letzten Schritt der Miro-Einstellungen deine Domänen hinzu und [verifiziere sie](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Außerdem kannst du die optionalen Einstellungen konfigurieren.

Da jetzt alles eingerichtet ist, können sich deine Nutzer von nun an über SSO in Miro authentifizieren!

Falls Probleme auftreten, wirf einen Blick auf unsere Liste häufiger Probleme und möglicher Lösungen.

## SSO-Konfiguration in Miro testen

1. Führe die obigen Schritte aus, um deine SSO-Einstellungen zu konfigurieren.
2. Klicke auf die Schaltfläche **SSO-Konfiguration testen**.
3. Überprüfe die Ergebnisse:

- Wenn keine Probleme gefunden werden, wird die Meldung **SSO Konfigurationstest war erfolgreich** angezeigt.
- Wenn Probleme gefunden werden, wird die Meldung **SSO-Konfigurationstest fehlgeschlagen** angezeigt, gefolgt von detaillierten Fehlermeldungen, die dir zeigen, was behoben werden muss.

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*SSO-Konfiguration in Miro testen*
