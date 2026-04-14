---
title: Idle Session Timeout
article_id: 360017571454
sidebar_position: 2
created_at: '2019-02-11T10:09:05Z'
updated_at: '2025-02-06T08:46:57Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: enterprise
  roles: company_admin
---

Session timeout feature allows you to set up a**limit** on how long your end-users are allowed to be inactive. The setting affects all members and [guests](../../../using-miro/sharing-boards/07-collaboration-with-guests.md). If the user session hits the limit and expires, they are automatically logged off their Miro profile and will need to authorize again before accessing the Enterprise data.

:::warning
Be mindful when setting timeout limits. Highly secured timeout limits that are too short in duration will result in users continually being logged out of their boards. Consider a balanced, secure approach to session timeouts and remember to communicate timeout limits clearly with your users.
:::

### How to enable Idle Session Timeout

1. Go to **Company** settings > **Security** > **Authentication** > **Idle Session Timeout**
2. Toggle on **Automatically log out inactive users** and set the **Timeout limit**

   ![idle-session-timeout.png](images/23921804858002_idle-session-timeout.png)
*Idle Session Timeout is enabled*

Activating the Idle Session Timeout functionality for the first time will populate the 1-day default session. The Admin can customize the duration and input a custom integer value from 1 to 9999 and select the units: minutes, hours, or days. The minimum allowed duration is 1 hour and the maximum allowed duration is 14 days. We recommend setting a duration of no less than 8 hours.

For the Idle Session Timeout feature, we define inactivity as none of the following actions present anywhere in the app during the defined time:

- mouse movement (or touchscreen movement)
- mouse clicks (or touchscreen taps)
- pressing keyboard

There will be a warning message shown to users several minutes before the logout. Users can simply move their mouse or press any key on their keyboard to remain logged in.

:::note
The default Idle Session Timeout value is 1 day. Settings can range from 1 hour to 14 days.
:::

:::note
Idle Session Timeout works everywhere (accessing user activity on different devices, integrations etc).
:::

:::note
If a user is a visitor on a public board stored in an Enterprise plan but is not part of the Enterprise plan that enabled session timeout, they are not affected.
:::

:::note
If a user belongs to multiple organizations which have different Idle Session Timeout intervals in place, then the shortest duration will prevail. For example, a user belongs to one organization with a 6-hour Idle Session Timeout, and one organization with a 30-minute Idle Session Timeout - they will be timed out of all active sessions in 30 minutes.
:::
