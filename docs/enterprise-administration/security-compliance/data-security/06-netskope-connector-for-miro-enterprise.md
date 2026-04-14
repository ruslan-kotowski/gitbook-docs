---
title: Netskope connector for Miro Enterprise
article_id: 4415711060498
sidebar_position: 6
created_at: '2022-01-19T06:23:42Z'
updated_at: '2025-02-26T11:27:29Z'
draft: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: '[Enterprise plan](../../../plans-billing/miro-plans/04-enterprise-plan.md)'
---

Miro custom connector for Netskope enables visibility on data leakage related events and allows managing the following traffic inside Miro:

- [Downloading board backup](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)

This guide provides steps to configure Netskope for Miro Enterprise plan and describes the user experience.

### Create a new Miro app in Netskope

Inside your Netskope instance go to **Settings > Security Cloud Platform > App Definition** and click on **NEW CLOUD APP**:

![new_cloud_app.jpg](images/21016020258834_new%20cloud%20app.jpg)
*Creating a Cloud app in Netskope![](blob:https://miro.atlassian.net/8cb061a4-e184-4bd6-bb95-774cd34fc8e7#media-blob-url=true&id=78b7a8cb-792a-41da-bf16-b26ca4480059&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.08.43.png&size=181298&height=513&width=1028&alt=)*

To create a new app inside Netskope you will be asked to import the following JSON file **miro-activities-for-netskope.json**:

```
[
{ "version": "0.0.0.1" },
{
"domain_name": "miro.com",
"uri_path": "/api/v1/boards/.+/",
"http_method": "GET",
"uri_param": [{ "key": "archive", "value": "true" }],
"resp_code": "200",
"pattern": "",
"activity_name": "Download"
},
{
"domain_name": "miro.com",
"uri_path": "/api/v1/boards/.+/resources/.+/files/original",
"http_method": "GET",
"uri_param": [],
"resp_code": "307",
"pattern": "",
"activity_name": "Download"
}
]
```

Enter the application name, select the **Custom Connector** option, and click on **IMPORT FROM FILE > Add To Activity List** to upload the **miro-activities-for-netskope.json** file downloaded from the previous step**.**

![uploading_the_file.jpg](images/21016033728530_uploading%20the%20file.jpg)![](blob:https://miro.atlassian.net/f4beb3ad-27a3-49c8-baee-aa660161e315#media-blob-url=true&id=337f93cd-b545-47df-8f27-ca4fa5667a3f&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.14.30.png&size=207190&height=630&width=1039&alt=)
*Uploading the file*

After importing the **miro-activities-for-netskope.json** file the recorded activities will be displayed. Now you can proceed to click on **SAVE** and create the Miro app.

![save_the_app.jpg](images/21016020260242_save%20the%20app.jpg)
*Saving the app![](blob:https://miro.atlassian.net/b9da4e19-b3b1-4c25-aed3-762f458fd639#media-blob-url=true&id=f7549007-0265-42e1-b946-a3e167124f12&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.26.58.png&size=209044&height=693&width=1028&alt=)*

Once the app is created you need to select it and click on **APPLY CHANGES.**

*![apply_changes.jpg](images/21016020260626_apply%20changes.jpg)**The option to apply changes to the Miro app*

![](blob:https://miro.atlassian.net/82b8ac6e-1952-44e7-a62f-cefb7dbee6ab#media-blob-url=true&id=975f42e8-de5d-4bbb-ae07-c243cce9bb2f&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.32.06.png&size=257154&height=575&width=1780&alt=)

### Create a new Policy for your Miro app in Netskope

Once the application is created you can proceed to create a policy. For that, you can navigate to **Policy > R****eal-time Protection** and click on **NEW POLICY > Cloud App Access.**

![create_a_policy.jpg](images/21016033731218_create%20a%20policy.jpg)
*Creating a policy for your Miro app![](blob:https://miro.atlassian.net/d2ae8479-8f5c-4417-8b09-2b57ee344d90#media-blob-url=true&id=e9c82ee5-cdea-4b33-8491-9613a848be81&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.39.02.png&size=107320&height=321&width=635&alt=)*

Here in **Destination,** you need to provide the Miro app you created in the previous step, set up a **Policy Name,** and click on **SAVE.**

*![save_the_policy.jpg](images/21016020261906_save%20the%20policy.jpg)**Saving the policy*

![](blob:https://miro.atlassian.net/abf26593-27ad-40f4-b3e5-731a9e58d062#media-blob-url=true&id=0edd2e23-2762-4173-8f3f-9a7bb74bf217&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.45.14.png&size=200430&height=722&width=1575&alt=)Then you can select where do you prefer to place the policy and click on **SAVE.**

![](blob:https://miro.atlassian.net/370ad8f1-d9ac-40a2-a218-d132dde62914#media-blob-url=true&id=2db9fc4c-fd8d-47cf-a77b-f1fc02edbb15&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2019.27.01.png&size=77286&height=404&width=729&alt=)![move_policy.jpg](images/21016020262674_move%20policy.jpg)
*Selecting where you prefer to place the policy*

Finally, you can apply changes by clicking on **APPLY CHANGES** button.

![applying_changes.jpg](images/21016020268434_applying%20changes.jpg)
*Applying changes*

![](blob:https://miro.atlassian.net/41cdf802-aa1c-4f9a-bd22-950ea6ad755e#media-blob-url=true&id=7f85d987-6550-4271-90da-c9273a0cbc9a&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2019.29.17.png&size=157218&height=490&width=1576&alt=)

### Events visualization

Once you are all set, you can visualize the traffic by navigating to **Skope IT**, filtering by the custom Miro app, and clicking on **See Events** as follow.

![see_events.jpg](images/21016033740306_see%20events.jpg)
*The option to see traffic events*

### User experience

The users for whom the Download activities should be blocked need to have the Netskope client installed in their machine. When the users try to perform a Download backup operation, Netskope blocks the action and shows a native OS popup with a message.

![alert.jpg](images/21016033746578_alert.jpg)
*A message shown to users that are not allowed to download a backup of a Miro board*
