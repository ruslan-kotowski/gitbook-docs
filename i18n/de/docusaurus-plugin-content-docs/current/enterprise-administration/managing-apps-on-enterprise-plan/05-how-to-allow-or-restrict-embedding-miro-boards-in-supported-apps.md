---
title: "So erlaubst oder beschr\xE4nkst du das Einbetten von Miro-Boards in unterst\xFC\
  tzte Apps"
article_id: 4405088016274
translation_id: 4405088016274
locale: de
sidebar_position: 5
created_at: '2021-08-13T05:51:25Z'
updated_at: '2025-11-25T16:06:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: live-embed
---

Miro verfügt über mehrere Integrationen, um ein Board einfach über externe Apps wie [Zoom](../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md), [Microsoft Teams](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md), [Jira](../../integrations-apps/atlassian/02-miro-for-jira-cloud.md), [Confluence](../../integrations-apps/atlassian/01-miro-for-confluence.md) und [andere zu teilen](https://miro.com/marketplace/category/embed-miro/).  Enterprise-Admins können das Einbetten von Boards in die unterstützten Apps zulassen oder einschränken.

> **Relevant für: Enterprise-Preisplan**

### Einbetten von Miro-Boards in unterstützte Apps

Wenn du ein Miro-Board in eine unterstützte App einbettest, kannst du den Zugriff auf das Board auch Personen ermöglichen, die kein Miro-Profil haben.

Das Teilen eines Boards in einer unterstützten App wirkt sich nicht auf deine Freigabeeinstellungen auf der Miro-Seite aus. Erfahre mehr über den Zugriff auf Boards, die in unterstützte Apps eingebettet sind/span>[.](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

![allow_restrict_embed_customize_embed.gif](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/21019705471122_allow_restrict_embed_customize_embed.gif)*Einbetten eines Miro-Boards mit eingeschränktem Zugriff*

### So beschränkst oder erlaubst du das Einbetten von Boards in unterstützte Apps

> **Verfügbar für: Unternehmens-Admins**

Unternehmens-Admins im Enterprise-Preisplan können die Möglichkeit konfigurieren, Miro-Boards in unterstützte Apps einzubetten**.**  Wenn diese Einstellung aktiviert ist, können Miro-Boards auch dann einbettet werden, wenn die öffentliche Freigabe in deiner Organisation oder in deinen Teams eingeschränkt ist/strong>.

So erlaubst bzw. beschränkst du die Freigabe für nicht angemeldete Personen in unterstützten Apps:

1. Gehe zu den **Organisationseinstellungen**.
2. Unter **Sicherheit** klickst du auf **Freigabe**.
3. Scrolle nach unten zum Abschnitt Inhalt und schalte das **Freigeben über Einbetten zulassen** ein/aus.

:::note
Erfahre mehr über [den Zugriff auf eingebettete Boards für Nutzer mit kostenlosen eingeschränkten Lizenzen](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
:::

![allow-embedding.pngFreigeben](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803639826_allow-embedding.png)
*über Einbetten im Enterprise-Preisplan*

Wenn du diese Einstellung deaktivierst, sind zuvor eingebettete Boards nicht mehr verfügbar. Neue Boards können weiterhin eingebettet werden, aber jede Person mit Besuchszugriff muss darauf zugreifen können.

Die Personen haben einen vollständigen Überblick über alle Apps, in die ein bestimmtes Board eingebettet wurde, mit der Möglichkeit, den Zugriff jederzeit zu widerrufen – alles über die Board-Freigabe-Einstellungen.  Erfahre mehr darüber, wie du den Zugriff auf Boards verwalten und widerrufen kannst/span>[.](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

### Können Boards, die in unterstützte Apps eingebettet sind, passwortgeschützt werden?

In den Unternehmens-Einstellungen haben Unternehmens-Admins die Möglichkeit, Passwörter für Miro-Boards zu verlangen, die über einen öffentlichen Link freigegeben sind.

Wenn du [ein Board über einen öffentlichen Link mit einem Passwort auf der Miro-Seite teilst](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), werden diese Einstellungen nicht in Boards widergespiegelt, die in unterstützten Apps eingebettet sind. Der Passwortschutz wird nicht erzwungen, wenn du ein Board in Microsoft Teams, Zoom/span>, [oder andere Apps einbettest.](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md)

Stattdessen stellen wir sicher, dass der Zugriff auf ein eingebettetes Board nur in der unterstützten App verfügbar ist und nicht außerhalb der App (z. B. in einem Webbrowser) bereitgestellt wird – es sei denn, das Board wird [auf der Miro-Seite geteilt](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).
