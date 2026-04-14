---
title: Visual numbers in Tables
article_id: 31356870414610
sidebar_position: 18
created_at: '2025-11-25T19:40:55Z'
updated_at: '2026-03-13T12:26:15Z'
draft: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: tables
availability:
  roles: board_editor
  plans: business, enterprise
  platforms: browser, desktop, mobile
---

Visual Numbers lets users turn numbers into visual progress bars. Users can set conditional formatting rules with custom colors, and set min/max ranges for better data visualization. Visual numbers also allows for percentage or currency formatting.

## Format numbers visually

Visual number formatting transforms numeric data into progress bars, making it easier to spot trends and track progress at a glance. You can display numbers as percentages or currencies, set custom ranges, and apply conditional formatting rules.

Apply visual formatting to a number field:

1. Hover over a number or formula field name to show the **three dots** (**...**) icon.
2. Click the **three dots** (**...**) icon and select **Edit field**.
3. In the **Display** section of the dialog, click **Bar**.
   The numbers will display as progress bars.
4. Choose your format:
   1. Percentage (%): Best for completion rates, progress tracking.
   2. Currency: Select from major currencies ($, €, £, ¥, and more).
5. Set the **Min** and **Max** range for your progress bars. For percentages, typically use 0-100. For currency, set appropriate min/max values for your data.
6. Pick a bar color from the color picker.
7. Toggle number labels on or off:
   1. On: Shows the numeric value alongside the progress bar.
   2. Off: Shows only the progress bar for a cleaner view.
8. Click **Save**.

## Apply conditional formatting

Conditional formatting automatically colors your progress bars based on rules you define, helping you quickly identify values that need attention.

1. Open the **Field settings** for a number or formula field.
2. Toggle **Conditional colors** on.
3. Click **Add rule**.
4. Define your rule:
   1. Select a condition (equals, does not equal, is greater than, is less than, is greater than or equal to, is less than or equal to, is empty, is not empty).
   2. Enter the value to compare against (if applicable).
   3. Choose a color for values that match this rule.
5. Add multiple rules as needed. Drag and drop rules to set their priority. Rules at the top take precedence.
6. Click **Save**.

Conditional formatting appears in both the table view and the side panel when viewing individual records.

Visual number formatting is currently only available in table view and side panel.

Timeline, Kanban, and Cards views will show standard numeric formatting.
