---
title: Einladungseinstellungen im Enterprise-Preisplan
article_id: 4412315533842
translation_id: 4412315533842
locale: de
sidebar_position: 3
created_at: '2021-12-13T04:56:26Z'
updated_at: '2026-02-19T10:56:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

Konfiguriere die Einstellungen für die Einladungen zum Enterprise-Preisplan, um festzulegen, wer neue Nutzer zu deinem Preisplan einladen kann. Du kannst deine Einladungseinstellungen an die Anforderungen deiner Teams und des gesamten Unternehmens anpassen.

> **Verfügbar für:** Enterprise-Preisplan
> **Wer kann es machen:** Unternehmens-Admins

:::tip
Wenn du neu bei Miro bist, erfahre mehr über [Team- und Unternehmenseinstellungen](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md).
:::

## Einstellungen zur Einladung ins Team

Für eine reibungslosere Zusammenarbeit kannst du allen **Teammitgliedern** erlauben, neue Mitglieder ins Team einzuladen. Wenn du mehr Kontrolle über Team-Einladungen wünschst, kannst du diese Option auf Unternehmens- und/oder Team-Admins beschränken, sodass alle Einladungsanfragen über die [Anfragenverwaltung](09-request-management-on-enterprise-plan.md) gesendet werden. Du kannst auch steuern, ob Nutzer [Gäste](../../using-miro/sharing-boards/07-collaboration-with-guests.md) in Teams einladen können.

### So konfigurierst du die Einstellungen für Team-Einladungen

Um deine Team-Einladungseinstellungen zu verwalten, gehe in der Admin-Konsole zu **Teams** und wähle dein Team aus. Dein Team-Feld wird geöffnet. Unter **Einladung** wähle eine der folgenden Optionen:

- **Nur Unternehmens-Admins**
  Nur Unternehmens-Admins können neue Mitglieder zum Team hinzufügen.
- **Unternehmens-Admins und Team-Admins**
  Unternehmens-Admins und Team-Admins können neue Mitglieder zum Team einladen.
- **Alle Teammitglieder**
  Alle Teammitglieder können neue Mitglieder zum Team einladen.

