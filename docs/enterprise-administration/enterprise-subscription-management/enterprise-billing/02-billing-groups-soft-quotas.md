---
title: Billing Groups Soft Quotas
article_id: 20150819688338
sidebar_position: 2
created_at: '2024-07-15T07:02:19Z'
updated_at: '2026-02-19T10:36:29Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: billing-groups
---

## Overview

Soft quotas are a new UI update to Billing Groups, allowing administrators to set an optional soft limit on the number of licenses assigned to a billing group. This feature provides greater transparency and actionable data for managing license assignments.

Soft quotas offer a flexible and informative way to manage license assignments within billing groups, ensuring administrators have the data they need to make informed decisions.

## Setting Soft Quotas

### Adding a Soft Quota

Administrators can add a soft quota when creating or editing a billing group. This limit is based on the total number of licenses assigned versus the total number of licenses available.
The overall soft quota limit for each billing group appears at the top of the Billing Group’s overview, displayed as a numerical value and a line progress bar.

When set, the soft quota limits also appear in the Billing Group Table.

### Visual Indicators

- **Green Bar:** Indicates the billing group is within the assigned license limit.
- **Red Bar and Warning Icon:** Indicates the billing group has exceeded the assigned license limit.

## Managing Soft Quotas

### Exceeding the Limit

Exceeding the soft quota limit does not affect how licenses are assigned. The purpose is to provide transparency and actionable data for administrators.

### Quick Filters

Administrators can filter billing groups by:

- **Quota Set:** To view groups with a set soft quota.
- **Quota Exceeded:** To view groups that have exceeded their soft quota limit.
