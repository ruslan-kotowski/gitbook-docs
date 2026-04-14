---
title: Jira Cards FAQ
article_id: 360013463739
sidebar_position: 17
created_at: '2020-04-23T20:04:11Z'
updated_at: '2026-03-20T14:10:12Z'
draft: false
---

This article answers the most popular questions regarding how our Jira Cards integration is built.

**Security**

**How does the Jira-Miro authentication work?**

See the Help Center articles for

- **Jira Server on-premise**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Third-party) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Data Center on-premise**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Third-party) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Cloud**
  Select from the Jira Cards settings page.
  - [OAuth 2.0](https://help.miro.com/hc/articles/8588617184402) (3LO)

**Is data secured in transit between Jira and Miro?**

We use the TLS security protocol. It encrypts HTTP messages before transmission and decrypts messages upon arrival. We also support mutual TLS for [Enterprise plan](https://help.miro.com/hc/articles/360017730433).

**Do you support mutual TLS?**

Yes, [learn more](https://help.miro.com/hc/articles/4410562720658).

**Will Miro retain any of the customer’s Jira data?**

Yes, Miro retains the card's data which are added to the board.

**How long is the retention period and how will the data be secured?**

For OAuth 1.0. (Jira Server or Data Center) also, the data are updated if the webhooks are configured during the Jira Cards plugin setup process. The retention period is unlimited. Only the general Miro security protocols are applied.

**Can we restrict the information that is retrieved from Miro?**

We did not find any mention in [Atlassian's documentation](https://developer.atlassian.com/server/jira/platform/webhooks/) of how to limit the information to just a few fields.

**Can we have a diagram showing the data flow between Jira and Miro?**

Detailed info can be found in [this Jira Developers article](https://developer.atlassian.com/server/jira/platform/oauth/). We implement our integration according to Atlassian documentation.

**How is the token handled?**

Oauth 1.0: Only the access token is used. The access token persists [for 5 years unless](https://developer.atlassian.com/server/jira/platform/oauth) revoked (no option to customize, as this policy is defined on the Atlassian side. You can revoke the token on the Jira side using web UI). Remember that each new token stops the integration from working and requires [reconnecting it](https://help.miro.com/hc/articles/360019501754#Step_2_-_Connection).

OAuth 2.0: Access token lasts for 1 hour. Refresh token lasts for 90 days (if you go 90 days without using the integration, you’ll have to re-authenticate).

**Is a single access token used for all of the customer’s Jira access?**

Every Miro user who intends to import, create or edit Jira Cards must connect their individual Jira credentials. All of the above actions can only be performed on behalf of individual Jira credentials.

**How are the request tokens, access tokens, private keys, and other OAuth secrets/credentials secured?**

During the integration, only access tokens are used. They are securely stored within the database and are used only on the server side.

For OAuth 1.0. (Jira Server and Data Center) the authToken is only used for the webhook. It is not the actual authentication token used by OAuth. Requests are sent over an encrypted connection. The secret key is auto-generated and is associated as per team.

**What endpoints does your integration use?**

```
POST /rest/api/2/issue - create new issue
```

```
PUT /rest/api/2/issue/id - update issue
```

```
GET /rest/api/2/user/picker?query=xx
```

```
GET /rest/api/2/myself
```

```
GET /rest/api/2/filter/favourite
```

```
GET /rest/api/2/issue/picker
```

```
GET /rest/api/2/serverInfo
```

```
GET /rest/api/2/issue/$key
```

```
GET /rest/api/2/issue/createmeta
```

```
GET /rest/api/2/issue/$key/editmeta
```

```
GET /rest/api/2/priority
```

```
GET /rest/api/2/issuetype
```

```
GET /rest/api/2/mypermissions
```

For OAuth 1.0. (Jira Server and Data Center) additionally, we use:

```
POST /rest/webhooks/1.0/webhook
```

**Will the cards work with Jira Datacenter?**

Yes. We are approved by Atlassian, and we already have a lot of customers successfully using Jira Cards with Datacenter. The installation procedure is the same.

**What IPs are you using to communicate to the Jira system?**

The list of our static IP addresses can be found [here](https://help.miro.com/hc/articles/360017572694).

Note that these are the addresses used only to communicate with the Jira system. Miro app's IPs are dynamic and to ensure that all the functionalities on the Miro boards (including some of those related to Jira cards) perform successfully, we ask to [add our domains to your allowlist](https://help.miro.com/hc/articles/360017572694).

**Can we integrate Jira with Miro, but block Jira issues with Security Level set to "Private"?**

No, that is not an option. Security Levels in Jira do not correlate with Miro.

**General**

**Can we connect Miro to Jira if we use a Jira server?**

Because Miro is an online tool, you can only connect to Jira when your instance is open to the public internet.

**Can we connect multiple Jira instances at the same time?**

Yes. However, keep in mind that connecting a Jira instance is about establishing the initial link, while an active connection refers to the linked instance currently in use. An active connection defines where Jira Cards get imported from when you open the Jira Cards app, and for which instance users are authorized. For a given user, there can be only one (1) active connection at a time. With OAuth 2.0, a user can edit any Jira Card associated with any linked instance for which they are already authenticated. For any other authentication protocol, an entire team shares an active instance, and can only import and interact with cards from that instance. You can define multiple organization-level settings and switch between active connections at the team level.

**What is the Server to Cloud migration process?**

Since your Jira Base URL will inevitably change during the migration to Cloud, the integration will break without changes on our end. Please [reach out to Miro](https://help.miro.com/hc/articles/360020185799) support for assistance.

**Will Miro create a webhook per team, per project, or per Miro instance?**

If you enable Automatic Webhook in your Miro settings, then webhook creation happens automatically. If you use team-level authorization with Jira, then Miro creates webhooks per team. If you use organization-level authorization, then Miro creates webhooks per organization.

**Does the Jira Cards plugin support Next-Gen projects?**

Yes, it does.

Please note that currently, there is no Epic link/field when creating a Jira Card for a Next-Gen project on Miro's side.

**Are custom Jira fields supported?**

Yes, we support almost all custom fields of *basic* types. If you have a *complex* data type field, it may not be supported and cause unexpected behaviour when updating or creating Jira cards on the board.

**What's going to happen with existing Jira Cards in case we switch to another Jira instance?**

Currently, when you move Jira issues from one Project to another in Jira, they no longer update on Miro's side.

As a workaround, we suggest you copy a Jira issue URL (Ctrl/Cmd+C) and paste it into a Miro board (Ctrl/Cmd+V). Thus, a Jira Card will show new values and will be updated automatically.

**If a board is moved to another Miro team, what will happen to Jira cards on the board?**

The Jira Cards will stay on the board, but no one will be able to modify them (even if the same Jira instance is configured for the target team).

When clicking a card, you will see a message: *"JIRA Card was imported from another account"*. If you want to make the cards editable, please import them to the board anew.

**Is there an additional cost for the Jira Cards integration?**

Jira Cards are available on all paid, and Education plans at no additional cost (Starter, Business, Education, and Enterprise plans).

**Can a user access all Jira Cards on the board?**

The permissions for the Jira Cards integration ensure that users can only create and edit cards in Jira projects that they have access to.

As all widgets on a Miro board are visible to everybody that has access to the board if somebody either doesn't have Jira credentials or doesn't have the right credentials, they will be able to view the collapsed Jira Card on a Miro board (with title and some other fields) but cannot expand the card to fully review it or modify it.

**Has Atlassian discontinued support for Jira Server?**

Yes, Atlassian has discontinued support for Jira Server as of February 2024.

**Does Miro Planner/Jira Cards support the Jira custom fields: Custom issue types, and Custom dependencies?**

Yes, both are supported. If the **Custom issue types** and **Custom dependencies** fields are set up in Jira, *and* Miro Planner is authenticated for that Jira instance, then these custom fields are available in the planner.

**Does Miro support OAuth 2.0 for Jira Data Center?**

Yes. See [Connect to Jira Data Center using OAuth 2.0.](https://help.miro.com/hc/articles/25753304280466)

**Jira Cards in Tables & Timelines**

**How can I import Jira issues to Tables and Timeline?**

You can drag and drop one or multiple Jira Cards directly into a Table or Timeline. This is currently the only way to do so.

**Which fields in the Table link to Jira?**

System Jira fields:

- Title
- Description
- End date (Due Date in Jira)
- Assignee (Beta)
- Status (Beta)

Custom Jira fields:

- Start date
- Estimate

**What fields in the Table do not sync to Jira?**

Click a cell to see which fields sync to Jira. Any field that syncs shows with a Jira logo. All other fields are stored in Miro only and do not sync to Jira.

**Why can’t I edit a field in Table or Timeline from the supported five Jira fields above?**

The field may not be present in the edit screen on Jira.

An easy check to know if the field is present in the edit screen or not:

On Miro, open the side panel for the Jira card. Check if the field is present in the side panel. If the field is not present, you must add the field to the edit screen on Jira.

There are some rare cases that the fields are editable on Jira, but not present in the edit screen on Jira. In this case, these fields cannot be edited on Miro.

Is the field you cannot edit **Start date** or **Estimate**? If so:

The field may not be present on Jira or missing from the edit screen (refer to previous point)

There may be a mapping issue for Start date or Estimate as these are custom Jira fields.

We map these fields according to this logic:

- **Start date**: We check for fields named: Start Date , StartDate, Target Start
- **Estimate**: We check fields named: Story Points, Story point estimate, Story Point, StoryPoints, StoryPoint
- If the Start date or Estimate field is not named as one of the following names above, this could explain why editing is not working.

**Why does editing the Start Date or Estimate in Miro Table or Timeline either not work or update the wrong field in Jira?**

We currently rely on automated mapping for the Start Date and Estimate fields in Jira. Since these are custom on Jira, there may be a case that multiple fields in your Jira configuration match the criteria mentioned above.

We select the first match according to the order of field names mentioned above:

For example, if a Jira ticket has both Story Points and Story point estimate fields, we match the first one according to the list above, which is Story Points. Therefore, any changes to the Estimate field in the table will update the Story Points field in Jira, not Story point estimate.

At the moment, there is no workaround for this. If you experience this issue, please send feedback to your support team so we can better understand your needs as we develop more advanced field mapping capabilities.

**Why can’t I import Jira cards from 2 different instances into a Table or Timeline?**

We currently only support one Jira instance per Table/Timeline. Once a Jira card is imported into a Table/Timeline, the Table/Timeline is linked to that specific Jira instance.

Even if all Jira records are deleted, the link to the original Jira instance remains. To import cards from a different Jira instance, you need to create a new Table/Timeline.

**Why can’t I see or edit the Status and Assignee fields for my Jira records in a Table or Timeline?**

Currently Jira Status and Assignee fields are not supported in Tables and Timeline. We have decided to disable these fields in Tables and Timeline to manage expectations, avoid confusion, and potential data loss. The Jira Status and Assignee fields and its contents exist, but it does not appear in Tables or Timeline.

You can still edit these fields directly in Jira cards using the side panel. Simply drag the row from the Table or Timeline onto the canvas to make your Jira card re-appear.

**More information:**

- [Jira Cards](https://help.miro.com/hc/articles/360017572434)
- [How to set up and to uninstall Jira Cards](https://help.miro.com/hc/articles/360019501754)
- [How to set up webHook for Jira Cards](https://help.miro.com/hc/articles/360017731113)
- [Possible issues with Jira Cards and Jira Add-on](https://help.miro.com/hc/articles/360017572654)