:::note
Bei [Abos mit flexiblem Lizenzmodell (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) werden die Teameinladungseinstellungen durch Einladungseinstellungen des Unternehmens ergänzt.
:::

### So konfigurierst du Gast-Einladungen

Unternehmens-Admins können die Option für Mitglieder, [Gäste](../../using-miro/sharing-boards/07-collaboration-with-guests.md) einzuladen, erlauben oder einschränken. Gäste können nur auf Boards zugreifen, zu denen sie eingeladen wurden, und benötigen keine Lizenz.

Aktualisiere die Einladungseinstellungen für Gäste in **Teams** > wähle dein Team > **Einstellungen** > **Gäste für das Team [Name] erlauben.**

:::note
Unternehmens-Admins können die automatische Deaktivierung von Gästen nach 30 Tagen Inaktivität ermöglichen.
:::

## Szenarien für Einladungen

:::tip
Je nach den [Einstellungen für die Anfragenverwaltung](09-request-management-on-enterprise-plan.md) können Anfragen zur Freigabe eines Boards oder zur Einladung eines Nutzers zu einem Team entweder direkt an Unternehmens-Admins, bestimmte Personen per E-Mail gesendet werden, oder es wird ein Service-Desk-Ticket erstellt.
:::

**Neue Mitglieder zu einem Team einladen**

Wenn Gäste nicht erlaubt sind und Mitglieder keine neuen Mitglieder einladen dürfen, sehen sie beim Versuch, ein Board zu teilen, die folgende Benachrichtigung und müssen eine Anfrage stellen.

**Eigentümer- oder Miteigentümerrolle gewähren**

Wenn Mitglieder keine neuen Mitglieder einladen dürfen und versuchen, einem Gast oder einem [Free Restricted](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) Mitglied in einem bestimmten Board die Eigentümer- oder Miteigentümerrolle zuzuweisen, sehen sie die folgende Benachrichtigung und müssen eine Anfrage stellen.

**Einladen einer externen Person oder eines Gastes zum Bearbeiten eines Boards**

:::note
Externe Gäste sind Gäste außerhalb deiner Unternehmensdomain. Sie haben eine externe Unternehmens-E-Mail-Adresse.
:::

Wenn Mitglieder keine neuen Mitglieder zum Team einladen dürfen und Gäste mit Bearbeitungszugriff nicht für das Team aktiviert wurden, sehen Nutzer beim Versuch, eine externe Person zum Bearbeiten eines Boards einzuladen, die folgende Benachrichtigung und müssen eine Anfrage stellen. Nach dem Absenden der Anfrage wird die eingeladene Person mit Kommentarzugriff zum Board hinzugefügt, sodass sie Kommentare auf dem Board hinzufügen kann, aber nicht den Inhalt bearbeiten kann.

## Einladungseinstellungen des Unternehmens

Die Einstellungen für Unternehmenseinladungen legen fest, wer neue Mitglieder zu deinem Enterprise-Abo einladen kann. Alle neuen Mitglieder erhalten je nach deinem [Lizenzmodell](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md) und der [Standardlizenz](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md) eine Advanced-, Standard-, Full- (veraltet), Free- oder Free Restricted-Lizenz.

### So konfigurierst du die Einstellungen für Unternehmenseinladungen

> **Verfügbar für**: [flexibles Lizenzmodell (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)

Um deine Einladungseinstellungen für das Unternehmen zu verwalten, gehe zu den **Unternehmens**-Einstellungen > **Sicherheit** > **Teilen** > **Einladung** und wähle eine der folgenden Optionen:

**Nur Unternehmens-Admins**
Nur Unternehmens-Admins können neuen Mitgliedern Lizenzen gewähren. Team-Admins und Mitglieder können nur bestehende Mitglieder aus dem Unternehmen zu ihren Teams einladen und keine neuen Lizenzen aktivieren.

**Unternehmens-Admins und Team-Admins**
Unternehmens-Admins und Team-Admins können neue Mitglieder einladen und neue Lizenzen hinzufügen. Team-Admins können neue Mitglieder nur zu den Teams einladen, in denen sie Team-Admin sind.

**Alle Mitglieder**
Jedes Mitglied des Enterprise-Abos kann neue Lizenzen hinzufügen, indem es Personen zu seinem Team einlädt, solange Einladungen für **Alle Teammitglieder** in den Einstellungen für Team-Einladungen erlaubt sind.

## Das Zusammenspiel von Unternehmens- und Teameinstellungen

Die Unternehmenseinstellungen ergänzen die Einstellungen für Teameinladungen. Unternehmens-Admins können in den Teameinstellungen festlegen, wer Personen zu einem bestimmten Team einladen kann. Dies bedeutet, dass Unternehmens-Admins Mitgliedern und Team-Admins erlauben können, ihre eigenen Team-Einladungen und die Zusammenarbeit zu verwalten, wobei die Lizenzen jedoch in den Unternehmenseinstellungen weiterhin von den Unternehmens-Admins gesteuert werden.

## Automatische Deaktivierung von Gästen

Richte die automatische Deaktivierung von Gästen nach 30 Tagen Inaktivität ein. Verwende diese Funktion, um Gäste zu entfernen und dein Abo zu schützen.

Wenn die Funktion aktiviert ist, werden Gäste (unabhängig von ihrer Domain), die in den vergangenen 30 Tagen in deinen Enterprise-Teams nicht aktiv waren, automatisch deaktiviert. Die 30-Tage-Frist kann nicht verändert werden.

Diese Einstellung wird für alle Teams innerhalb der Organisation angewendet.

Gehe zu deinen **Unternehmens**-Einstellungen > **Sicherheit** > **Freigabe** und aktiviere **Gäste automatisch deaktivieren**.

:::tip
Sobald die Einstellung aktiviert ist, wird die Aktion in den [Audit-Protokollen](../security-integrations/security-management/01-audit-logs.md) als **Einstellung für das Verfallen externer Nutzer aktiviert/deaktiviert** aufgezeichnet. Auch Deaktivierungsereignisse werden in den [Audit-Protokollen](../security-integrations/security-management/01-audit-logs.md). Der Akteur wird als **Miro Automation** angezeigt.
:::
