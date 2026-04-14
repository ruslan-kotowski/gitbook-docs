---
title: Manage team privacy and discovery on Enterprise Plan
article_id: 360011821219
sidebar_position: 12
created_at: '2020-02-07T12:46:14Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
availability:
  plans: enterprise
  roles: company_admin
---

Working in a large organization often means that content and users are distributed across multiple teams. Ensure everybody has access to what they need by allowing members of your subscription to see and join relevant teams.

### Team discovery

**Team discovery** is a team-level setting that controls how members of the organization can find and join the team. To manage discovery settings for a team, go to the **Company settings > Teams** and then click on the Team you want to change the settings for. Then select the **Settings** tab.

![team-management-list.png](images/23921803038994_team-management-list.png) *Teams list within company settings*

:::warning
Team discovery can be set up by Company Admins and Team Admins [if the Team Admins are allowed to invite users to the team](../../administration/user-management/02-invitation-settings.md) (they will also receive user requests to join the team).
:::

Team discovery has three states:

- **Hidden** — unless members are invited to the team, they can’t find it
- **Members can join after approval** — the team is visible and members can request to join
- **Open to members** — the team is visible and members can join it right away

If a team has [domain allowlist restrictions](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md#restrict-sharing-outside-the-allowed-domains), only users whose email domains are on the team’s allowlist will be able to discover and request to join the team. This setting ensures that team discoverability follows the domain restrictions set at the team level.

:::tip
Enable our Team Discovery feature along with [Just-in-Time provisioning](../user-management/13-user-provisioning-on-enterprise-plan.md)), and the default team you set for newly registered users will also be visible for existing users to join.
:::

![team-management-discovery-settings.png](images/23921780537234_team-management-discovery-settings.png)
*Team discovery settings*

Team discovery doesn’t affect the way members see other users in your subscription. So, unless it is overruled by Team privacy, members can see the complete list of other users in settings.

Members of your Enterprise plan will be able to find teams that they can join by opening the Teams menu in the upper left of the Dashboard and the selecting ![icon-zoom-in.svg](images/23921803048338_icon-zoom-in.svg) **Join team**. A list of teams will appear with the option to **Join** or **Ask to Join**, depending on the individual team's security settings.

![team-management-join.png](images/23921780544914_team-management-join.png) *List of discoverable teams*

### Team privacy

**Team privacy** is a company-level functionality that sets the visibility of both teams and users. It is found in the **Company** settings > **Security** > **Sharing,** in the **Team Privacy** section.

![team-management-privacy.png](images/23921780547218_team-management-privacy.png)
*Team privacy settings*

- When Team privacy is disabled, members of the subscription can see the complete list of users in settings and the list of discoverable teams. It is the default state for the Enterprise plan subscriptions to ensure that all members can find relevant content and collaborate with other users to foster knowledge sharing, transparency and reduce duplication of work
- When enabled, Team privacy allows members of the subscription to only see teams to which they are invited to and other users in these teams only. It can be used when working with different clients in separate teams to ensure that they don’t learn about each other. With Team privacy enabled it is not possible to [share boards with the entire company in one click](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#sharing-a-board-with-the-entire-company).

### Team privacy and Team discovery working together

Team privacy has a higher priority than discovery set up on the team level. You'll see a notification that team discovery settings are not effective. You can still manage its options, which will take effect once Team privacy is disabled.

:::note
Both Team privacy and Team discovery settings affect the experience of members inside the subscription and have no impact on how a user can [join the subscription itself](../user-management/13-user-provisioning-on-enterprise-plan.md).
:::
