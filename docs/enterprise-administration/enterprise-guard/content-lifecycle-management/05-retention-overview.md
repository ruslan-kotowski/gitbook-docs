---
title: Retention overview
article_id: 19205049882770
sidebar_position: 5
created_at: '2024-05-28T17:53:34Z'
updated_at: '2026-01-05T11:47:05Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Retention ensures data protection and compliance by allowing administrators to define, edit, and delete policies tailored to their organization's needs. Retention policies play a crucial role in safeguarding Miro boards within the organization, allowing you to retain certain boards for a specified period of time. Retention ensures Miro boards do not get deleted accidentally or intentionally until the board is out of the retention period. By leveraging retention policies, organizations can ensure data protection, compliance, and the preservation of business-critical information automatically, at-scale.

Retention policies help mitigate the following risks and challenges:

- **Adherence to compliance requirements:** Data retention is a fundamental aspect of numerous data privacy laws, and non-compliance poses monetary and reputational risks.
- **Safeguarding business-critical information:** Preserving data employed in crucial decision-making processes is imperative for future reference and supports well-informed decision-making

## Release notes

- Creating, updating, or deleting a policy triggers the retention policies process, which can take up 24 hours to complete. However, updating the name or description of a policy happens immediately as these actions do not trigger the retention policies process.
- When a team is deleted, all the boards belonging to the team will be permanently deleted after the expiration time of the trashed team even if they are under retention. Deleted teams remain in the Deleted teams page for 90 days from the date of deletion. After this time period, the boards belonging to the deleted team are also permanently deleted even if they are under retention. For more information, see Understand Retention policies scenarios.
