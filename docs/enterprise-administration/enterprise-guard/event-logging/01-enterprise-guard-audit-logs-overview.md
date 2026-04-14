---
title: Enterprise Guard audit logs overview
article_id: 17331872857746
sidebar_position: 2
created_at: '2024-02-27T21:08:55Z'
updated_at: '2025-11-25T15:41:36Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Audit logs provides admins with a comprehensive record of all events associated with Enterprise Guard. These logs are a valuable resource for efficient troubleshooting and offer detailed insights into critical events, such as updates to the trash time-to-live policy and trashed board permission policy, the creation, update, or deletion of retention policies for the organization, or the permanent deletion of a board from the trash. Systematically tracking these activities strengthens monitoring, analysis, and maintenance, ensuring a secure and well-managed system.

## Enterprise Guard events in audit logs

In addition to [the existing events logged](../../security-integrations/security-management/01-audit-logs.md#events-in-audit-logs), the audit logs include records about the following event categories and events associated with Enterprise Guard.

### Trash Policy

The following table lists the event categories and event actions logged for the Organization Trash Policy component.

|  |  |
| --- | --- |
| **Event category** | **Event action** |
| Administration | Trash time-to-live policy changed for the organization |
| Administration | Trashed board permission policy changed for the organization |

*Table 1: Event categories and event actions logged for the Organization Trash Policy component*For more information on trash policies, see [our documentation](https://help.miro.com/hc/articles/13860817985426-Trash-Policy).

### Retention Policy

The following table lists the event categories and event actions logged for the Content Retention Policies component.

|  |  |
| --- | --- |
| **Event category** | **Event action** |
| Administration | Retention policy created for organization |
| Administration | Retention policy updated for organization |
| Administration | Retention policy deleted for organization |

*Table 2: Event categories and event actions logged for the Content Retention Policies component*For more information on retention policies, see [our documentation](https://help.miro.com/hc/articles/16855776325778-Retention-Beta).

### Data Discovery

The following table lists the event categories and event actions logged for the Content Discovery component.

|  |  |
| --- | --- |
| **Event category** | **Event action** |
| Administration | Changed private information detection for the organization  (enabled/disabled) |
| Administration | Suppressed a data discovery match in the organization |

*Table 3: Event categories and event actions logged for the Content Discovery component*

For more information on data discovery, see [our documentation](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md).

### Intelligent Guardrails

The following table lists the event categories and event actions logged for the Intelligent Guardrails component.

|  |  |
| --- | --- |
| **Event category** | **Event action** |
| Intelligent guardrails | Intelligent guardrails changed for a board |

*Table 4: Event categories and event actions logged for the Intelligent Guardrails component*

For more information on Intelligent Guardrails, see [our documentation](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md).

### eDiscovery

The following table lists the event categories and event actions logged for the eDiscovery component.

|  |  |
| --- | --- |
| **Event category** | **Event action** |
| Administration | Case created for organization |
| Administration | Case closed for organization |
| Administration | Legal hold created for organization |
| Administration | Legal hold closed for organization |
| Administration | Legal hold applied to board Board released from legal hold |

*Table 3: Event categories and event actions logged for the eDiscovery component*

For more information on eDiscovery, see [our documentation](https://help.miro.com/hc/sections/22049853357842-eDiscovery-Legal-Hold-Beta).
