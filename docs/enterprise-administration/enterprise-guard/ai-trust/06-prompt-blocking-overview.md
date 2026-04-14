---
title: Prompt blocking overview
article_id: 29332642230546
sidebar_position: 6
created_at: '2025-09-09T07:58:00Z'
updated_at: '2026-01-12T11:23:15Z'
draft: false
---

Prompt blocking lets Sensitive Content Admins prevent users from submitting AI prompts that include sensitive information, helping you keep sensitive data out of Miro AI across your organization. Miro scans the text a user enters in the prompt field and any text-based content they add from the board. If that content matches the sensitivity labels or source code patterns selected in the Prompt blocking configuration, Miro blocks the prompt submission.

:::note
Only text-based content is supported in this release.
:::

## How it works

- You choose which label categories to block at the org level. Changes take effect immediately for everyone in your organization.
- When sensitive data is detected in a prompt, Miro AI shows a policy message in the user’s entry point, the prompt is blocked, and it cannot be sent to Miro AI.
- Prompt blocking and board scanning are different. Board scanning locates sensitive content on boards and can auto-classify the board. Prompt blocking reviews what users attempt to send to Miro AI.

## What gets blocked

- Privacy-related labels: Select from all our built-in privacy labels, such as SPII, HIPAA, credentials, financial numbers. For more information on our built-in privacy labels, see [Sensitivity labels and infotypes reference](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md).
- Code scanning. When enabled, Miro blocks prompts that include recognized source code. See [Code scanning](06-prompt-blocking-overview.md#code-scanning) for more details.

## Typical outcomes for users

When the user enters a prompt that contains sensitive information per your configuration:

- Users see a message such as We can’t generate this content as it may violate your organization’s policy.
- The prompt is not sent to Miro AI. Users can edit the prompt and try again.

## Code scanning

Code scanning blocks AI prompts that include recognizable source code. This requires a minimum of 5 lines of code to trigger blocking.

Example:

```
function connect() {

  const token = "example-token";

  fetch("https://api.example.com/health");

  return true;

}
```

## Supported languages

- C
- C#
- C++
- Go
- HTML
- Java
- JavaScript
- JSON
- PHP
- PowerShell
- Python
- Rust
- Shell script
- SQL
- TypeScript
