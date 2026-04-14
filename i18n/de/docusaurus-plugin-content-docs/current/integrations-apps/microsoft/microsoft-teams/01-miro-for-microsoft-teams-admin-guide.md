---
title: Miro für Microsoft Teams (Admin-Anleitung)
article_id: 4406387610002
translation_id: 4406387610002
locale: de
sidebar_position: 1
created_at: '2021-09-09T10:28:14Z'
updated_at: '2025-11-25T16:07:14Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
availability:
  notes: 'Erhältlich für: Free-, Starter-, Business-, Education- und Enterprise-Preispläne
    sowie alle Microsoft 365-Preispläne'
---

:::note
Die Einstellungen für die Erlaubnis und den Zugriff variieren je nach Art des Preisplans. Weitere Informationen zu externen Nutzern in Microsoft Teams findest du in [der Richtlinie für Apps von Microsoft](https://learn.microsoft.com/microsoftteams/apps-external-users).
:::

Aktiviere die Miro-Integration für Microsoft Teams, um die Zusammenarbeit innerhalb deines Unternehmens zu beschleunigen. Miro für Microsoft Teams bietet eine Reihe von Möglichkeiten, die es Nutzern ermöglichen, Echtzeit-Benachrichtigungen zu erhalten und auf eingebetteten Miro-Boards in Teams-Meetings, -Kanälen, -Chats und -Kalendereinladungen zusammenzuarbeiten.

Miro unterstützt außerdem adaptive Karten durch das Aufklappen von Links und die Erweiterung von Suchmeldungen, was Nutzern mehr Kontext auf freigegebenen Boards bietet und eine schnelle Zugriffsverwaltung auf Boards ermöglicht - und das alles, ohne den Bereich von Microsoft Teams zu verlassen.

:::tip
Erfahre mehr über die [Integration](..) von Miro [in Microsoft Teams](..).
:::

{
 *Miro für Microsoft-Teams*

## App-Verwaltung

:::warning
Microsoft-Admins müssen die Miro-Integration für Microsoft Teams im Katalog der App-Verwaltung von Microsoft aktivieren. Miro Enterprise Admins müssen die Integration auch über das Feld für die App-Verwaltung von Miro aktivieren.
:::

### App-Verwaltung in Microsoft Teams

Die Einstellungen können je nach Konto variieren. Erfahre mehr darüber, [wie du Apps in Microsoft Teams verwalten kannst](https://learn.microsoft.com/microsoftteams/manage-apps).

Um sicherzustellen, dass dein Unternehmen den größtmöglichen Nutzen aus der Integration zieht, solltest du die Miro App mit Hilfe [der Richtlinien zur Einrichtung von Apps von Microsoft](https://learn.microsoft.com/microsoftteams/teams-app-setup-policies) installieren und anheften.

### App-Verwaltung in Miro

In den Einstellungen deines Miro-Unternehmens > **Apps** siehst du zwei Microsoft Teams Apps:

- Miro für Microsoft Teams (Tab Integration) - Miro in Kalender, Teams-Meetings, -Kanäle und -Chats einbetten
- Microsoft Teams (Bot-Integration) - Nutzer-Benachrichtigungen

Wenn du Microsoft Teams (Bot-Integration) deaktivierst, erhalten Personen keine Miro-Benachrichtigungen mehr in Microsoft Teams.

![Microsoft-Teams-Bot-Tab-Apps.png](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21017606037010_Microsoft-Teams-Bot-Tab-Apps.png)*Microsoft Teams Apps*

## Zugriffseinstellungen für die gemeinsame Nutzung von Boards verstehen

Wenn du ein Board als Tab in Meetings, Kalendereinladungen, Chats und Kanälen hinzufügst, können Nutzer die entsprechenden Freigabeberechtigungen festlegen. Um ein Board als Tab in Microsoft Teams hinzuzufügen, besuche Hinzufügen von Miro als Tab in Microsoft Teams. Erfahre mehr über die [Zugriffseinstellungen für ein eingebettetes Board](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

### Zugriffseinstellungen für dein Board konfigurieren

Die Option Zugriffseinstellungen folgt organisationsweiten Zugriffskontrollen.  Wenn du die Freigabe von Board-Einbettungen im Enterprise-Preisplan eingeschränkt hast, ist diese Option für die Personen nicht verfügbar. Weitere Informationen findest du unter [Verwalten der Richtlinien zur Freigabe von Integrationen in Unternehmen.](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)

![publi__editing_is_turned_off.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21017593055506_publi%D1%81%20editing%20is%20turned%20off.jpg)*Beispiel für das Ausschalten der öffentlichen Bearbeitung durch den Unternehmens-Admin*
