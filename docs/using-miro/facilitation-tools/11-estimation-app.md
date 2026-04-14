---
title: Estimation app
article_id: 5651786248210
sidebar_position: 8
created_at: '2022-05-20T11:28:11Z'
updated_at: '2025-11-25T16:08:42Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: estimation
availability:
  plans: starter, business, enterprise
  roles: team members with editing rights on the board
---

Estimations are a vital part of agile development and planning. They help align team members on scope of work, identify gaps in analysis or understanding, and set clear expectations for delivery.

During estimations, team members assign a number to a task that reflects the amount of work required. In order to make realistic estimations, a numbering system is used which adds the previous numbers together. Team members can then discuss and align on the number they chose.

Use our estimation app to run multiplayer estimation sessions on a Miro board with [cards](../essential-tools/02-cards.md), [sticky notes](../essential-tools/14-sticky-notes.md) and [Jira Cards](../../integrations-apps/atlassian/03-jira-cards.md).

To start estimation:

1. Access the Estimation app from the Creation toolbar and select **Start new session**. You may need to add the Estimation app from the **Tools, Media and Integrations** (**+**) icon:
   ![estimation-entry-point.png](images/21537436002962_estimation-entry-point.png)*Estimation app on the toolbar*
2. Select the estimate scale: in the drop-down menu, choose the **T-shirt** (available for Miro [cards](../essential-tools/02-cards.md) only) or **Fibonacci** estimation technique.
3. Drag the estimation area across the objects you want to estimate. You can select cards, stickies, or [Jira Cards](../../integrations-apps/atlassian/03-jira-cards.md) for estimation. You can exclude particular objects from the estimation by clicking the blue dots.
4. If your selection includes Jira cards, you will be prompted to select the Jira board to which these cards belong. This ensures that your estimates are accurately and predictably saved in Jira. Without this step, Jira is unpredictable at saving these estimates.
5. Click **Estimate x cards/stickies** once you’re ready to start estimation.![estimation_launch.gif](images/21016786471186_estimation%20launch.gif)*Launching the estimation session*![estimation_app_jira_cards.png](images/21016786474514_estimation_app_jira_cards.png)*Using Estimation app with Jira Cards*

Everyone on the board (and those who join the board while the estimation session is ongoing) will be able to join the estimation session. Everyone participating must have board edit access and Jira permissions. Estimations can be done synchronously or asynchronously. All estimates are anonymous.

![join_estimation.jpg](images/21016751234578_join%20estimation.jpg)
*The pop-up to join the estimation session*

Users will be redirected to the first item to add their estimates after clicking **Join estimation**. Users can vote on all items or skip some items and vote on particular ones only. To edit an estimate, click the pen icon.

![adding_estimates.gif](images/21016751237010_adding%20estimates.gif)
*Estimation in progress*

As the session runs, the facilitator can see a poll of the estimates provided for each item and the avatars of who has provided an estimate. When all items have been provided estimates by all the required participants, the facilitator can “Choose the final estimate” for each item. The facilitator can also edit the agreed-upon estimates.

![agreed_estimates.gif](images/21016751238162_agreed%20estimates.gif)
*Estimation finished*

Once you agree on estimates for all items, the facilitator will see the pop-up with the option to end the session and share results. The facilitator can also click **End for all** to finish the session at any moment. This will show the number of total points. Click **End and share results** on the pop-up, and the session results will be saved.

![end_session.gif](images/21016751242386_end%20session.gif)
*Estimation agreement*

If you estimate Miro cards or stickies, the estimates are saved as tags on the cards or stickies.

![estimate_tags.jpg](images/21016786489362_estimate%20tags.jpg)
*Tags show the estimations of the cards*

If you estimate Jira Cards using the **Fibonacci** estimation technique, the estimates are saved to Jira (at the moment, syncing only works for Fibonacci estimates). Note that the facilitator should authorize with their Jira credentials prior to giving final estimates. The estimation results will be automatically synced with the corresponding Jira issues.

**For Fibonacci estimations to appear on Jira cards and in Jira tasks:**

1. Make sure the story points field is set up in Jira.
2. Check whether you have the relevant permission in Jira to update the value of the story points field.
