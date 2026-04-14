---
title: Microsoft Power BI (user guide) (BETA)
article_id: 18945202296210
sidebar_position: 6
created_at: '2024-05-15T12:52:10Z'
updated_at: '2024-11-07T13:30:25Z'
draft: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
availability:
  plans: Browser, Desktop App
---

Combine the collaborative strength of Miro with the analytical power of Power BI. With Power BI reports and dashboards embedded directly into Miro boards, your team can streamline decision-making processes, visualize data-driven strategies, and drive project progress with clarity and precision.

- Utilize embedded Power BI data for real-time insights and informed decision-making.
- Collaborate effectively with team members by updating and adding charts to Miro boards containing Power BI data.

## How to embed Microsoft Power BI reports in Miro

:::tip
Confirm with your Company Admin that the Power BI integration has been set up for your organization.
:::

1. Navigate to Microsoft Power BI and copy the link of the report or dashboard from the browser address bar (not from the Share menu, as it's currently unsupported).
2. Paste the copied link on any Miro board.
3. Click **Connect** to authorize the Miro app in Microsoft Power BI.
4. After connecting, a dialog will open asking you to select which charts to embed. Ensure the list matches the original report.
5. Click **Add all charts** to embed them on the board.
6. The charts will be added as images to your Miro board.

## Requirements to embed Power BI data in Miro

To embed a Power BI report or dashboard into a Miro board, you must:

- Be part of a Miro team or account where the Power BI integration is enabled.
- Have access to the specific Power BI report or dashboard you wish to embed.
- Ensure that the Miro board where you wish to embed the Power BI data is not shared via public link.
- Have a supported Power BI Cloud service (Power BI Premium per capacity SKU or Fabric Capacity Reservation SKU). On premise service is not supported.

## Viewing and editing embedded Power BI data

Users who have access to the Miro board containing embedded Power BI data can view the data, regardless of their Power BI authorization or license status. This includes users with view, comment, or edit permissions for the board.

If you have edit permissions on a Miro board with embedded Power BI data, you can update it using the **Update** functionality or add charts using the **Add charts** functionality, even if you don't have access to the original Power BI content. However, it's not possible to explore or access the original chart's data or change filters through the integration.

## Data retention

The embedded Power BI data follows Miro’s standard data retention policy applied to all customer data. Read our [Miro Data Processing Addendum](https://miro.com/legal/documents/Miro-Data-Processing-Addendum.pdf).

## Troubleshooting

Follow these troubleshooting steps to resolve common issues encountered while using the Power BI integration in Miro.

Authorization and admin approval issues

If you cannot authorize the app or are prompted for admin approval without an option to request it, contact your Company Admin to ensure approval requests are enabled. If you see a **Need admin approval** window, request approval through the window.

Embedding issues

If charts do not appear as expected, reach out to your Company Admin to ensure you have the correct Microsoft Power BI subscription.

Link verification

For missing items, double-check the link used and ensure it's copied directly from the browser address bar.
