---
title: Enterprise Guard Dashboard overview
article_id: 26707467343890
sidebar_position: 6
created_at: '2025-05-14T13:14:06Z'
updated_at: '2026-03-17T08:39:20Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

## Centralized security and governance view

The Enterprise Guard dashboard offers a centralized, high-level view of your organization’s security and information governance insights in one unified view. Designed for Enterprise Guard administrators, this dashboard brings together key metrics across core domains—including Data Discovery, Classification, Content Lifecycle, and eDiscovery—into a single, consolidated interface. It enables quick visibility into current exposure, policy coverage, and legal readiness—empowering administrators to detect potential risks early, take timely, proactive measures, and address any areas requiring attention.

## Real-time, actionable metrics

Each metric in the Enterprise Guard dashboard reflects real-time data, updated daily. All metrics are actionable and link directly to their respective domain dashboards, enabling administrators to explore detailed insights and configure settings as needed. Whether you're monitoring board sensitivity, classification status, retention policies, or legal holds, this dashboard provides a centralized starting point. This layered approach ensures consistency across the Enterprise Guard product and simplifies navigation for busy admins.

## Support for large-scale governance

The Enterprise Guard dashboard is especially useful for Enterprise Guard Admins managing large-scale deployments on the Enterprise plan. It brings clarity to complex information governance setups and supports informed decision-making by consolidating the most important signals in one place. As part of our commitment to a more intuitive Enterprise Guard experience, the Enterprise Guard dashboard helps admins not only understand what’s happening, but also what to do next—with links to take action directly from the data. Whether you're reporting to leadership or managing day-to-day data governance, this dashboard ensures you can access relevant information quickly, prioritize actions, and demonstrate the value of your organization’s security and compliance strategy.

## Related domain-specific dashboards

In addition to the Enterprise Guard dashboard, administrators can explore a suite of domain-specific dashboards designed to provide deeper insights and control across key areas of governance. Each of these dashboards enables focused decision-making within its respective area while maintaining alignment with the broader Enterprise Guard framework. These include:

- **Data Discovery dashboard:** surface and analyze where sensitive information resides across your boards.
- **Classification dashboard:** track and manage board-level classification coverage and sensitivity labels.
- **Content Lifecycle dashboard:** monitor data retention policies and automate lifecycle management actions.
- **eDiscovery dashboard:** gain visibility into legal holds and streamline eDiscovery preparation workflows.

## Understand dashboard metrics

Enterprise Guard dashboards include two types of metrics: current metrics and historic metrics. To ensure clarity and consistency, each metric presented in the Enterprise Guard dashboards is defined in the [Enterprise Guard dashboard metrics documentation](../../enterprise-subscription-management/enterprise-guard-overview/07-enterprise-guard-dashboard-metrics-reference.md).

:::note
Notes on metrics:

- All metrics in Enterprise Guard exclude boards of trashed teams and boards under legal hold.
- All classification metrics exclude templates and trashed boards.
:::

## Understand errors, empty states, and historical changes

Understanding how to interpret empty states and error messages is essential for accurately reading Enterprise Guard dashboard metrics.

### Understand behavior of historical data when settings change

If a feature, such as Classification, is disabled after data has been collected, historic metrics will still show values from the active period. For example, if you disable Classification in May and Classification was active in April with 20 boards classified:

- April values will continue to appear on the dashboard.
- The May graph will display **no data available**, as data collection has stopped.
