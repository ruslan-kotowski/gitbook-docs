---
title: Talktrack Admin security
article_id: 11148211487378
sidebar_position: 8
created_at: '2023-04-24T08:12:36Z'
updated_at: '2025-11-25T16:22:19Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Talktrack allows individual users to record interactive video or audio walkthroughs of their Miro board so they can share their ideas without spending extra time in meetings. Learn how Miro ensures Enterprise-grade security and compliance for Talktrack.

> ***Miro UI updates in phased rollout***
> Miro is enhancing the board user interface to be more inclusive and intuitive, and introducing an evolution of Projects called Spaces. The rollout will occur gradually for all Miro accounts over several weeks.
>
> In case you already have the enhanced UI and Spaces layout, this article may describe entry-points that have changed.
>
> To view the most current documentation, see [Miro's new simplified user interface](../../../using-miro/working-on-the-board/02-miro's-new-simplified-user-interface.md).
>
> This article will be updated when the rollout is complete.

:::note
Grant access to [Talktrack](../../../using-miro/facilitation-tools/asynchronous-tools/02-talktrack-board-recordings.md) for your organization in your [Feature access](../../managing-enterprise-teams-and-content/06-feature-activation.md) settings.
:::

:::note
You can learn about Talktrack's privacy and security details in the [Miro Talktrack whitepaper for Enterprises](https://go2.miro.com/rs/228-GPV-835/images/Talktrack_WhitePaper.pdf).
:::

## Enterprise-grade security

Miro is the enterprise-ready online workspace for innovation that empowers distributed teams of any size to dream, design, and build the future together. In the office, remote, or a mix, your teams can use Miro for every use case across the company.

But with that comes great responsibility, which is why we take security as seriously as we do collaboration — to help keep your ideas safe.

|  |  |  |
| --- | --- | --- |
| **Checkmark.png**  **Approved and certified** | **Security_lock.png**  **Trusted protection** | **Fingerprint.png**  **Secure access management** |
| Industry best practices and regulatory requirements | Protect and manage your intellectual property | Control who can access and manage your Miro content |

## Approved and certified

Miro follows industry best practices and regulatory requirements, including [ISO 27001, SOC2 Type II, and SOC3](https://miro.com/trust/compliance/). We also ensure your infrastructure and services are compliant with GDPR standards — this includes Talktrack recordings.

**Content lifecycle management**

**Talktrack deletion**
**Deleting a Talktrack:** When a Talktrack is deleted, it can’t be restored.

**Deleting a board:** Talktracks are layered recordings that provide context to a board. If a board is deleted, its Talktracks will also be deleted. However, if an admin restores a deleted board within 90 days, the board's Talktracks will also be restored. Read more about [board deletion](../../../using-miro/managing-boards/07-how-to-delete-a-board.md).

**Privacy**

**Data captured when recording a Talktrack:** The recorder's cursor movements and the viewport of the Miro board, the content of the board at the time the Talktrack is created, the recorder's video, either their camera view or avatar depending on whether the camera is on or off, the recorder's audio from the selected audio source, and any other audio that is present in the same physical space as the presenter.

**Data not captured when recording a Talktrack:** The cursor or information of any other users who are accessing the board at the time of recording, the recorder's screen or computer sounds.

**Privacy notice**

The legal basis for processing personal data related to Talktrack, where Miro is controller (essentially metadata), are performance of a contract (self-serve users) and/or legitimate interests (all users). The customer is the controller of the data recorded with Talktrack. The customer’s legal basis is for the customer to assess and likely to be legitimate interests.

**Accessibility**

Talktrack provides keyboard navigation and auto-transcription/closed caption support.

**Observability**

[Audit logs](../../security-integrations/security-management/01-audit-logs.md) are available for Talktrack in the admin settings. We have integrations with the following SIEM (Security Information and Event Management) systems:
[Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md)
[IBM QRadar](../../security-integrations/security-information-and-event-management-siem/02-miro-connector-for-ibm-qradar.md)

**External auditing**

Miro leverages best-in-class external consulting firms to perform annual audits. Our current ISO 27001 certification is signed by BSI (British Standard Institution) from the UK and the SOC2 & SOC3 reports by KirkpatrickPrice from the US. Read more about [compliance at Miro](https://miro.com/trust/compliance/).

## Trusted protection

Protect and manage the intellectual property created or added to our platform. Your data is encrypted in transit with the TLS 1.3 protocol and at rest with AES 256.

**Encryption**

Data in Miro — including Talktrack data — is by default encrypted at rest with the AES256 algorithm and in transit with TLS1.3 protocol. Read more in our [Miro Encryption Whitepaper](https://go2.miro.com/rs/228-GPV-835/images/Encryption%20Whitepaper.pdf).

**Data classification**

The [Board classification](../../canvas-25-admin-features/data-security/02-data-classification.md) label is not visible while watching or recording a Talktrack.

**Encryption Key Management**

If your organization has [Encryption Key Management](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md) (EKM) configured and deployed, Admins can request that Miro use your organization's encryption key for Talktrack content.

**Data residency**

By default, Talktrack data is stored in the same location as other customer content data in Miro: on AWS servers located in the EU. Miro provides a higher level of control and compliance over your company's data by ensuring all your customer content is hosted in Europe. For customers who have requested for [US Data Center Residency](../../canvas-25-admin-features/data-security/09-us-data-center-residency.md), Talktrack data is stored in our primary data center in Ohio and back up data center in Virginia.

## Secure access management

Control who can access Miro with enterprise-grade functionality, leveraging advanced identity and administrative capabilities. Read more about Enterprise Plan [security & compliance features](../../../administration/security-compliance).

**Controlling your organization’s access to Talktrack**

Company admins can grant or revoke access to Talktrack for the entire company or specific teams in their [Feature access](../../managing-enterprise-teams-and-content/06-feature-activation.md) settings.

**Access to record a Talktrack**

The option to [record a Talktrack](../../../using-miro/facilitation-tools/asynchronous-tools/02-talktrack-board-recordings.md#how-to-create-a-talktrack) is available for users that have commenting or editing access on a board, or are board owners or co-owners.

**Access to view a Talktrack**

Talktrack playback is available for all users that have [access to the board](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Frequently asked questions

Can a company admin see which boards have a Talktrack?

You can only see if a board has a Talktrack by opening it. If the board is not shared with you, you can use [content admin permissions](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) to gain access and see the Talktrack.

How can I turn off Talktrack for my company or team?

To turn off Talktrack, go to your [Feature access](../../managing-enterprise-teams-and-content/06-feature-activation.md) settings and select **No one can use**, or remove access for specific teams by clicking **X** next to the team name.

What happens to existing Talktracks when an admin revokes access to the Talktrack feature?

Existing Talktracks will remain available, but no new Talktracks can be recorded.

Can admins delete Talktracks?

Admins can share a board with themselves in the [content admin permissions](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), and then delete the Talktrack from the board.

Are the names of users shown on the app and/or saved with Talktrack data?

Talktrack displays the name (either first and last name or display name, depending on availability) during playback and as the "recorder name." However, Talktrack only saves user IDs, so no personal information is saved with the recording. If the user is not part of the organization during playback, the display name will show as "Unknown User."
