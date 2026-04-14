---
title: Billing groups
article_id: 6574185673874
sidebar_position: 1
created_at: '2022-07-12T12:53:45Z'
updated_at: '2026-02-19T10:50:00Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: billing-groups
availability:
  plans: enterprise
  roles: company_admin
---

Billing groups enable company admins to map users to internal budgets. Since each user can be assigned to only one group, admins can easily track the number of licenses used by each cost center. Admins can also set a soft quota on licenses available to each billing group. This simplifies processes like license true-ups, renewals, and chargebacks for teams.

## Billing group settings

Your billing group settings show a comprehensive overview of license usage. For example, details of all existing billing groups, including user count, the number each type of licenses, and if assigned, the [soft quota](02-billing-groups-soft-quotas.md) of licenses allotted per group. Use the search field to quickly find a specific billing group.

### Where to find your billing groups

To find your billing group settings go to **Company** **settings** > **Subscription** > **Billing groups.**

:::note
Users not assigned to a billing group are automatically placed in the default company billing group. You can see the number of assigned active users in the banner at the top of your Billing group settings.
:::

## How to create a billing group

1. Go to **Company** **settings** > **Subscription** > **Billing groups**.
2. Click **Create a billing group**.
3. Add the billing group name.
4. (Optional) To set a soft quota on licenses assigned to this billing group, select Add quota for Standard licenses or Add quota for Advanced licenses, and input a number.
   To learn more about soft quotas, see the FAQ at the end of this article.
