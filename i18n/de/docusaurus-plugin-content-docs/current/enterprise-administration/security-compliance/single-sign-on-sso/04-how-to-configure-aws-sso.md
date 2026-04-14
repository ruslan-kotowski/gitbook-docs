---
title: Konfigurieren von AWS SSO
article_id: 360014798100
translation_id: 360014798100
locale: de
sidebar_position: 4
created_at: '2020-07-01T20:03:44Z'
updated_at: '2025-02-26T11:33:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Erhältlich für: Enterprise-, Business-Preisplan** Einrichtung durch: Unternehmens-Admin'
---

>  Es wird dringend empfohlen, die Funktion SSO in einem separaten Fenster im Inkognito-Modus deines Browsers zu konfigurieren. Auf diese Weise bleibt die Sitzung im Standardfenster und du kannst die SSO-Autorisierung deaktivieren, falls etwas nicht richtig konfiguriert ist.

Wenn du eine Testinstanz einrichten möchtest, bevor du SSO für die Produktion aktivierst, fordere sie bitte bei deiner Kontaktperson bei Miro oder bei einem Vertriebsmitarbeitenden an. Es werden nur diejenigen zu dieser Testinstanz hinzugefügt, die SSO konfigurieren.

> **⚠️ In unserem Hauptartikel über SSO** [**hier**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **findest du Regeln, unterstützte Funktionen und die optionale Konfiguration auf der Miro-Seite.**

## Voraussetzungen

Zum Einrichten des AWS SSO-Zugangs mit Miro benötigst du Folgendes:

1. Zugriff auf die AWS SSO-Konsole mit IAM-Berechtigungen zur Anwendungsverwaltung.
2. Admin-Berechtigungen auf Unternehmensebene für den Enterprise- oder Business-Preisplan von Miro.

## Anweisungen für die Einrichtung

1. Füge auf der Seite zum Konfigurieren von AWS SSO eine neue Anwendung hinzu und suche nach **Miro**.    Beim Hinzufügen der Miro App können der Anzeigename und die Beschreibung aktualisiert werden.
   application_catalog.jpg
   AWS SSO-Anwendungskatalog
2. Logge dich in einem anderen Browserfenster in die Miro-Übersicht ein.  Wir empfehlen hierfür ein separates Inkognito-Browserfenster./span>
3. Klicke oben rechts auf dein Profilsymbol und gehe dann zu **Einstellungen**.  Vergewissere dich, dass im linken Bedienfeld das richtige Team aus dem Dropdown-Menü oben links ausgewählt ist.
4. Gehe im linken Bedienfeld zu **Enterprise-Integrationen** (Nutzer des Business-Preisplans müssen zu **Sicherheit** gehen) und aktiviere die Umschaltfunktion **SSO/SAML aktivieren**.  Gib den folgenden Wert für die SAML Sign-in URL von AWS SSO ein.

application_configuration_page.jpg
AWS SSO – Seite für die Anwendungskonfiguration

5. Lade die AWS SSO-SAML-Metadaten-Datei herunter und kopiere das Zertifikat X509 und füge es in das **Zertifikat Key x509** ein.  Deine Konfiguration in Miro sollte jetzt in etwa so wie die folgende Konfiguration aussehen.

Miro_SSO_settings.jpg
SSO-Konfigurationseinstellungen in Miro

6. Gib in der SSO-Konfiguration von Miro den E-Mail-Domänennamen deines Unternehmens in den Wert für **Domänen** ein.  Vergewissere dich, dass du mindestens eine Unternehmensdomäne hinzugefügt hast.
7. Klicke auf **Speichern**, um die Änderungen zu übernehmen.
8. Kehre zu deiner Anwendung für Miro in der AWS SSO-Webkonsole zurück.  Überprüfe unter Anwendungsmetadaten, ob die folgenden Werte eingetragen sind. Diese sollten automatisch eingefügt werden, wenn du nach der Miro-Anwendung gesucht und sie hinzugefügt hast, anstatt eine eigene Anwendung zu erstellen.
9. |  |  |
   | --- | --- |
   | **Feld** | **Wert** |
   | ACS-URL der Anwendung | [https://miro.com/sso/saml](https://Miro.com/sso/saml) |
   | SAML-Publikum der Anwendung | https://miro.com/ |
10. Wähle **Änderungen speichern** aus.
11. Weise der Anwendung unter zugewiesene Nutzer der Anwendung in der AWS SSO-Konsole einen [Nutzer zu.](https://docs.aws.amazon.com/singlesignon/latest/userguide/assignuserstoapp.html)

Das wars auch schon! Deine SSO-Konfiguration ist nun abgeschlossen.

Schau dir diesen Artikel an, wenn du die automatische Bereitstellung für Miro aktivieren möchtest.

## Testen

Im folgenden Abschnitt erfährst du, wie du die SSO-Integration verifizieren kannst.  Stelle vor der Verifizierung sicher, dass der Nutzer, der die Verifizierung durchführt, sowohl bei AWS SSO als auch bei Miro abgemeldet ist, bevor er die folgenden Schritte durchführt. Ein Nutzer kann sich nur dann mit SSO anmelden, wenn er in deinem Verzeichnis existiert, Mitglied deines Enterprise- oder Business-Preisplans in Miro ist und er der App zugewiesen ist./span>

### Verifizieren von IdP-initiiertem SSO von AWS SSO

1. Greife mit den Anmeldedaten eines/einer der Miro-Anwendung zugewiesenen Nutzer auf das AWS SSO-Endnutzerportal zu.
2. Wähle in der Liste der Anwendungen die Miro-Anwendung aus, um eine Anmeldung bei Miro einzuleiten.
3. Bei erfolgreicher Anmeldung wirst du in der Miro-Übersicht eingeloggt.

### Verifizieren des vom Dienstanbieter initiierten SSO von Miro

1. Rufe [https://miro.com/login/](https://Miro.com/login/) auf und wähle **Mit SSO einloggen** aus.  Gib dann deine geschäftliche E-Mail-Adresse ein.
2. Du wirst zum AWS SSO-Portal weitergeleitet. Dort musst du die Anmeldedaten eines/einer der Anwendung zugewiesenen Nutzer in die AWS SSO-Konsole eingeben.
3. Bei erfolgreicher Anmeldung wirst du in der Miro-Übersicht eingeloggt.

### Alternativ kannst du auch in Miro testen

1. Führe die obigen Schritte aus, um deine SSO-Einstellungen zu konfigurieren.
2. Klicke auf die Schaltfläche **SSO-Konfiguration testen**.
3. Überprüfe die Ergebnisse:
   1. Wenn keine Probleme gefunden werden, wird die Meldung **SSO Konfigurationstest war erfolgreich** angezeigt.
   2. Wenn Probleme gefunden werden, wird die Meldung **SSO-Konfigurationstest fehlgeschlagen** angezeigt, gefolgt von detaillierten Fehlermeldungen, die dir zeigen, was behoben werden muss.![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*SSO-Konfiguration von Miro testen*

## Fehlerbehebung

Allgemeine Hinweise zur Fehlerbehebung findest du im [AWS SSO-Leitfaden zur Fehlerbehebung](http://docs.aws.amazon.com/singlesignon/latest/userguide/troubleshooting.html).
