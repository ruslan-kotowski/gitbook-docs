---
title: Miro Connector For IBM QRadar
article_id: 6964551810834
sidebar_position: 2
created_at: '2022-08-03T11:29:28Z'
updated_at: '2025-02-26T11:34:22Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Get actionable insights from the Audit Logs of your Miro Enterprise plan with The Miro Connector for IBM QRadar. Detect, prioritize and respond to security threats faster and use this integration to effortlessly ingest Miro Audit Log data directly into your IBM QRadar SIEM system.

The connector is available for QRadar 7.4.2+.

- Gain actionable insights by monitoring key user activity to enable more informed decision-making.
- Get real-time monitoring and visibility. Automate ingestion of data from Miro’s Audit Logs directly into IBM QRadar, without requiring manual data exports or mapping.
- Streamline Security Monitoring. Easily monitor and detect threats or policy violations, and protect your organization’s sensitive data.
- Speed incident analysis and remediation by using QRadar’s prioritized alerts.

This guide describes the steps to install and configure IBM QRadar for Miro Enterprise plan.

## Overview

IBM QRadar is an enterprise security information and event management (SIEM) product. It collects log data from enterprise customers, its network devices, host assets and operating systems, applications, vulnerabilities, and user activities and behaviors.

The Miro app for IBM QRadar uses the [Audit Logs API](https://developers.miro.com/reference#get-logs "https://developers.miro.com/reference#get-logs") to fetch Miro Enterprise Audit Logs into IBM QRadar.

## Prerequisites

- Download and install the Miro Audit Logs custom DSM from the [IBM App Exchange](https://exchange.xforce.ibmcloud.com/hub "https://exchange.xforce.ibmcloud.com/hub")
- Install [Universal Cloud REST API Protocol](https://www.ibm.com/docs/en/dsm?topic=configuration-universal-cloud-rest-api-protocol "https://www.ibm.com/docs/en/dsm?topic=configuration-universal-cloud-rest-api-protocol")

## Configure Log Sources for Miro

Follow these steps to configure new Log Source Management.

1. In order to add a new log source in IBM QRadar first make sure that the [Log Source Management app](https://www.ibm.com/docs/en/qradar-common?topic=app-installing-qradar-log-source-management "https://www.ibm.com/docs/en/qradar-common?topic=app-installing-qradar-log-source-management") is installed in your QRadar console under the **Admin** tab.![Configure_log_sources_for_Miro.jpeg](images/21017430471570_Configure%20log%20sources%20for%20Miro.jpeg)**Configuring log sources for Miro in QRadar**

**2.** After being redirected to a new tab select **Log Sources**.![Manage_log_sources.jpeg](images/21017430473362_Manage%20log%20sources.jpeg)*Managing log sources in QRadar*

3. Click on **New log Source** and select **Single Log Source.*![New_log_source.jpeg](images/21017430474130_New%20log%20source.jpeg)Add a new log source*

![Adding_a_single_or_multiple_log_sources.png](images/21017430475154_Adding%20a%20single%20or%20multiple%20log%20sources.png)

*Select single log source*

4. Search and select **Miro Audit Logs** as the **Log Source type.**Then click **Step 2: Select Protocol Type.**

![Select_a_log_source_type.png](images/21017430478994_Select%20a%20log%20source%20type.png)

*Select log source type*

5. Search and select Universal Cloud REST API as the protocol type. Then Click **Step 3: Configure Log Source Parameters.*![Select_a_protocol_type.png](images/21017417442066_Select%20a%20protocol%20type.png)*Select protocol type**

6. Configure the following log source parameters, leaving the remaining parameters as default:

- **Name**: Text field. I.e: Miro Audit Logs
- **Extension**: MiroAuditLogsCustom_ext
- **Coalescing Events**: off

Then click **Step 4: Configure Protocol Parameters.**![Configure_log_source_parameters.png](images/21017417443474_Configure%20log%20source%20parameters.png)

![Configure_log_source_parameters_2.png](images/21017417444882_Configure%20log%20source%20parameters%202.png) *Configure log source parameters*

:::warning
In order to avoid IBM QRadar combining all events into a single event is important to make sure that **Coalescing Events** option is switched off.
:::

7. Configure the following protocol parameters, leaving the remaining parameters as default:

- **Log Source Identifier:** Text field. I.e: miro-test
- **Workflow**: [Miro-Workflow.xml](https://github.com/IBM/IBM-QRadar-Universal-Cloud-REST-API/blob/master/Community%20Developed/Miro/Miro-Workflow.xml "https://github.com/IBM/IBM-QRadar-Universal-Cloud-REST-API/blob/master/Community%20Developed/Miro/Miro-Workflow.xml") content file
- **Workflow Parameter Values**: Add the [Miro SIEM authentication](#how-to-get-the-miro-siem-access-token) token to the [Miro-Workflow-Parameter-Values.xml](https://github.com/IBM/IBM-QRadar-Universal-Cloud-REST-API/blob/master/Community%20Developed/Miro/Miro-Workflow-Parameter-Values.xml "https://github.com/IBM/IBM-QRadar-Universal-Cloud-REST-API/blob/master/Community%20Developed/Miro/Miro-Workflow-Parameter-Values.xml")

```
<Value name="access_token" value="" />
```

Then click **Step 5:** **Test Protocol Parameters.*![Configure_protocol_parameters.png](images/21017417445522_Configure%20protocol%20parameters.png)Test the protocol parameters*

8. You can test whether the protocol parameters were set up correctly by clicking **Start Test,** or skip this step by clicking **Skip Test and Finish.*![Option_to_test_protocol_parameters.png](images/21017430489106_Option%20to%20test%20protocol%20parameters.png)Testing protocol parameters*

9. If you choose to test the protocol parameters and everything is set up correctly, you'll see the **Test Protocol Parameters** page with a green checkmark. ![Testing_protocol_parameters.png](images/21017417449234_Testing%20protocol%20parameters.png)*Successful protocol parameter test*

10. Once you click **Finish** the new **Log Source** should be displayed and enabled.![New_log_source_enabled.png](images/21017430491154_New%20log%20source%20enabled.png)
*New log source displayed and enabled*

11. Once the log source has been created, you need to deploy the changes. Go to the **Admin** tab in the IBM QRadar console and click **Deploy Changes**. ![Deploy_changes.png](images/21017417452178_Deploy%20changes.png)
*Deploy log source changes*

## Create a new event mapping in IBM QRadar (optional)

Next you need to create a new event mapping in IBM QRadar.

1. Once your log source is deployed you can see your log activity in the **Log Activity** tab in the IBM QRadar console. You can filter the log events by log source by clicking the **Add Filter** option.![Add_filter.png](images/21017430493842_Add%20filter.png)*Log source deployed in activity log in QRadar*

2. Select **Log Source [Indexed]** as Parameter, choose the **Log Source** you created in the previous steps (in this example, Miro Enterprise Test) and click **Add Filter.*![Adding_a_filter.png](images/21017430493586_Adding%20a%20filter.png)Log source deployed in activity log in QRadar*

3. After adding the new filter you can now select the time range. For example, Last 12 Hours.![Select_the_time_range.png](images/21017417454738_Select%20the%20time%20range.png)
*Selecting a the rime range for the new filter*

4. Create a new event mapping in IBM QRadar for **Unknown events** in Miro integration.  ![Unknown_event.png](images/21017417455378_Unknown%20event.png)
*The new log source with unknown event*

5. Select the **Unknown** event, click on the **Actions** option and then select the **DSM Editor** option. ![DSM_Editor.png](images/21017430496274_DSM%20Editor.png) *Editing an unknown event*

6. On the DSM Editor click on the **Event Mapping** tab and then click **plus** to add an event.![DSM_Editor.jpeg](images/21017417457682_DSM%20Editor.jpeg)
*Editing a new mapping event*

7. To create a new event mapping you need to provide the following parameters:

- **Event ID**: should match the **Event type** from this [IBM guide](https://www.ibm.com/docs/en/qradar-on-cloud?topic=mapping-creating-event-map-categorization) and it should be unique.
- **Event Category**: event

Once you've added the **Event ID** and **Event Category,** you need to add a QID Record by clicking on the **Choose QID** link. Refer to the [IBM guide](https://www.ibm.com/docs/en/qradar-on-cloud?topic=mapping-creating-event-map-categorization). ![Create_a_new_mapping_event.jpeg](images/21017417458322_Create%20a%20new%20mapping%20event.jpeg)*Creating event mapping*

8. In the QID Records modal window, configure the following parameters:

- **Name**: text field. I.e: Organization SCIM enabled
- **Description:** Description field
- **High Level Category:** QRadar team as suggested Category field
- **Low Level Category:** QRadar team as suggested Sub-Category field
  > ⚠️ To know more about IBM categories, please read the [IBM QRadar documentation](https://www.ibm.com/docs/en/qradar-on-cloud?topic=mapping-creating-event-map-categorization)

Then click **Save**.
![QID_record.png](images/21017430499602_QID%20record.png)*Saving the QID record configuration*

9. Once the QID Record is created you can select it by clicking **Ok.** ![QID_record_created.png](images/21017430500882_QID%20record%20created.png)*Selecting the saved QID record*

10. Now you can see the QID Record selected in the Create a new Event Mapping modal window. Click **Create** to finish the creation of the new event mapping. ![Create_a_new_event_mapping.jpeg](images/21017417465106_Create%20a%20new%20event%20mapping.jpeg)*New event mapping creation*

11. Now you can search the event mapping by the event ID.  ![SCIM_enabled.jpeg](images/21017430502674_SCIM%20enabled.jpeg)*Searching for the new event mapping*

## How to edit an existing QID Record (optional)

In case you need to edit an existing QID Record, you can use the [IBM QRadar interactive API.](https://www.ibm.com/docs/en/qradar-on-cloud?topic=api-accessing-interactive-documentation-page "https://www.ibm.com/docs/en/qradar-on-cloud?topic=api-accessing-interactive-documentation-page")  ![API_documentation.png](images/21017430503698_API%20documentation.png)*IBM QRadar API documentation*

1. In the interactive API, select folder **data_classification** and **qid_records**. Then search for a specific QID record by filtering by name in **Query** (i.e: name="Organization scim enabled") and click **T****ry it Out.** ![Search_for_QID_record.png](images/21017417469202_Search%20for%20QID%20record.png)
*Updating the interactive API*

2. Copy the id from the previous response and then select the **data_classification** folder, **qid_records** item and **qid_record_id.** Then filter by **qid_record_id** **> Path > Value** pasting the copied id and click **Try it Out.**  *![Test_QID_record.png](images/21017417470354_Test%20QID%20record.png)*

3. Copy the body from the previous response and then switch to the **POST** method. Here add the id you previously copied in **qid_record_id** > **Path** > **Value**, paste the body you copied from the previous step in **qid_record** > **Body** > **Value** and modify the desired attribute (i.e: description), then click **Try it Out**.  ![POST_method.png](images/21017417471122_POST%20method.png)

4. The description attribute will be updated accordingly. ![Description_attribute.jpeg](images/21017430509074_Description%20attribute.jpeg)*Description attribute updated*

## How to get the Miro SIEM access token

To get the Miro SIEM access token:

1. Log in to Miro as a Company Admin

2. Go to **Settings** > **Apps and integrations** > **Enterprise Integrations**

3. Toggle on **SIEM**

4. Copy the **Access token** ![Miro SIEM access token in Enterprise admin console](https://help.miro.com/hc/article_attachments/23921803737362)*Miro SIEM access token*
