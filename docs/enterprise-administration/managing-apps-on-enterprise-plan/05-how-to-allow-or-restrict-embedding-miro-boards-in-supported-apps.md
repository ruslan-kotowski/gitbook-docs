---
title: How to allow or restrict embedding Miro boards in supported apps
article_id: 4405088016274
sidebar_position: 5
created_at: '2021-08-13T05:51:25Z'
updated_at: '2025-11-25T16:06:56Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: live-embed
availability:
  plans: '[Enterprise plan](../../plans-billing/miro-plans/04-enterprise-plan.md)'
---

Miro has several integrations that enable users to easily share a board across external apps like  [Zoom](../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md), [Microsoft Teams](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md), [Jira](../../integrations-apps/atlassian/02-miro-for-jira-cloud.md), [Confluence](../../integrations-apps/atlassian/01-miro-for-confluence.md), and [others](https://miro.com/marketplace/category/embed-miro/). Enterprise Admins can allow or restrict embedding boards within the supported apps.

### Embedding Miro boards in supported apps

When you embed a Miro board in a supported app, you can grant board access to the app’s users even if they don’t have Miro profiles.

Sharing a board inside a supported app doesn’t affect your sharing settings on the Miro side. Learn more about [Access to boards embedded in supported apps](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

![allow_restrict_embed_customize_embed.gif](images/21019705471122_allow_restrict_embed_customize_embed.gif)*Embedding a Miro board with restricted access*

### How to restrict or allow embedding boards in supported apps

> **Who can do it:** Company Admins

Company Admins on the Enterprise plan can configure the ability to embed Miro boards in supported apps**.** With this setting turned on, users can embed their Miro boards even if [public sharing is restricted in your organization or teams](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md#restrict-sharing-via-public-link).

To allow or restrict sharing with non-signed-in users in supported apps:

1. Go to **Organization** **settings**.
2. Under **Security**, click on **Sharing**.
3. Scroll down to the Content section and toggle on/off **Allow sharing via embed**.

:::note
Learn more about [embedded board access for users on Free Restricted licenses](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md#free-restricted-board-access).
:::

![allow-embedding.png](images/23921803639826_allow-embedding.png)
*Allowing sharing via embed on the Enterprise plan*

If you turn the setting off, previously embedded boards will become unavailable. New boards can still be embedded, but will require each visitor to have access.

Users have a full view of all of the apps where a specific board has been embedded with the ability to revoke access at any time — all from the board sharing settings. Learn more about how to [manage and revoke access to embedded boards](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

### Can boards embedded in supported apps be password protected?

In Company settings, Admins have the option to require passwords for Miro boards that are shared by a public link.

When you [share a board via a public link with a password on the Miro side](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md), these settings are not reflected in boards embedded across supported apps. Password protection is not enforced when you embed a board in [Microsoft Teams](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md), [Zoom](../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md), or other apps.

Instead, we ensure that access to an embedded board is only available in the supported app and not provided outside the app (for example, in a web browser) — unless the board is [shared on the Miro side](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).
