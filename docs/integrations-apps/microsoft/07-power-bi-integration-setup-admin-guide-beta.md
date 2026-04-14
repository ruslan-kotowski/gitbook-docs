---
title: Power BI integration setup (admin guide) (BETA)
article_id: 18945328862994
sidebar_position: 8
created_at: '2024-05-15T12:57:57Z'
updated_at: '2025-11-25T15:42:21Z'
draft: true
availability:
  plans: Browser, Desktop App
  roles: company_admin
---

For organizations looking to integrate Microsoft Power BI with Miro, this guide provides step-by-step instructions on setting up the integration, enabling it for your team, and addressing security considerations.

Key features:

- Embed Power BI reports and dashboards into miro boards
- Specify charts to import into Miro boards
- Request updated Power BI content directly from Miro boards

:::tip
The Power BI integration is currently in private beta.
:::

### Technical implementation

Miro is integrated with Power BI through the [REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/) together with [Power BI embedded analytics Client APIs](https://learn.microsoft.com/en-us/javascript/api/overview/powerbi/). Users can easily link their Power BI reports or dashboards to Miro boards by authorizing Power BI access. For authentication, we use [OAuth2.0](https://learn.microsoft.com/en-us/entra/identity-platform/v2-protocols).

### Integration requirements

Ensure your subscription includes:

- Power BI Cloud
- Supported subscriptions:
  - Power BI Premium per capacity SKU
  - Fabric Capacity Reservation SKU

## Set up the Power BI integration

1. Log in to Microsoft Entra as an admin.
2. Navigate to **Enterprise applications** > **Consent and permissions** > **Admin consent settings**
3. Under **Admin consent requests**, set **Yes** for **Users can request admin consent to apps they are unable to consent to**.
4. In **Who can review admin consent requests**, select the necessary users, roles, and groups who will be allowed to review admin consent requests.
5. Users will then be able to ask for approval. To see the approval request screen, a non-admin user should paste a Power BI link to a Miro board on the Miro team enabled for Miro + Power BI integration testing.
6. The admins selected in Step 4 can navigate to the Admin consent requests screen and approve the pending request.
7. Once approved, the Miro + Power BI integration becomes allowed for any user to authorize on their own.
8. To check whether the integration works, paste a link to a Power BI dashboard or a report on a Miro board that belongs to a team you have enabled the integration for.
9. Click **Connect** to confirm authorization on the Power BI webpage.
10. A dialog will open asking you to select which charts to embed. Select a chart and click **Add chart**.
11. The charts will be added as images to your Miro board.

## How to turn off the Power BI integration

Admins can revoke permission by deleting the Miro app from Enterprise applications in Microsoft Entra.

1. Log in to Microsoft Entra.
2. Click on **Enterprise applications**  > **Consent and permissions**.
3. From the list of applications, locate and select **All applications**.
4. Find the **Contenthub Microsoft Power BI Integration** app from the list.
5. Click on the app to access its properties.
6. Within the application properties, click on **Delete**.

## Integration limitations

- Embedding on public boards is not possible.
- Embedding dataset links is not supported.
- Embedding links from the Share menu is not supported.

## Data retention

The embedded Power BI data follows Miro’s standard data retention policy applied to all customer data. Read our [Miro Data Processing Addendum](https://miro.com/legal/documents/Miro-Data-Processing-Addendum.pdf).

Different types of data from pasted Power BI links are fetched as image and stored in Miro:

- Images of tiles from Power BI Dashboards
- Images of visuals from Power BI Reports
- Titles of Power BI Dashboards, Reports, Visuals, and Tiles
- Page names from Power BI Reports
- Filter names and values from Power BI Reports

## Frequently asked questions

Why is the Power BI integration in Beta?

The Beta phase aims to gather feedback to enhance stability and user experience. Security remains a top priority.
