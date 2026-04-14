---
title: Konfigurieren von ADFS SSO
article_id: 360022411353
translation_id: 360022411353
locale: de
sidebar_position: 2
created_at: '2019-04-29T20:13:47Z'
updated_at: '2025-11-25T16:04:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '**Erhältlich für: Enterprise-, Business-Preisplan** Einrichtung durch: Unternehmens-Admin'
---

Miro unterstützt Single-Sign-On (SSO) über SAML 2.0.

Ein SAML 2.0-Identitätsanbieter (IdP) kann viele Formen annehmen, einschließlich eines selbst gehosteten Active Directory Federation Services (ADFS)-Servers. ADFS ist ein von Microsoft als Standardrolle für Windows Server bereitgestellter Service, der ein Web-Login unter Verwendung bestehender Active-Directory-Zugangsdaten bereitstellt.

In dieser Anleitung findest du Screenshots aus **Server 2012R2**, aber ähnliche Schritte sollten auch in anderen Versionen möglich sein.

Zunächst musst du ADFS auf deinem Server installieren. Die Konfiguration und Installation von ADFS liegt außerhalb des Umfangs dieses Leitfadens, wird aber in diesem [Microsoft-Artikel](http://msdn.microsoft.com/library/gg188612.aspx) detailliert beschrieben.

Vergewissere dich während des Tests, dass die Authentifizierung für deine Working Station auf dieselbe E-Mail-Adresse gestellt ist, die du für den Test verwendest – andernfalls erlaubt dir ADFS selbst mit korrekter Konfiguration und korrektem Profil nicht, dich einzuloggen.

>  Es wird dringend empfohlen, die Funktion SSO in einem separaten Fenster im Inkognito-Modus deines Browsers zu konfigurieren. Auf diese Weise bleibt die Sitzung im Standardfenster und du kannst die SSO-Autorisierung deaktivieren, falls etwas nicht richtig konfiguriert ist.

Wenn du eine Testinstanz einrichten möchtest, bevor du SSO für die Produktion aktivierst, fordere sie bitte bei deiner Kontaktperson bei Miro oder bei einem Vertriebsmitarbeitenden an. Es werden nur diejenigen zu dieser Testinstanz hinzugefügt, die SSO konfigurieren.

> **⚠️ In unserem Hauptartikel über SSO** [**hier**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **findest du Regeln, unterstützte Funktionen und die optionale Konfiguration auf der Miro-Seite.**

## Schritt 1 - Relying Party Trust hinzufügen

1) Melde dich beim ADFS-Server an und starte die **ADFS Management-Konsole**.

2) Wähle den Ordner **Relying Party Trusts**aus **AD FS Management** und füge ein neues **Standard Relying Party Trust** aus der Seitenleiste **Actions**hinzu. Dadurch wird der Konfigurations-Assistent für den neuen Trust gestartet.

add_a_party_trust.jpg
Party Trust hinzufügen

3) Wähle im Bildschirm **Select Data Source** die letzte Option **Enter Data About the Party Manually.**

step_3.jpg
**Wähle Enter Data About the Party Manually**

4) Gib einen **Displaynamen** ein, den du in der Zukunft erkennen wirst, und alle Anmerkungen, die du vornehmen möchtest.

display_name.jpg
Displaynamen hinzufügen

5) Wähle die Schaltfläche **ADFS FS (ADFS 2.0) Profil** aus.

step_5.jpg

next.jpg
Du wirst aufgefordert, nach einem Zertifikat zu suchen, um die Ansprüche zu ver- und entschlüsseln. Dies ist optional. Du kannst es durch Klick auf **Weiter** überspringen.

6) Aktiviere das Label " **Enable Support for the SAML 2.0 WebSSO protocol**".
Die URL des Dienstes lautet https://miro.com/sso/saml.

**Beachte**, dass am Ende der URL kein Schrägstrich steht.

step_6.jpg
Support für das SAML 2.0 WebSSO Protokoll aktivieren

7) Füge eine **Relying Party Trust Identifizierung** als `https://miro.com/` hinzu

