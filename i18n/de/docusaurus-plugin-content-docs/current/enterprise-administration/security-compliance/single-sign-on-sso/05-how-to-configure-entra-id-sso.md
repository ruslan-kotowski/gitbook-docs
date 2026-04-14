---
title: Konfiguration von Entra ID Single Sign-on (SSO)
article_id: 360022722233
translation_id: 360022722233
locale: de
sidebar_position: 5
created_at: '2019-05-07T12:03:08Z'
updated_at: '2025-11-25T16:04:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Erhältlich für: Business-Preisplan, Enterprise-Preisplan Erforderliche Rolle:
    Unternehmens-Admins'
---

> *💡 Es wird dringend empfohlen, die Single Sign-on-Funktion in einem separaten Inkognito-Modus-Fenster deines Browsers zu konfigurieren.* Auf diese Weise bleibt die Sitzung im Standardfenster und du kannst die Single Sign-on-Autorisierung deaktivieren, falls etwas nicht richtig konfiguriert ist.

Wenn du eine Testinstanz einrichten möchtest, bevor du Single Sign-on im Produktivsystem aktivierst, wende dich bitte an das [Support-Team](https://help.miro.com/hc/requests/new?referer=help-center-article), um Unterstützung zu erhalten. Es werden nur diejenigen zu dieser Testinstanz hinzugefügt, die Single Sign-on konfigurieren.

> **⚠️ In unserem Hauptartikel über Single Sign-on** [**hier**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **findest du Regeln, unterstützte Funktionen und die optionale Konfiguration auf der Miro-Seite.**

## Hinzufügen und Konfigurieren der App

 1. Finde die vorkonfigurierte Miro-Anwendung in der Entra ID Enterprise Application Gallery ([Enterprise Applications](https://portal.Entra.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/) > +New Application).

2. Erstelle die App und klicke auf **2.** **Single Sign-on einrichten** (oder wähle **Single Sign-on** auf der linken Seite und wähle die **SAML**-Anmeldemethode aus).

3. Du wirst feststellen, dass die **SAML-Basiskonfiguration** bereits eingerichtet ist:

:::warning
Falls die Single Sign-on-Anmeldung nach der vollständigen Einrichtung fehlschlägt, versuche die Entity-ID von `https://miro.com`auf `https://miro.com/` zu ändern.
:::

:::warning
Sign-on URL (Anmelde-URL), Relay State und Logout URL (Abmelde-URL) (für Single Sign-out) müssen leer gelassen werden, da diese Funktionen nicht unterstützt werden.
:::

Auch die **Attribute und Ansprüche** sind bereits festgelegt:

:::warning
Bitte beachte Folgendes:
a) Der UPN wird zum Hauptparameter, anhand dessen ein Nutzer in Miro erkannt wird, und dieser Parameter kann von der Entra-Seite aus nicht aktualisiert werden. Wenn du die E-Mail-Adressen von Nutzern in Miro aktualisieren musst, ohne SCIM zu verwenden, wende dich bitte an unser [Supportteam](https://help.miro.com/hc/requests/new?referer=help-center-article).
b) Miro akzeptiert [**GivenName,** **Surname**, **DisplayName** und **ProfilePicture**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Andere Attribute werden über Single Sign-on (SSO) nicht unterstützt, können aber über [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md) transferiert werden.
:::

### Erstellen des Zertifikats

1. In Microsoft Entra, stelle sicher, dass das **SAML-Signaturzertifikat** > **Signieroption** entweder **SAML Assertion signieren** oder **SAML-Antwort und Assertion signieren** ist.

2. **Lade** die **Base64**-Datei herunter.

## Konfigurieren von Single Sign-on (SSO) in deinem Miro-Preisplan

1. Öffne die **Base64**-Datei in einem Texteditor und kopiere dann das **x509**-Zertifikat aus der Datei.

2. In Miro, unter **Security > Authentication**, füge das kopierte **x509**-Zertifikat in das Feld **Key x509 certificate** ein.

3. Kopiere in der Microsoft Entra-Einstellungen-UI die **Login-URL**, gehe dann zur Miro **Security > Authentication**-Seite und füge sie in das Feld **URL für SAML-Anmeldung** ein.

4. Auf der Miro **Security >**  **Authentication**-Seite, im Abschnitt **Benutzer aus diesen Domains melden sich mit Single Sign-on (SSO) an**, stelle sicher, dass du mindestens eine Unternehmensdomäne hinzufügst.

:::warning
Stelle in Miro sicher, dass **Profilbilder vom Identitätsanbieter synchronisieren** nicht aktiviert ist. Entra ID unterstützt keine Synchronisierung von Nutzerprofilfotos. Wenn **Profilbilder vom Identitätsanbieter synchronisieren** nicht aktiviert ist, können Nutzer ihre eigenen Profilfotos festlegen.
:::

5. Klicke auf **Speichern**.

Deine Single Sign-on-Konfiguration ist nun abgeschlossen.

## Konfigurieren von Ansprüchen, wenn sich UPN und E-Mail-Adresse unterscheiden

Du kannst die Einstellungen so konfigurieren, dass jedes Entra-Attribut, das im E-Mail-Format vorliegt, als **NameID** in Miro verwendet wird.

### IDP- und SP-initiierte Anmeldungen

*Bei der IDP-initiierten Anmeldung* sendet Entra Miro den Wert, den du als **NameID** verwendest (**user.mail** im Beispiel unten).

Bei diesem Workflow greifen deine Endnutzer über das Symbol in ihrer Portalkonsole auf Miro zu (zum Beispiel unter `https://myapplications.microsoft.com/`). Von dort wird eine Anfrage an Miro gesendet und *der Nutzer wird mit der von dir definierten **NameID** angemeldet.*Miro erwartet, dass dieses Attribut mit der **E-Mail-Adresse** des Nutzers in Miro übereinstimmt. Eine Nichtübereinstimmung führt zu einer fehlgeschlagenen Authentifizierung.

*Bei der SP-initiierten Anmeldung* sendet Miro eine Anfrage speziell für die **UPN** des Nutzers und erwartet, dass diese mit der **E-Mail-Adresse** des Nutzers in Miro übereinstimmt. Eine Nichtübereinstimmung führt zu einer fehlgeschlagenen Authentifizierung.

Jetzt wird erwartet, dass das Feld mit der **SAML-Anmeldungs-URL** in deinen Miro-Einstellungen die **Login-URL** der Miro-App in deiner Entra-Instanz enthält. Dies wird die URL sein, zu der Miro den Nutzer von der [Miro-Anmeldeseite](https://miro.com/sso/login/) weiterleiten wird.

Wenn der Nutzer von der App zur Login-URL weitergeleitet wird, wird die SAML-Anfrage generiert. Bei diesem Workflow wird der Nutzer mit der E-Mail-Adresse angemeldet, die er auf der Miro-Anmeldeseite eingegeben hat und die Miro dann von Entra anfordert, wobei erwartet wird, dass sie das UPN-Attribut ist.

### Vorgehensweise bei der Einrichtung

Damit deine Nutzer über die Entra-**E-Mail** und nicht über den **UPN** auf Miro zugreifen können, kannst du das Feld **SAML-Anmelde-URL** in Miro mit der URL der App aus der Entra-Konsole ausfüllen. Dann sieht der SP-initiierte Workflow wie folgt aus:

1. Der Nutzer greift auf Miro zu, indem er seine Miro-E-Mail-Adresse eingibt, die er in Miro hinterlegt hat. Miro erkennt, dass die Person mit dem definierten Nutzerprofil angemeldet sein sollte.
2. Der Nutzer wird zu seinem App-Link weitergeleitet, der für die Identitätsanbieter-initiierte Anmeldung verwendet wird.
3. Der Link verwendet das **NameID**-Attribut *das du definiert hast* und sendet es an Miro.
4. Der Nutzer wird also in Miro in dem zuvor definierten Nutzerprofil mit der von dir festgelegten **NameID** angemeldet.

Schau dir [diesen Artikel](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md) an, wenn du die automatische Bereitstellung für Miro aktivieren möchtest.

Sieh dir bitte [diesen Artikel](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md) an, falls du während der Konfiguration auf Probleme gestoßen bist.

## Entra Testing Tool

Um zum Testing Tool zu gelangen, wähle die Registerkarte **Single Sign-in** in den Einstellungen deiner App und scrolle bis zum Ende des Abschnitts nach unten.

Entra empfiehlt, den Prozess zur Testanmeldung zu verwenden, um die Verbindung zu überprüfen und eine Fehlermeldung zu beheben. Nach dem Test erhältst du Anweisungen, wie du die Situation lösen kannst.

Bitte denke daran, mit welchen von Entra/ADFS verwalteten Anmeldeinformationen deine Workstation authentifiziert ist. Wenn du versuchst, dich mit einem anderen Satz von Anmeldeinformationen bei Miro anzumelden, kann der Anmeldeversuch fehlschlagen, da der Identitätsanbieter deinen Hauptsatz von Anmeldeinformationen überträgt und es zu einer Nichtübereinstimmung kommt. Das kann zum Beispiel passieren, wenn du der SSO-Admin bist und das Anmeldeverfahren mit anderen Nutzer-Anmeldedaten testest.

## Alternativ kannst du in Miro testen

1. Führe die obigen Schritte aus, um deine SSO-Einstellungen zu konfigurieren.
2. Klicke auf die Schaltfläche **SSO-Konfiguration testen**.
3. Überprüfe die Ergebnisse:
   1. Wenn keine Probleme gefunden werden, wird die Bestätigungsmeldung **SSO-Konfigurationstest war erfolgreich** angezeigt.
   2. Wenn Probleme gefunden werden, wird die Bestätigungsmeldung **SSO-Konfigurationstest fehlgeschlagen** angezeigt, gefolgt von detaillierten Fehlermeldungen, die dir zeigen, was behoben werden muss.

##
