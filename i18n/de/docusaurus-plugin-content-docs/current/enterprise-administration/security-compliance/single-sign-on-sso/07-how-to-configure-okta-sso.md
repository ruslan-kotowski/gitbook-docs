---
title: So konfigurierst du OKTA SSO
article_id: 360023901054
translation_id: 360023901054
locale: de
sidebar_position: 7
created_at: '2019-05-31T11:32:41Z'
updated_at: '2025-11-25T16:05:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Erhältlich für: Enterprise-, Business-Preisplan** Einrichtung durch: Unternehmens-Admin'
---

>  Es wird dringend empfohlen, die Funktion SSO in einem separaten Fenster im Inkognito-Modus deines Browsers zu konfigurieren. Auf diese Weise bleibt die Sitzung im Standardfenster und du kannst die SSO-Autorisierung deaktivieren, falls etwas nicht richtig konfiguriert ist.

[Wenn du eine Testinstanz einrichten möchtest, bevor du SSO im Produktivsystem aktivierst, wende dich bitte an das Support-Team, um Unterstützung zu erhalten.](https://help.miro.com/hc/requests/new?referer=help-center-article) Es werden nur diejenigen zu dieser Testinstanz hinzugefügt, die SSO konfigurieren.

> **⚠️ In unserem Hauptartikel über SSO** [**hier**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **findest du Regeln, unterstützte Funktionen und die optionale Konfiguration auf der Miro-Seite.**

## Okta einrichten

### Hinzufügen und Konfigurieren der App

Klicke auf die Registerkarte **Anwendungen** und wähle die Option **App-Katalog durchsuchen**:

browse_app_catalog.jpg
Anwendungsbereich in Okta

Suche nach unserer vorkonfigurierten App für die einfache Einrichtung und klicke, um sie **hinzuzufügen**:

Miro_pre-configured_app.jpg
Miro im Okta App-Katalog

Gib der App in deiner Galerie die gewünschte Bezeichnung (weitere Schritte sind optional) und klicke auf **Weiter**, um zur Registerkarte **Anmeldeoptionen** zu wechseln:

general_settings.jpg
Allgemeine Einstellungen der Miro-App

In den **Anmeldeoptionen** sind alle von uns benötigten Werte bereits ausgefüllt und es werden keine zusätzlichen Daten benötigt.

:::warning
Du kannst auf Wunsch individuelle Werte hinzufügen, aber vergewissere dich, dass **Default Relay State** *leer* bleibt: Unsere eigenständigen Apps verwenden während des Authentifizierungsprozesses eine Umleitung an den Browser des Endnutzers und generieren hierfür eindeutige RelayState-Werte. Wenn du einen Standardwert verwendest, überschreibt Okta unsere Daten und deine Personen können nur auf die Browserversion von Miro, aber nicht auf die eigenständigen Apps (Desktop, Tablet, Smartphone) zugreifen.
:::

sign-on_options.jpg
Anmeldemethoden

Klicke zum **Fertigstellen**. Du kannst später bei Bedarf zurückgehen und beliebige Felder bearbeiten.

### Format für Nutzernamen

>  Das **Format für Anwendungsnutzernamen** ist standardmäßig auf den **Okta-Nutzernamen** festgelegt. Es ist in Ordnung, wenn dein Nutzername eine E-Mail-Adresse ist. Lege alternativ den Nutzernamen auf eine **E-Mail-Adresse** fest.

:::warning
Die E-Mail-Adresse ist die primäre Identifikationsmethode, über die Personen in Miro erkannt werden. Sie sollte nicht in Okta aktualisiert werden, außer du hast SCIM aktiviert. Wenn du SCIM nicht verwendest, aber die E-Mail-Adressen von Endnutzer aktualisieren musst, wende dich bitte an unser [Supportteam](https://help.miro.com/hc/requests/new?).
:::

### Profilbilder konfigurieren (optional)

Das Einrichten eines benutzerdefinierten Attributs wie ProfilePicture kann als separater Prozess angesehen werden. Halte dich an diesen [Leitfaden](https://drive.google.com/file/d/1go4BJWzFpQS5R04WdN1Q4O5Dy93k4wGp/view), um das Attribut in Okta einzurichten, und [aktiviere anschließend die ProfilePicture-Anforderung](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) in Miro.

## Miro einrichten

Scrolle nach unten zu **SAML-Signaturzertifikate**, um die IDP-Metadaten zu erhalten. Wenn du keine ausgestellten Zertifikate hast, erstelle zunächst eines.

Klicke anschließend auf **Aktionen** und wähle **IdP-Metadaten anzeigen**:

view_Idp_metadata.jpg
IdP-Metadaten abrufen

Du wirst zu einer separaten Registerkarte weitergeleitet, die alle Informationen enthält. Kopiere das Zertifikat ab der Zeile, die mit &lt;ds:X509Certificate&gt; beginnt, und kopiere es in die Miro-SSO-Einstellungen im Feld Key x509 Certificate/span>**.**

certificate_in_Miro_SSO_settings.jpg
 /span>Key x509-Zertifikat in den Miro SSO-Einstellungen

Gehe zurück zur Metadaten-Seite und kopiere die URL aus der Zeile **SingleSignOnService** nach **Location=**und füge sie in **SAML Sign-in URL** ein.

Fertig!

Füge als letzten Schritt der Miro-Einstellungen deine Domänen hinzu und [verifiziere sie](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Außerdem kannst du die optionalen Einstellungen konfigurieren.

Falls Probleme auftreten, wirf einen Blick auf unsere Liste häufiger Probleme und möglicher Lösungen.

## SSO-Konfiguration in Miro testen

1. Führe die obigen Schritte aus, um deine SSO-Einstellungen zu konfigurieren.
2. Klicke auf die Schaltfläche **SSO-Konfiguration testen**.
3. Überprüfe die Ergebnisse:

- Wenn keine Probleme gefunden werden, wird die Meldung **SSO Konfigurationstest war erfolgreich** angezeigt.
- Wenn Probleme gefunden werden, wird die Meldung **SSO-Konfigurationstest fehlgeschlagen** angezeigt, gefolgt von detaillierten Fehlermeldungen, die dir zeigen, was behoben werden muss.

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*SSO-Konfiguration in Miro testen*
