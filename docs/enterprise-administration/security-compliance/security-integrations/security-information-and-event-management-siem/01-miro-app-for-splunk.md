---
title: Miro app for Splunk
article_id: 4404745057170
sidebar_position: 1
created_at: '2021-08-05T11:26:49Z'
updated_at: '2025-11-25T16:06:50Z'
draft: false
---

[Miro's Splunk integration](https://splunkbase.splunk.com/app/5677) allows Enterprise customers to export two types of log data into Splunk for advanced security monitoring, compliance reporting, and operational analysis across the organization. This integration supports:

- [Audit logs](../../../security-integrations/security-management/01-audit-logs.md): capture user and system-level activity across your entire organization, such as user access, board sharing, permission changes, app installations, logins, and administrative actions.
- [Content logs](../../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md) (Enterprise Guard add-on): capture detailed content-level activity inside Miro boards, such as creation, editing, and deletion of board objects (widgets, sticky notes, images, text, frames), as well as comment activity.

## Best practices

- Use separate indexes for Audit Logs and Content Logs.
- Plan retention periods based on compliance needs.
- Review both log types together for comprehensive activity monitoring.

## Prerequisites

- Enterprise Plan subscription.
- Enterprise Guard add-on is required to enable Content Logs.
- Admin access to both:
  - Miro Admin Console (to enable SIEM and generate tokens)
  - Splunk instance (to configure data inputs)

## Generating access tokens in Miro

Both audit log and content log tokens can be generated from the same location in Miro:

1. Navigate to **Enterprise Integrations → Apps & Integrations** in your Admin Console.
2. For Audit Logs: Enable the **SIEM** toggle.
   For Content Logs: Enable the **eDiscovery** toggle.

Alternatively, generate tokens by registering a custom Miro app with the scopes: **auditlogs:read**, **contentlogs:export**.

:::warning
Audit Logs and Content Logs use separate tokens. Select the correct token for each input type.
:::

You will also need your **Organization ID** — this can be copied from your Admin Console URL:
`https://miro.com/app/org/\{organization_id\}/...`

## Installing and configuring the Splunk app for Miro

1. Install the [Miro Splunk app](https://splunkbase.splunk.com/app/5677) from Splunkbase.
2. In your Splunk instance, go to **Miro App → Inputs**.
3. Click **Create New Input**.
4. Select the desired input type: **Audit Logs** or **Content Logs** (for Enterprise Guard customers).
5. Provide the following information:
   - **Token** — select the appropriate token based on input type.
   - **Organization ID**.
   - **Time interval** — determines how often Splunk pulls new events.
   - **Index** — specify which index to store log data. For Content Logs, a separate index is recommended due to higher volume and data sensitivity.

Once configured, Splunk will begin collecting log events from Miro.

## Troubleshooting

- Ensure that tokens are correctly generated and mapped to the right input type.
- Verify Organization ID matches your Admin Console.
- Validate that indexes are correctly created and permissions assigned in Splunk.

## Search logs in Splunk

After you configure the data inputs, you can search and analyze logs in Splunk using the indexes you assigned for Audit Logs and Content Logs.

- **Audit Logs:**

  ```
  index="your_audit_index" source="miro_audit_logs"
  ```
- **Content Logs:**

  ```
  index="your_content_index" source="miro_content_logs"
  ```

Replace `your_audit_index` and `your_content_index` with the indexes you specified during input setup. You can use standard Splunk search, filtering, and visualization functions on both log types.

## Data visualization in Splunk

The Splunk App for Miro includes pre-built dashboards for Audit Logs to help you monitor user and system activity. After you set up Content Logs, you can build custom dashboards to visualize board-level content changes using Splunk's standard visualization tools.

Use filters, charts, and time-based graphs to analyze trends such as:

- Board content deletions or changes over time
- Spike detection for mass content modifications
- User activity on sensitive boards

:::note
Out-of-the-box dashboards in the Splunk App are currently designed for Audit Logs. Content Logs can be analyzed through custom search queries and dashboards depending on your organization's needs.
:::

Click to view the User Activity visualizations XML code.

```
<dashboard theme="light" version="1.1">
<label>Miro User Activity</label>
<description>Overview of user events in your Miro account.</description>
<search id="basesearch">
<query>source=miro_audit_logs | fields * | eval context.team.name = if(isnull('context.team'), 'context.team.name', "None") | search context.organization.name = "$form.organization$" context.team.name = "$form.team$"</query>
<earliest>$time.earliest$</earliest>
<latest>$time.latest$</latest>
</search>
<fieldset submitButton="false">
<input type="time" token="time">
<label>Time range</label>
<default>
<earliest>-30d@d</earliest>
<latest>now</latest>
</default>
</input>
<input type="dropdown" token="organization">
<label>Organization</label>
<fieldForLabel>context.organization.name</fieldForLabel>
<fieldForValue>context.organization.name</fieldForValue>
<search base="basesearch">
<query>| table context.organization.name | dedup context.organization.name</query>
</search>
<choice value="*">All</choice>
<default>*</default>
<initialValue>*</initialValue>
</input>
<input type="dropdown" token="team">
<label>Team</label>
<choice value="*">All</choice>
<default>*</default>
<initialValue>*</initialValue>
<fieldForLabel>context.team.name</fieldForLabel>
<fieldForValue>context.team.name</fieldForValue>
<search base="basesearch">
<query>| table context.team.name | dedup context.team.name</query>
</search>
</input>
</fieldset>
<row>
<panel>
<single>
<title>Total events</title>
<search base="basesearch">
<query>| stats count</query>
</search>
<option name="drilldown">none</option>
</single>
</panel>
</row>
<row>
<panel>
<chart>
<title>Events by date</title>
<search base="basesearch">
<query>| timechart count as Events</query>
</search>
<option name="charting.axisTitleX.visibility">collapsed</option>
<option name="charting.axisTitleY.visibility">visible</option>
<option name="charting.axisY2.enabled">0</option>
<option name="charting.chart">area</option>
<option name="charting.chart.nullValueMode">gaps</option>
<option name="charting.chart.stackMode">stacked</option>
<option name="charting.drilldown">none</option>
<option name="charting.layout.splitSeries">0</option>
<option name="charting.legend.mode">standard</option>
<option name="charting.legend.placement">none</option>
<option name="refresh.display">progressbar</option>
</chart>
</panel>
<panel>
<chart>
<title>Events by team</title>
<search base="basesearch">
<query>| rename context.team.name as Team | stats count as "Events" by Team | sort - "Events"</query>
</search>
<option name="charting.chart">pie</option>
<option name="charting.chart.sliceCollapsingThreshold">0.03</option>
<option name="charting.drilldown">all</option>
<option name="refresh.display">progressbar</option>
<drilldown>
<set token="form.team">$click.value$</set>
</drilldown>
</chart>
</panel>
</row>
<row>
<panel>
<single>
<title>Board events</title>
<search base="basesearch">
<query>| search event = board_* | stats count</query>
</search>
<option name="drilldown">none</option>
</single>
</panel>
<panel>
<single>
<title>Boards created</title>
<search base="basesearch">
<query>| search event = board_created | stats count</query>
</search>
<option name="drilldown">none</option>
</single>
</panel>
<panel>
<single>
<title>Boards opened</title>
<search base="basesearch">
<query>| search event = board_opened | stats count</query>
</search>
<option name="drilldown">none</option>
</single>
</panel>
</row>
<row>
<panel>
<chart>
<title>Boards opened or created</title>
<search base="basesearch">
<query>| search event = board_created OR event = board_opened | timechart count as "Boards created" by event</query>
</search>
<option name="charting.axisTitleX.visibility">collapsed</option>
<option name="charting.axisTitleY.visibility">visible</option>
<option name="charting.chart">column</option>
<option name="charting.chart.stackMode">stacked</option>
<option name="charting.drilldown">none</option>
<option name="charting.layout.splitSeries">0</option>
<option name="charting.legend.placement">right</option>
<option name="refresh.display">progressbar</option>
</chart>
</panel>
</row>
</dashboard>
```

Click to view the Security Activity visualizations XML code.

```
<dashboard theme="light" version="1.1">
<label>Miro Security Activity</label>
<description>Overview of security events in your Miro account.</description>
<search id="basesearch">
<query>source=miro_audit_logs | fields * | search context.organization.name = "$form.organization$"</query>
<earliest>$time.earliest$</earliest>
<latest>$time.latest$</latest>
</search>
<fieldset submitButton="false">
<input type="time" token="time">
<label>Time range</label>
<default>
<earliest>-30d@d</earliest>
<latest>now</latest>
</default>
</input>
<input type="dropdown" token="organization">
<label>Organization</label>
<fieldForLabel>context.organization.name</fieldForLabel>
<fieldForValue>context.organization.name</fieldForValue>
<search base="basesearch">
<query>| table context.organization.name | dedup context.organization.name</query>
</search>
<choice value="*">All</choice>
<default>*</default>
<initialValue>*</initialValue>
</input>
<input type="dropdown" token="team">
<label>Team</label>
<choice value="*">All</choice>
<default>*</default>
<initialValue>*</initialValue>
<fieldForLabel>context.team.name</fieldForLabel>
<fieldForValue>context.team.name</fieldForValue>
<search base="basesearch">
<query>| table context.team.name | dedup context.team.name</query>
</search>
</input>
</fieldset>
<row>
<panel>
<single>
<title>Successful sign-ins</title>
<search base="basesearch">
<query>| search event = sign_in_succeeded | stats count</query>
</search>
<option name="drilldown">none</option>
</single>
</panel>
<panel>
<single>
<title>Failed sign-ins</title>
<search base="basesearch">
<query>| search event = sign_in_failed | stats count</query>
</search>
<option name="drilldown">none</option>
</single>
</panel>
</row>
<row>
<panel>
<chart>
<title>Sign-ins by authentication method</title>
<search base="basesearch">
<query>| search event = sign_in_* | timechart count as Events by details.authType</query>
</search>
<option name="charting.axisTitleX.visibility">collapsed</option>
<option name="charting.axisTitleY.visibility">visible</option>
<option name="charting.axisY2.enabled">0</option>
<option name="charting.chart">column</option>
<option name="charting.chart.nullValueMode">gaps</option>
<option name="charting.chart.stackMode">stacked</option>
<option name="charting.drilldown">none</option>
<option name="charting.layout.splitSeries">0</option>
<option name="charting.legend.mode">standard</option>
<option name="charting.legend.placement">right</option>
<option name="refresh.display">progressbar</option>
</chart>
</panel>
</row>
<row>
<panel>
<table>
<title>Sharing events</title>
<search base="basesearch">
<query>| search event = *public_link* OR event = *sharing* | rename context.team.name as Team createdBy.name as User object.name as Board details.role as Details event as Event | table id _time Event Team User Board Details</query>
</search>
<option name="count">10</option>
<option name="drilldown">cell</option>
<option name="refresh.display">progressbar</option>
</table>
</panel>
</row>
<row>
<panel>
<table>
<title>File events</title>
<search base="basesearch">
<query>| search event = board_exported OR event = file_* | rename context.team.name as Team createdBy.name as User object.name as Board details.type as Type details.object as Object event as Event | table id _time Event Team User Board Type Object</query>
</search>
<option name="count">10</option>
<option name="drilldown">cell</option>
<option name="refresh.display">progressbar</option>
</table>
</panel>
</row>
</dashboard>


```
