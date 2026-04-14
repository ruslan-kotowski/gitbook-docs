---
title: Set up a Looker integration
article_id: 25112862440978
sidebar_position: 4
created_at: '2025-03-05T14:00:46Z'
updated_at: '2025-06-04T08:30:26Z'
draft: false
---

:::note
For comprehensive admin docs with details and further information on the Miro + Looker Integration, please refer to the [Looker admin documentation](https://docs.google.com/document/d/1AUCQWRwDICLygwVmwSxXpz7RmRivPit0EIKgBMIkT6A/edit?usp=sharing).
:::

To set up a **Looker** integration with Miro, you must register the OAuth app in Looker.

## Prerequisites

- Ensure that a **Company admin** has approved Looker for your Miro organization.

## Register OAuth app in Looker

1. In the **Looker Marketplace**, find and select **API Explorer extension**.
2. Select **Install**.
3. Go to **Home** > **Applications** > **API extension**.
4. Find and select **Register OAuth App**.
5. Select **Run**.
6. A menu opens where you can add Request data.
   Add the following values:
   - **client_guid**: `15609152-a12a-4fa1-b364-337e7896d25d`
   - **body**:

   ```
   {
     "redirect_uri": "https://integrations.miro.com/api/contenthub/public/oauth/callback",
     "display_name": "Miro",
     "description": "Miro Looker Integration",
     "enabled": true,
     "group_id": ""
   }
   ```
7. Select **I understand that this API endpoint will change data**.
8. Select **Run**.
9. A successful run returns the body with a **HTTP 200** response code.
   - 💡 If the returned body includes `"enabled":false`, then run the Update OAuth App API with the same values as in step 6.

You have successfully set up a Looker integration with Miro.

## More information

- See [Looker API Reference](https://developers.looker.com/api/explorer/4.0/methods/Auth/register_oauth_client_app) (External).