5. To add new users to the billing group, you can [upload a CSV file](#how-to-assign-users-to-a-billing-group-via-csv-file) with the list of user email addresses, or [assign users](#how-to-assign-a-user-to-a-billing-group) later.
6. (Optional) Assign a contact for the billing group. The contact can be reached for information about license usage.
7. Click **Create billing group**.

## How to edit a billing group

You can edit a billing group name, set or update a soft quota, change the billing group contact, and add users to the billing group.

:::note
Adding users to a new billing group automatically transfers them from their previous group.
:::

1. Go to **Company settings** > **Subscription** > **Billing groups**.
2. Click the three dots next to a billing group and choose **Edit**.
3. Edit any of the billing group properties. To add users to the billing group, [upload a CSV file](#how-to-assign-users-to-a-billing-group-via-csv-file) with the list of user email addresses, or [assign users](#how-to-assign-a-user-to-a-billing-group) later .
4. Click **Save**.

## How to delete a billing group

1. Go to **Company** settings > **Subscription** > **Billing groups**.
2. Click the three dots next to a billing group and choose **Delete**.
3. Confirm the deletion.
4. All users that were in this billing group will be assigned back to the main account, and will no longer be a member of any billing group.

## How to assign a user to a billing group

A user can be a member of only one billing group within the organization.

1. Go to **Company** settings > **Active users**.
2. Click the three dots next to a user.
3. Choose **Change billing group**.
4. Select a billing group and click **Assign user**. The user will be added to the new billing group.

## How to bulk-assign users to a billing group

Assign multiple users to a billing group at once.

1. Go to **Company** settings > **Active users**.
2. Select users manually or apply filters and select up to 50 users at once.
3. Click **Bulk actions** and select **Assign billing group**.
4. Choose a group and click **Assign users**. If some users are already members of other billing groups, you’ll be able to deselect them or change their billing group assignment.

## How to check which users are in a billing group

Check who is in a billing group to manage user access and billing more effectively.

1. Go to **Company** settings > **Subscription** > **Billing groups**.
2. Click on a specific billing group to see the users assigned to it.

## How to remove a user from a billing group

If a user isn't assigned to a specific billing group or is removed from one, they automatically default to the company's standard account billing group.

1. Go to **Company** settings > **Active users**.
2. Click the three dots next to a user.
3. Choose **Change billing group**.
4. Select **Default account billing group**. The user will be removed from the billing group and will now sit in the overarching billing group for the company.

## How to assign users to a billing group via CSV file

Assign several users to a billing group by uploading a CSV file with user emails. If a user is already a part of another billing group, they’re moved to the newly assigned billing group.

:::note
Make sure your CSV file has only one column with the header ‘e-mail’. This column should include your list of emails to be added to the billing group. Check your CSV uses commas to separate the values. Information in additional columns will not be processed. Miro does not save the CSV files.
:::

1. Go to **Company** settings > **Subscription** > **Billing groups**.
2. Click the three dots next to a billing group and choose **Edit**.
3. Upload a CSV file with the list of user email addresses.
4. Click **Save**.

## How to assign users to a billing group via SCIM

Set up [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) to automatically allocate users to a billing group according to a cost center.

#### Step 1: Configure your Identity Provider (IdP)

Ensure your IdP is set up to add the cost center to Miro. See guides for:

- [Setting up automated provisioning with OKTA](../../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md)
- [Setting up automated provisioning with Azure AD](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)

#### Step 2: Assign cost centers to your billing group

Add one or more cost centers to a billing group. All present and future users from these cost centers will auto-join the billing group.

**How to add a cost center**

1. Open the [**Edit billing group**](#how-to-edit-a-billing-group) page.
2. Enter your cost center in the **Insert cost center** field.
3. Press **Enter** on your keyboard.
4. Add any additional cost centers as needed.
5. Click **Save**.

:::note
*Miro does not verify the cost center information you enter. Make sure you enter accurate information for cost center names. This field is not case-sensitive.*
:::

### Managed by SCIM badge

Users with an assigned cost center linked to a billing group, are labeled as **Managed by SCIM**. You'll see this badge next to the user name.

These users can’t be manually added to billing groups and can only be assigned a cost center through a SCIM update.

### Cost center and billing group guidelines

- A billing group may contain several cost centers, but a single cost center can link to just one billing group.
- To reassign a cost center, first you need to [remove the cost center from its current billing group](#how-to-remove-a-cost-center-from-a-billing-group).
- Users who are assigned to a billing group based on their cost center cannot be manually assigned to another billing group.
- Removing a cost center from your billing group will also remove all SCIM-provisioned users from that billing group.
- Non-SCIM-provisioned users may be manually assigned to any billing group.

### How to remove a cost center from a billing group

1. Open the [**Edit billing group**](#how-to-edit-a-billing-group) page.
2. Click the **X**next to the cost center you would like to remove.
3. Click **Save**.

## How to export billing group data

Company admins can export a CSV file with the list of users in **Company** settings > **Active users**. You can then use the billing groups attribute in the exported CSV spreadsheet to filter budgets.

## Frequently asked questions

What happens when my users change cost centers at the Identity Provider (IdP) side?

After a SCIM update:

- if this new cost center is assigned to a billing group, the user will be automatically moved to this new billing group.
- if this new cost center is not assigned to a billing group or the cost center was removed from the user in IdP, the user will be automatically moved to the default company billing group.

What happens to users who were manually assigned to a billing group after implementing SCIM for billing groups?

They are auto-assigned to a new billing group according to their cost center, while those without a matching or any cost center remain in their current billing group.

Why can’t I manually assign a user to billing groups anymore?

Users assigned to a billing group via their SCIM cost center cannot be manually moved to another group.

What happens if my IdP stops syncing the cost center attribute to Miro?

New users won’t auto-assign to a billing group without synced cost centers, but can be manually assigned until syncing resumes.

What is a billing group soft quota?

A soft quota enables you to optionally set a limit on Advanced , Standard, or Full (legacy) licenses available for a billing group.

When you create or edit a billing group, you can enable **Add quota for Standard licenses** or **Add quota for Advanced licenses** and input a number.

The soft quota appears, as the number you set and a progress bar that indicates consumption, at the top of the billing group overview.

To learn more about soft quotas, see [Billing Groups Soft Quotas](02-billing-groups-soft-quotas.md).
