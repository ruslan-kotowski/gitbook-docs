---
title: Lizenzverwaltung im Flexiblen Lizenzmodell (FLP)
article_id: 360018622159
translation_id: 360018622159
locale: de
sidebar_position: 5
created_at: '2020-12-29T10:44:01Z'
updated_at: '2026-02-23T18:22:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Relevant für: Enterprise-Preisplan'
---

Erfahre mehr über die Lizenzverwaltung im flexiblen Lizenzmodell (FLP), einschließlich der Optionen für die Lizenzverwaltung, die für neue Nutzer verfügbar sind, und wie du vorhandene Lizenzen umwandelst.

:::tip
Wenn du FLP noch nicht kennst, empfehlen wir, zuerst das [Flexible Lizenzmodell](03-flexible-licensing-program-flp.md) und [die Nutzerzugriffsebenen im Enterprise-Preisplan](../../user-management/11-user-access-levels-on-enterprise-plan.md) zu lesen, um zu verstehen, wie unsere Lizenzmodelle, Lizenztypen und Miro-Rollen miteinander funktionieren.
:::

## Lizenzen an neue Nutzer zuweisen

Mitglieder Gäste Besucher

Aufgrund der Standard-Lizenzeinstellungen deines Unternehmens wird neuen Mitgliedern entweder eine Free- oder eine kostenlose eingeschränkte Lizenz zugewiesen. Um eine Standard-Lizenz für neue Mitglieder in deinem Abo festzulegen, wende dich an deine Miro-Kontaktperson.

Neuen Mitgliedern wird die Standardlizenz zugewiesen:

- wenn von Mitgliedern ohne Adminrechte eingeladen
- automatisch über [Just-in-Time-Bereitstellung](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), [Domainsteuerung](../../canvas-25-admin-features/domain-control/01-domain-control.md) oder [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)

Unternehmens-Admins haben auch die Möglichkeit, eine Lizenz für eingeladene Mitglieder auszuwählen.

- Wähle **Free**, wenn du möchtest, dass Nutzer die Option haben zu bearbeiten (sie erhalten ein Upgrade auf eine Standard- oder vollständige (Legacy) Lizenz, sobald sie ein Board bearbeiten oder erstellen, zur Bearbeitung eines Boards eingeladen werden, Miteigentümerschaft für das Board erhalten oder Bearbeiterrechte in einem [Projekt](../../../using-miro/sharing-boards/16-projects.md) bekommen)
- Wähle **Free Restricted**, um das Mitglied ohne Bearbeitungsrechte einzuladen

Gäste, die zu einem Board eingeladen werden, erhalten immer eine **Free** Lizenz. Erfahre, wie du [Gäste mit einem Enterprise-Preisplan einlädst](../../../using-miro/sharing-boards/07-collaboration-with-guests.md).

[Besucher](../../../using-miro/sharing-boards/08-collaboration-with-visitors.md) von öffentlich freigegebenen Boards sind kostenlos und benötigen keine Lizenzen.

## So upgradest oder downgradest du Lizenzen

> **Verfügbar für:** Unternehmens-Admins

**Free**-Lizenzen werden automatisch auf eine Standard- oder Full (legacy)-Lizenz aktualisiert, sobald der Nutzer ein Board erstellt oder bearbeitet.

Eingeschränkt kostenfrei zu Standard oder Vollversion (veraltet)  Standard oder Vollversion (veraltet) zu Eingeschränkt kostenfrei Lizenzen im Bulk umwandeln

Kostenlose eingeschränkte Lizenzen können manuell von Unternehmens-Admins oder im Rahmen der [Enterprise-Workflow-Automatisierung](../enterprise-workflow-automation/01-enterprise-workflow-automation.md) auf eine Standard- oder Volllizenz upgegradet werden.

So aktualisierst du eine Eingeschränkte kostenlose Lizenz auf eine Volllizenz:

1. Öffne **Teams** oder gehe zu **Organisationseinstellungen** > **Nutzer** > **Alle Nutzer** > **Aktive Nutzer**.
2. Klicke auf das **Symbol mit den drei Punkten** (**...**) neben einem Nutzer mit einer kostenlosen eingeschränkten Lizenz.
3. Wähle **Ändern zu Standardmitglied** aus.

Volllizenzen können auf eine kostenlose eingeschränkte Lizenz heruntergestuft werden, wenn Unternehmens-Admins den Zugriff des Nutzers einschränken und zusätzliche Volllizenzen freigeben möchten.

Vollmitglieder können nicht auf eine kostenlose Lizenz herabgestuft werden, da kostenlose Lizenzen nur neuen Nutzern zugewiesen werden können.

So stufst du eine Volllizenz auf eine kostenlose eingeschränkte Lizenz herunter:

1. Öffne **Teams** oder öffne **Organisationseinstellungen** > **Nutzer** > **Alle Nutzer** >**Aktive Nutzer**.
2. Klicke auf das **Dreipunkt-Symbol** (**...**) neben einem vollen Nutzer.
3. Wähle **In kostenlose eingeschränkte Lizenz ändern**.

So konvertierst du mehrere Lizenzen auf einmal:

1. Öffne **Organisationseinstellungen** > **Nutzer** > **Alle Nutzer** > **Aktive Nutzer**.
2. Wähle alle Nutzer, deren Lizenzen du konvertieren möchtest, einzeln aus oder wende Filter an, um Nutzer auszuwählen. Du kannst bis zu 50 Nutzer auswählen.
3. Klicke auf **Massenaktionen** und wähle eine neue Lizenzoption aus.