step_7.jpg
**Relying Party Trust Identifizierung hinzufügen**

*Auf dem nächsten Bildschirm kannst du die Multifaktor-Authentifizierung konfigurieren, aber dies liegt außerhalb des Umfangs dieses Leitfadens.*

rejecting_on_step_7.jpg
*Ablehnen der Konfiguration der Multifaktor-Authentifizierung*

8) Wähle die Option **Permit all users to access this relying party** (Allen Nutzern Zugriff auf die Relying Party gewähren).

step_8.jpg
Allen Nutzern Zugriff auf die Relying Party gewähren

Auf den nächsten zwei Bildschirmen zeigt der Assistent eine Übersicht über deine Einstellungen.

Klicke auf dem Endbildschirm auf **Close** (Schließen) und öffne den Editor **Claim Rules** (Anspruchsregeln).

final_step.jpg
Abschluss des Hinzufügens eines Relying Party Trust

Vergewissere du dich außerdem, dass deine Konfiguration **Signed Assertion** (signierte Bestätigung) beinhaltet.

## Schritt 2 - Anspruchsregeln erstellen

Sobald die Treuhandgesellschaft erstellt wurde, kannst du die Anspruchsregeln erstellen.
Standardmäßig wird der Bearbeiter der Anspruchsregel geöffnet, sobald du den Trust erstellt hast.

1) Klicke auf **Add Rule** (Regel hinzufügen), um eine neue Regel zu erstellen.

adding_a_rule.jpg
Neue Regel hinzufügen

2) Erstelle die Regel **Send LDAP Attribute as Claims**(LDAP Attribute als Ansprüche senden).

claim_rule_template.jpg
Eine Regel erstellen

3) Auf dem nächsten Bildschirm kannst du die Regel benennen, und sie unter Einsatz des **Active Directory** als dein Attributspeicher wie folgt mappen:

| LDAP Attribut | Ausgehende Anspruchsart |
| --- | --- |
| E-Mail-Adressen | E-Mail-Adresse |
| Given-Name | FirstName |
| Surname | LastName |

map_LDAP_attributes.jpg
Mapping von LDAP-Attributen

Klicke auf **OK**, um die neue Regel zu speichern.

4) Erstelle eine weitere neue Regel, indem du auf**Add Rule** (Regel hinzufügen) klickst und dieses Mal **Transform an Incoming Claim** (Eingehenden Anspruch umwandeln) als Vorlage wählst.

add_another_rule.jpg
**Auswahl von Transform an Incoming Claim als Vorlage**

5) Benenne dann die Regel und lege die folgenden Parameter fest:

|  |  |
| --- | --- |
| **Eingehende Anspruchsart** | E-Mail-Adresse |
| **Ausgehende Anspruchsart** | Name ID |
| **Ausgehende Namens-ID Format** | Email |

set_rule_parameters.jpg
Regelparameter festlegen

Klicke schließlich auf **OK**, um die Anspruchsregel zu erstellen und dann erneut auf **OK**, um die Regelerstellung zu beenden.

Und damit hast du die ADFS-Konfiguration abgeschlossen! Wenn du danach einfach [die SSO-Funktion für deinen Miro-Preisplan](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) aktivierst, können die Personen SAML einsetzen, um sich in Miro zu authentifizieren.

## SSO-Konfiguration in Miro testen

1. Führe die obigen Schritte aus, um deine SSO-Einstellungen zu konfigurieren.
2. Klicke auf die Schaltfläche **SSO-Konfiguration testen**.
3. Überprüfe die Ergebnisse:

1. Wenn keine Probleme gefunden werden, wird die Meldung **SSO Konfigurationstest war erfolgreich** angezeigt.
2. Wenn Probleme gefunden werden, wird die Meldung **SSO-Konfigurationstest fehlgeschlagen** angezeigt, gefolgt von detaillierten Fehlermeldungen, die dir zeigen, was behoben werden muss.

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*SSO-Konfiguration in Miro testen*
