---
title: Nutzerbereitstellung im Enterprise-Plan
article_id: 4403139914130
translation_id: 4403139914130
locale: de
sidebar_position: 13
created_at: '2021-07-01T07:59:23Z'
updated_at: '2025-11-25T16:05:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: scim
---

Mit der automatischen Bereitstellung werden alle neuen Nutzer innerhalb deiner Unternehmensdomains zu deinem Enterprise-Abo weitergeleitet und erhalten Zugriff auf die Assets deines Unternehmens.

Miro Enterprise bietet verschiedene Bereitstellungsoptionen: Einladungen, Just-in-Time-Bereitstellung (JIT), System für domainübergreifendes Identitätsmanagement (SCIM) und Domainsteuerung.

> **Erhältlich für:** Enterprise-Preisplan

## Einladungen

Du kannst Nutzer zu deinem Abo einladen, indem du auf die Schaltfläche **Mitglieder einladen** in deinem Dashboard klickst. Einladungen werden sofort gesendet und erfordern keine zusätzliche Einrichtung.

Erfahre mehr darüber, wie du deine Arbeit in Miro freigeben und mit anderen zusammenarbeiten kannst, indem du [Einladungen im Enterprise Preisplan verwalten](05-manage-user-invitations-on-enterprise-plan.md) und [Boards teilen und Mitwirkende einladen](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) besuchst.

![invite_members_button.jpg](../../../../../../docs/enterprise-administration/user-management/images/21017653284754_invite%20members%20button.jpg)*Die Option, Mitglieder auf dem Miro-Dashboard einzuladen*

## Just-in-Time-Bereitstellung (JIT)

Die JIT-Bereitstellung, integriert mit [Single Sign-on (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), fügt automatisch alle neuen Nutzer, die unter deinen SSO-Domains deines Unternehmens registriert sind, einem bestimmten Team in deinem Enterprise-Preisplan hinzu.
Die JIT-Bereitstellung kann ganz einfach in deinen Miro SSO-Einstellungen aktiviert werden. Erfahre [wie man SSO einrichtet](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

![user_provisioning_jit_provisioning.png](../../../../../../docs/enterprise-administration/user-management/images/21017682931730_user_provisioning_jit_provisioning.png)*Aktivierung der Just-in-Time (JIT) Bereitstellung in den SSO-Einstellungen*

## System for Cross-domain Identity Management (SCIM)

SCIM, integriert mit [Single Sign-on (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), ermöglicht es dir, Nutzer in deinem Enterprise-Preisplan über deinen gewählten Identitätsanbieter (IdP) automatisch bereitzustellen und zu verwalten.

Wenn SCIM aktiviert ist, kannst du Nutzer zu bestimmten Teams hinzufügen, ihre Details und E-Mail-Adressen aktualisieren und ihren Aktivierungsstatus direkt innerhalb deines gewählten Identitätsanbieters verwalten. Diese Funktion automatisiert den Austausch von Nutzerinformationen zwischen deinem Miro-Konto und deinem IdP.

SCIM automatisiert den Austausch von Nutzerinformationen zwischen Miro und deinem IdP, sodass du den Zugriff der Mitarbeitenden auf deinen Enterprise-Preisplan zentral über den IdP verwalten kannst.

Erfahre mehr über die [SCIM-Funktionen](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) und überprüfe die Konfigurationsschritte für [Entra ID](../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md), [OKTA](../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md) oder [OneLogin](../security-integrations/system-for-cross-domain-identity-management-scim/06-setting-up-automated-provisioning-with-onelogin.md).

## Domainsteuerung

[Domainsteuerung](../canvas-25-admin-features/domain-control/01-domain-control.md) ermöglicht es dir, automatisch neue Personen zu deinem Enterprise-Abo hinzuzufügen, die Möglichkeit für Personen in Unternehmen einschränken, separate Miro-Abos zu erstellen, und die Nutzeraktivität innerhalb deiner Domain zu überwachen.

Mit der Domainsteuerung kannst du eine Bereitstellungsregel für die Personen deines Unternehmens festlegen:

- Neu in deiner Domain registrierte Personen können Zugriff auf dein Abo anfordern
- Neu in deiner Domain registrierte Personen treten deinem Abo automatisch bei
- Neu in deiner Domain registrierte Personen treten deinem Abo automatisch bei und niemand in der Domain darf neue Miro-Teams einrichten

![Add-a-domain-Image1.png](../../../../../../docs/enterprise-administration/user-management/images/21017653288082_Add-a-domain-Image1.png)*Domainsteuerung in den Miro-Sicherheitseinstellungen*

## So funktioniert die Lizenzierung

Wenn Unternehmens-Admins neue Personen einladen, können sie – je nach Abo-Setup – eine Lizenz für die eingeladene Person auswählen.

Nutzer, die von Nicht-Admins eingeladen oder automatisch über JIT, SCIM oder die Domainsteuerung für dein Abo bereitgestellt werden, erhalten die*Standardlizenz*:

- **für Preispläne mit nicht flexiblem Lizenzmodell (Nicht-FLP):** Die Standardlizenz ist eine Volllizenz (wenn die Organisation nicht über ausreichende Volllizenzen verfügt, erhalten automatisch erfasste Nutzer eine [kostenlose eingeschränkte](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) Lizenz).
- **für Preispläne mit dem flexiblen Lizenzmodell (FLP):** Die Standardlizenz kann Free oder [kostenlose eingeschränkte](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) sein.

:::note
Erfahren Sie mehr über unsere [Enterprise-Lizenzmodelle](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md), [Lizenzverwaltung beim flexiblen Lizenzmodell](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md), wie Sie Lizenzzuweisungen und Upgrades mit der [Anfragenverwaltung](09-request-management-on-enterprise-plan.md) verwaltenund wie Sie die Lizenznutzung mit dem [Software-Asset-Management](../security-integrations/software-asset-management/01-software-asset-management-miro-enterprise.md) nachverfolgen können.
:::

## Häufige Fragen

Wenn die Domainsteuerung so eingestellt ist, dass neue Personen erfasst werden, funktioniert sie ähnlich wie JIT, indem Personen mit bestimmten Domains automatisch einem Standardteam innerhalb des Enterprise-Abos zugewiesen werden?

Ja, aber die Domainsteuerung erfordert nicht, dass SSO für den Enterprise-Preisplan konfiguriert wird. Sie funktioniert auch ohne SSO.

Können wir verhindern, dass automatisch bereitgestellte Nutzer eine Volllizenz erhalten, bis sie aktiv mit der Arbeit an einem Board beginnen?

Ja, dies ist mit dem [flexiblen Lizenzmodell](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md) möglich.

Kann ich mehrere Bereitstellungsoptionen für mein Enterprise-Abo einrichten?

Ja, du kannst mehrere Bereitstellungsoptionen gleichzeitig verwenden.
