---
title: Manage Prompt blocking
article_id: 30612936057234
sidebar_position: 8
created_at: '2025-10-29T00:48:53Z'
updated_at: '2026-01-12T11:23:52Z'
draft: false
---

To adjust which labels are blocked or to toggle code scanning:

1. Go to **Settings** → **Enterprise Guard** → **Data discovery** → **Configuration**.
2. In **Prompt blocking**, select **Manage**.
3. In the side panel, do any of the following:
   - Turn **Select all** on or off.
   - Check or uncheck specific label categories you want to block.
   - Toggle **Code scanning** on or off.
4. Select **Apply changes**.

Changes take effect immediately for all users. Prompts containing newly unblocked items will proceed. Prompts containing still-blocked items will continue to be stopped.

## Related reference

- [Sensitivity labels and infotypes reference](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md)
- [Code scanning](06-prompt-blocking-overview.md#code-scanning)
