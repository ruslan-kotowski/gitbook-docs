---
title: "Kostenlose eingeschr\xE4nkte Lizenz"
article_id: 360011746739
translation_id: 360011746739
locale: de
sidebar_position: 4
created_at: '2020-02-05T07:29:16Z'
updated_at: '2026-02-19T10:40:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Wenn sich neue Nutzer einem Miro-Abo anschließen, kann ihnen je nach [Enterprise-Lizenzmodell](02-enterprise-licensing.md) eine kostenlose eingeschränkte Lizenz zugewiesen werden.

> **Relevant für:** Enterprise-Preisplan

## Wann wird Nutzern eine kostenlose eingeschränkte Lizenz zugewiesen

**Im flexiblen Lizenzmodell (FLP)** kann einem Nutzer die kostenlose eingeschränkte Lizenz zugewiesen werden, wenn:

- Die Standardlizenz für neue Nutzer ist auf kostenlose eingeschränkte Lizenz eingestellt
- Ein Unternehmens-Admin lädt den Nutzer ein und wählt im Einladungsfenster die kostenlose eingeschränkte Lizenz für ihn aus
- Ein Unternehmens-Admin stellt den Nutzer in **Unternehmenseinstellungen > Aktive Nutzer** auf kostenlose eingeschränkte Lizenz um

:::note
Erfahre mehr über das [flexible Lizenzmodell (FLP)](03-flexible-licensing-program-flp.md) und [die Verwaltung von Lizenzen im FLP](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

**Bei einer nicht flexiblen Lizenzierung (Non-FLP)** kann einem Nutzer die kostenlose eingeschränkte Lizenz zugewiesen werden, wenn:

- Der Nutzer wird bei der Registrierung von [Domainsteuerung](../../canvas-25-admin-features/domain-control/01-domain-control.md) oder [Just-in-Time-Bereitstellung](../../user-management/13-user-provisioning-on-enterprise-plan.md) in einer Organisation automatisch erfasst, die nicht über genügend Advanced-, Standard- oder Volllizenzen (Legacy) verfügt.
- Der Nutzer wird in ein Team in der Organisation eingeladen, das nicht über genügend Advanced-, Standard- oder Volllizenzen (Legacy) verfügt.

Wenn mehrere Nutzer gleichzeitig eingeladen werden, erhalten sie Lizenzen in der Reihenfolge ihrer E-Mail-Adressen in der Liste der Eingeladenen. Wenn die Organisation nicht genügend Lizenzen hat, erhalten die Nutzer am Ende der Liste eine kostenlose eingeschränkte Lizenz. In diesem Fall erhält der Einladende eine Pop-up-Benachrichtigung über einen begrenzten Zugriff für einige Nutzer.

## So funktionieren kostenlose eingeschränkte Lizenzen für Nutzer

Nutzer mit einer kostenlosen eingeschränkten Lizenz können Boards in den Teams, in denen sie aktiv sind, ansehen und kommentieren. Sie können Bearbeitungsrechte sowie eine Standard- oder Volllizenz von Unternehmens-Admins anfordern. Sie können zudem Teams in der Organisation entdecken und diesen zusammen mit anderen Mitgliedern beitreten.

:::note
Unternehmens-Admins können [die Einstellungen für die Anfragenverwaltung konfigurieren](../../user-management/09-request-management-on-enterprise-plan.md).
:::

### Board-Zugriff mit einer kostenlosen eingeschränkten Lizenz

Die folgenden Zugriffsberechtigungen zum Ansehen, Kommentieren oder Bearbeiten gelten für Nutzer mit einer kostenlosen eingeschränkten Lizenz:

|  |  |
| --- | --- |
| **So wurde das Board freigegeben** | **Zugriffsebene** |
| Öffentlicher Link | Personen mit einer eingeschränkten kostenlosen Lizenz können je nach gewährter Zugriffsebene Boards ansehen und/oder bearbeiten. |
| Team- oder Unternehmenslink | Personen mit einer eingeschränkten kostenlosen Lizenz können je nach gewährter Zugriffsebene Boards ansehen und/oder kommentieren. |
| [Eingebetteter Link](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md) | Personen mit einer eingeschränkten kostenlosen Lizenz können je nach gewährter Zugriffsebene Boards ansehen und/oder kommentieren.  Personen mit einer eingeschränkten kostenlosen Lizenz können keine Boards bearbeiten und auch keinen Bearbeitungszugriff anfordern, selbst wenn der Bearbeitungszugriff über die Einbettungsberechtigungen gewährt wird. |

## So verwaltest du eingeschränkte kostenlose Lizenzen

> **Verfügbar für:** Unternehmens-Admins

Bei allen Abos können Unternehmens-Admins eine eingeschränkte kostenlose Lizenz im Abschnitt **Aktive Nutzer** in den Team- oder Unternehmenseinstellungen auf eine Standard- oder Volllizenz upgraden.

**Flexibles Lizenzmodell (FLP)**

Bei FLP-Abos können Unternehmens-Admins eine erweiterte, Standard- oder Volllizenz auch jederzeit auf eine kostenlose eingeschränkte Lizenz downgraden.

Wenn ein Nutzer mit einer kostenlosen eingeschränkten Lizenz Bearbeitungszugriff anfordert, erhalten Unternehmens-Admins die Anfrage entsprechend ihrer [Einstellungen der Anfragenverwaltung](../../user-management/09-request-management-on-enterprise-plan.md).

:::note
Erfahre mehr über die [Lizenzverwaltung im flexiblen Lizenzmodell](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

## Häufige Fragen

**Was passiert mit meinen eingeschränkten kostenlosen Lizenzen, wenn ich meinem Nicht-FLP-Preisplan weitere Standard- oder Volllizenzen hinzufüge?**

Deine bestehenden Nutzer der eingeschränkten kostenlosen Lizenz werden nicht automatisch auf die neuen Standard- oder Volllizenzen aktualisiert. Unternehmens-Admins können Lizenzen manuell upgraden.
