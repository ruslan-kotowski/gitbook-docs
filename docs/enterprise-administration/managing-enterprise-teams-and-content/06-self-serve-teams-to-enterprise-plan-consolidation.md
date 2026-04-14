---
title: Self-serve teams to Enterprise plan consolidation
article_id: 9951494429970
sidebar_position: 7
created_at: '2023-02-06T09:56:12Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  roles: company_admin
  notes: 'Relevant for: Enterprise Plan'
---

The team consolidation feature allows you, as a Company Admin, to bring all teams created from your domains into your Enterprise plan. This ensures enhanced security, collaboration, and streamlined management by unifying all teams in one place.

Learn about the process, and read essential information about what happens before, during and after consolidation.

## Consolidating your teams

Miro provides Enterprise Plan customers the option to move any self-serve and free teams owned by their domain to their Enterprise account. Teams will be consolidated as they are, including:

- All boards (in their current state at the time of consolidation)
- All users, their roles and access rights
- Spaces structure
- Templates
- Apps (if allowed in the target Enterprise company settings)

:::note
- Teams consolidation is included at no additional cost for customers on the Enterprise Plan.
For complex consolidations that involve planning, coordination, option discovery, or validation, please contact your account team.
- While the Teams Consolidation feature addresses most standard use cases, custom or unique scenarios may require review by our experts.
:::

### Benefits of consolidating teams

- Take ownership of boards created within teams outside of your organization.
- Ensure utmost security by consolidating usage and content to be governed by your Enterprise security settings.
- Allow your users to collaborate more effectively and take advantage of Enterprise features
- Minimal user impact as the team structure stays intact. Uses can collaborate as they did before, but now with additional Enterprise Plan features.

## How to consolidate your teams into your Enterprise plan

The following step-by-step instructions explain how the new method for consolidating teams works.

**Procedure**

Follow these steps:

### **Step 1: Verify and configure your domain**

1. If your domain is not verified, you'll see a prompt to verify your domain. Additionally, you'll be provided with an estimated number of teams, users, and boards that are currently outside the domain.
   Verify your domain to enable team consolidation.
2. (Optional) Configure your domain by enabling the **Block users from creating new subscriptions** setting to prevent team creation outside of your Enterprise plan.
3. Once your domain is verified, the system will display the exact number of teams, estimated number of users, and boards outside your Enterprise plan, calculated based on your verified domains.

### **Step 2: Select teams for consolidation**

1. Start new consolidations by clicking the **Review teams** button on your **Managed domains** page.
2. The data collection process can take up to 20 minutes, during which you may close the page. Your results will be saved automatically.
3. After loading, you’ll see a detailed list for each team, including:
   1. Plan Type
   2. Number of Users
   3. Number of Boards
   4. Team Owners
4. Select which teams you would like to consolidate into your Enterprise plan, then click **Next**.

### **Step 3: Review the summary**

1. A summary page will display the selected teams for consolidation.
2. Review the estimated total number of teams, users, and boards that will be consolidated.
3. Submit your consolidation request by clicking **Submit request** once you’re satisfied. Please note consolidation will not happen immediately. **The Miro support team will contact you with the details.**

### **Step 4: Track consolidation progress**

After submitting your request, on your **Managed domains** page, you’ll see a Consolidation progress bar tracking the status.

**Request Submitted:** the Miro Support team received your consolidation request.

**Details confirmed:** you received the consolidation pre-check reports and confirmed the consolidation execution date and time with Miro Support.

**Consolidation started:** team consolidation started per the agreed date and time.

**Teams moved: t**he Miro Support team will share the results of the team consolidation with you and you will see the record in the audit logs.

### **Step 5: Pre-check results and scheduling**

1. As soon as the date and time are confirmed, the **Miro Team** will inform **Team owners** about the upcoming consolidation by email.
2. The **Miro Support Team** will share the results of the consolidation with you.

You have successfully consolidated teams into your Enterprise plan.

### Best practices for selecting teams

To ensure a smooth consolidation process, consider the following tips when selecting teams for consolidation:

- **Prioritize security**: Focus on teams that manage critical company data to ensure they are securely brought under the Enterprise plan.
- **Collaborative value**: Select teams with high levels of activity by reviewing the **number of users** and **boards**. Teams with more users and boards often contribute more to overall collaboration.

## During consolidation

During the migration, the team’s boards will be temporarily unavailable. An in-product notification banner will inform team members that the team is being migrated and they should try again later.

The consolidation time will vary based on the number of teams, users, and boards involved and can range from a few minutes to several hours. Following the consolidation, the Miro team will send a confirmation that the consolidation has been successfully completed and provide a post-consolidation report detailing the process and any necessary changes or updates. This ensures that you are fully informed about the consolidation's outcome and any necessary next steps.

## After consolidation

1. After the consolidation is complete, you will receive confirmation and a post-consolidation report from the Miro team.  The newly added Enterprise users will also receive an email.
2. Review the post consolidation report and validate that the teams were consolidated.
3. If you are using SSO, validate that consolidated corporate domain users are able to login via SSO based on Active Directory. The newly added Enterprise users will also receive an email after the consolidation is complete.
4. Update [team permissions](10-team-permissions-on-enterprise-plan.md) if needed (default team settings are applied to the team post-consolidation). If you have a large number of teams, you can update their settings using the [Update team settings API](https://developers.miro.com/reference/enterprise-dataclassification-team-settings-set). If you need assistance with the API, please reach out to [Miro support](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).

**For Company Admins**

- Company Admins will see the newly added teams within their Enterprise account under [**Teams**](07-team-management-on-enterprise-plan.md).
- All newly added users will appear under [**Users**](../user-management/12-user-management-overview-on-enterprise-plan.md#active-users-section).
- We recommend that company admins inform their team admins of any changes to [team permissions](10-team-permissions-on-enterprise-plan.md).

**For end users**

- Users may experience a change in the login flow if SSO is enabled.
- Users will see their team(s) appear with a house icon, indicating it is now part of the Enterprise account.
- Users will have access to all [Enterprise Plan features.](../../plans-billing/miro-plans/02-plans-and-features-available.md)

## FAQ

**What prerequisite are there to run the consolidation?**

To run the consolidation, domains must be verified.

**What happens if you don't have FLP and are bringing over licenses without enough Full licenses available?**

The most active users will be given Full licenses, while other users will be given Free Restricted licenses.

**Will existing Enterprise users participating in consolidation change their role license after the consolidation?**

Existing users are not changed until they are board owners, co-owners, or editors. Free internal users are converted to Full licenses while Free Restricted users will stay the same.

**How will Miro communicate to users who participate in the consolidation?**

- Emails will be sent to the creators of all Teams being consolidated before the consolidation.
- The newly added Enterprise users will also receive an email after the consolidation is complete.

**Will deactivated users become active after consolidation?**

Users active/deactive state will not change during consolidation; deactivated users will remain deactivated.

**How can I delete empty teams that have no boards and are created outside my Enterprise?**

We recommend requesting the consolidation of these teams. Once consolidated, you can easily delete them from within your Enterprise instance.
