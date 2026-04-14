---
title: Hinzufügen mehrerer Identitätsanbieter
article_id: 16287287497234
translation_id: 16287287497234
locale: de
sidebar_position: 1
created_at: '2024-01-10T10:51:24Z'
updated_at: '2026-02-18T08:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Erhältlich für: Enterprise Einrichtung durch: Unternehmens-Admins'
---

:::note
Das Hinzufügen mehrerer Identitätsanbieter ist ein privates Feature, das ausschließlich für Enterprise-Kunden verfügbar ist. Um auf diese Funktion zuzugreifen und sie zu aktivieren, wende dich an deinen Miro Account Team Manager oder Customer Success Manager. Der Miro-Support kann diese Funktion nicht aktivieren.
:::

Verwende mehrere Identitätsanbieter (IdPs) für Single Sign-on (SSO). Dies ist besonders praktisch für große Unternehmen mit mehreren Zweigstellen oder Tochtergesellschaften, die jeweils ihren eigenen IdP haben, aber Zugriff auf dasselbe Miro-Abo benötigen.

## Vorbereitung zum Hinzufügen mehrerer Identitätsanbieter

Um sicherzustellen, dass [Single Sign-on (SSO)](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) nach dem Hinzufügen mehrerer Identitätsanbieter-Apps weiterhin funktioniert, musst du die Konfiguration der bestehenden IdP-App aktualisieren.

Entra ID und einige andere IdPs unterstützen das neue Konfigurationsformat erst, wenn dein Unternehmen die Multi-IdP-Funktion aktiviert. Um Unterbrechungen bei der Anmeldung zu vermeiden, empfehlen wir dir, einen telefonischen Termin mit deinem Customer Success Manager zu vereinbaren, der dich Schritt für Schritt bei der gleichzeitigen Aktivierung der Multi-IdP-Funktion und der Aktualisierung der Konfiguration anleiten kann.

### So konfigurierst du deine Enterprise-Einstellungen

1. SCIM ausschalten.
2. Die SSO-Konfiguration aktualisieren.
3. Die SSO-Funktionalität überprüfen.

#### SCIM deaktivieren

Wir unterstützen derzeit [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) nicht mit mehreren Identitätsanbietern. Um SCIM für deinen Enterprise-Preisplan zu deaktivieren, gehe zu **Unternehmenseinstellungen** > **Konto** > **Enterprise-Integrationen** und schalte **SCIM-Provisionierung** aus.

#### Aktualisiere die SSO-Konfiguration

**Alte Konfiguration**

Wenn Miro Single Sign-on (SSO) ursprünglich in deinem Identitätsanbieter (IdP) konfiguriert wurde, wurden wahrscheinlich die folgenden Konfigurationswerte verwendet:

- **Callback-URL/ACS:** https://miro.com/sso/saml
- **Entity ID:** https://miro.com

**Neue Konfiguration**

Um sicherzustellen, dass der IdP weiß, auf welche Konfiguration er sich in Miro bezieht, müssen die folgenden Werte aktualisiert werden. Gehe zu **Einstellungen** > **Sicherheit** > **Authentifizierung**.

Diese Werte stehen in den SSO-Einstellungen zur Verfügung, sobald dein Unternehmen die private Multi-IdP-Funktion aktiviert hat, und haben folgendes Format:

- **Callback-URL/ACS:** https://miro.com/sso/saml/&lt;org_id&gt;/&lt;saml_settings_id&gt;
- **Entity-ID:** "https://miro.com/&lt;org_id&gt;/&lt;saml_settings_id&gt;

![Callback URL and Entity ID in the Enterprise admin console](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/23763575205778_image.png)

*Callback-URL und Entity-ID in der Enterprise Admin-Konsole*

#### Bestätige die Funktionalität deines Single Sign-on (SSO)

Sobald du deine Identitätsanbieter-Konfiguration aktualisiert hast, teste, ob das Single Sign-on ordnungsgemäß funktioniert, indem du dich ab- und erneut anmeldest.

## Hinzufügen eines neuen Identitätsanbieters (IdP)

Der Prozess zum Hinzufügen neuer Identitätsanbieter (IdPs) ist ähnlich zur bestehenden [Single Sign-on (SSO)-Konfiguration](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), beinhaltet jedoch einige wesentliche Änderungen:

- **Neue Felder:** „IdP-Name“ und „IdP-Beschreibung“ (optional). Diese Felder helfen Nutzern und Admins, den richtigen Identitätsanbieter bei der Anmeldung zu identifizieren, insbesondere wenn mehrere Identitätsanbieter verwendet werden.

  Da diese Felder in den Admin-Einstellungen angezeigt werden und den Nutzern bei der Anmeldung über Single Sign-on (SSO) angezeigt werden können, empfehlen wir dringend, einen eindeutigen Namen zu vergeben (z. B. Geschäftseinheit oder IdP-Name).

  ![idP-name-and-IdP description.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016020733970_idP-name-and-IdP%20description.png)
*Die Option, einen IdP-Namen und eine IdP-Beschreibung hinzuzufügen*
- **Nur-lesbare Felder:** 'Callback URL' (Zulässige Callback-URL, benutzerdefinierte Assertion Consumer Service-URL, Antwort-URL) und 'Entity ID' (Kennung, Relying Party Trust Identifier) werden jetzt automatisch in deinen Miro-IdP-Einstellungen generiert, sobald deine Organisation die private Multi-IdP-Funktion aktiviert hat.

  Bisher waren diese Werte statisch, da sie für alle IdP-Konfigurationen gleich waren. Sobald die Werte generiert wurden, musst du sie auch kopieren und in die entsprechenden Felder in den Einstellungen deines IdP-Anbieters einfügen.

  ![Callback-ID-and-Entity-ID-fields.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034166290_Callback-ID-and-Entity-ID-fields.png)
*Callback-URL- und Entity-ID-Felder*

## Verwaltung mehrerer Identitätsanbieter (IdPs)

> **💡** Du kannst bis zu 20 Identitätsanbieter auf einmal hinzufügen und aktivieren.

Nach dem Hinzufügen der IdPs kann jede Konfiguration nach Bedarf aktiviert oder deaktiviert werden. Um einen IdP zu deaktivieren, gehe zu **Unternehmenseinstellungen** > **Konto** > **Authentifizierung** und deaktiviere den IdP.

![Toggle-on-or-off-IdPs.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034165010_Toggle-on-or-off-IdPs.png)
*Die Option, einen IdP ein- oder auszuschalten*

## Ansicht bei Anmeldung für E-Mail-Domains mit mehreren IdPs

Wenn die E-Mail-Domain eines Nutzers mit mehreren IdP-Konfigurationen verknüpft ist, kann er während der Anmeldung eine auswählen. Wenn diese Konfigurationen verschiedene Domains haben, wird der Nutzer automatisch zum entsprechenden IdP weitergeleitet.

![sso-screenshot.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/22437449166610_sso-screenshot.png)
*Ansicht mehrerer IdPs bei der Anmeldung*
