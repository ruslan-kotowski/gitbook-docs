---
title: Amazon Q (Beta)
article_id: 31347586131346
sidebar_position: 3
created_at: '2025-11-25T13:35:45Z'
updated_at: '2025-12-29T15:25:31Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  roles: board_owner, Board co-owners, board_editor, team_member, team_admin, User
    admins, Content admins, (Setup) Company admins; Amazon Q admin
  plans: business, enterprise
  platforms: browser, desktop
---

The Amazon Q integration enables teams to retrieve company knowledge into the Miro AI platform via Sidekicks and Flows. Enterprise intelligence is delivered and visualized directly inside Miro.

:::note
You can only use the Amazon Q integration with the Miro AI platform. [Sign-up here](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb) to get access.  You will be notified when the Miro AI platform is enabled for your organization.
:::

Enterprise knowledge is often scattered across numerous tools like Slack, Confluence, Salesforce, Google Drive, and internal repositories, which forces product managers, engineering leaders, and technology teams to spend valuable time searching for crucial details and aligning on insights.

The following Miro and Miro AI functionalities support Amazon Q integration:

- [**Flows**](../../using-miro/miro-ai/04-flows-overview.md)
  Visualize workflows that transform scattered information into clear deliverables, helping teams automate and standardize how they turn insights into action.
- [**Sidekicks**](../../using-miro/miro-ai/06-sidekicks-overview.md)
  Work in tandem with AI agents that reason over board content and enterprise data to generate new artifacts, give instant insights, and accelerate ideation, documentation, and design.

## Set up Amazon Q integration

Ensure that you have [signed-up here](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb), and have received confirmation from Miro that the Miro AI platform is enabled for your organization, then complete the following two procedures.

To set up the Amazon Q integration with Miro, you must add Miro as a data accessor in Amazon Q Business, then connect the Amazon Q index to the Admin Console in Miro.

### Add Miro as a data accessor in Amazon Q Business

1. In the Amazon Q Business console, in the navigation pane click **Applications**.
2. Click the application where you want to add a data accessor.
3. In the navigation pane, click **Data accessors**.
4. Click **Add data accessor**.
5. Under **Data accessors**, for **Miro** click the plus (**+**) icon.
6. For **External ID**, add your Miro organization ID.
   To get your Miro organization ID, in Miro go to Admin Console. Copy the organization ID from the browser URL bar.
   ![](images/31367058137746_image.png)
   *Find your organization ID in Admin Console. You can copy the ID from the browser URL bar.*
7. Click **Add data accessor**.
8. Note the following details. You need each value to complete the setup in Miro Admin Console:
   - Application ID
   - IdC application ARN
   - Retriver ID
   - Application region
   - IdC application region

### Connect an Amazon Q index to the Admin Console in Miro

1. In Miro, go to **Admin Console** > **Apps & integrations** > **Apps** > **Add apps**.
2. Search and locate Amazon Q.

   > ✏️ If you are unable to find Amazon Q by name, then search by the following client ID: `1601842442647206821`.
3. In the app profile, select whether to add the app for **All teams** or **Specific teams**.
4. Review the permissions page.

   > ✏️ The Amazon Q app is developed and maintained by Miro, and does not require specific permissions.
5. Click **Add**.
6. Go to **Apps** > **Manage Apps**.
7. Search and locate Amazon Q.
8. Click **Settings**.
9. Add the Amazon Q data accessor details. See the final step in [Add Miro as a data accessor in Amazon Q Business](#add-miro-as-a-data-accessor-in-amazon-q-business).
10. Click **Save**.
    Your configuration is applied.
