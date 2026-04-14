---
title: Manage team signup mode
article_id: 360017730073
sidebar_position: 2
created_at: '2019-02-11T10:08:39Z'
updated_at: '2025-06-23T13:26:46Z'
draft: false
availability:
  plans: free, starter, business, education
  roles: team_admin, company_admin
---

Specify how users can join a team in your organization. For example, you can set team membership as invitation only, make all teams joinable for all users in a domain, or require users to request to join.

:::note
On Free, Starter, and Education plans, the Team admin specifies the team signup mode. On Enterprise, the Company admin specifies the team signup mode.
:::

![team-signup-mode.png](images/25008758551186_team-signup-mode.png)

*Team signup mode in Admin console*

1. From your Miro dashboard, select your avatar in the top-right, and select **Admin console**.
2. Go to **Security > Permissions**.
3. Under **Team signup mode**, select one of the following options:
   - **Invitation only**
     New members must be invited to join a team in your organization.
   - **Discoverable and open to anyone with a certain domain**
     New members can join any team inside your verified domain. To verify, enter your email domain, and click **Add**. A modal opens. Enter your domain email address, and click **Send verification**. Check your email, and in the verification email click **Verify domain**.
     > ✏️ If the domain you add is the same as your Miro account email, then your domain is verified automatically, and no confirmation is sent.

- **Discoverable, but open only after admin's approval**
  New members can find teams and must request to join. Team admin or Company admin can approve team membership requests. When a new member requests to join a team, admins receive an email notification. Follow the prompts in the email to approve the request.
  ![request_to_join_a_team.jpg](images/21019704701714_request%20to%20join%20a%20team.jpg)*Email notification for admins to approve a team membership request*

**More information:**

- [Invite users](../user-management/01-invite-users.md)
- [Board access rights](../../using-miro/sharing-boards/01-board-access-rights.md)
- [Manage team privacy and discovery on Enterprise Plan](../../enterprise-administration/managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
