---
title: Monitor encryption key management status
article_id: 31325531757970
sidebar_position: 2
created_at: '2025-11-24T17:59:06Z'
updated_at: '2026-04-02T09:24:29Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Admins can monitor and track the status of their encryption key management (EKM) configuration in the Miro Admin console. This brings greater transparency into key onboarding and encryption progress, helping you stay informed without needing additional support.

## Check EKM status

1. In the Miro Admin console, go to **Enterprise Guard**.
2. Select **Encryption key management**.
3. In the **Status** section, review the current status and message.

## Understand EKM status

The **Status** section shows where you are in the EKM setup and encryption process.

| Status | What it means |
| --- | --- |
| **Custom keys added** | Miro is setting up encryption with your custom keys. Once ready, your keys automatically start encrypting content. |
| **Key activation in progress** | New content is encrypted with your custom keys. Re-encryption of existing content is in progress. |
| **Custom keys active** | All content is encrypted with your custom keys. |
| **Switching back default keys** | Miro is changing your encryption back to Miro’s default keys. Your custom keys will be removed. |

## Review configured keys

In the Keys section, you can view the identifiers for the keys currently configured for EKM. If Miro manages your custom keys, you may see a notification instead of a key ARN.

- **Primary key**

  Encrypts your organization’s boards, comments, and other content.
- **Backup storage key**

  Encrypts archived versions and backups.
- **Key ARN**

  The key identifier in [AWS KMS](https://aws.amazon.com/kms/). If Miro manages your custom keys, you may see a notification instead of a key ARN.

(Optional) To make changes to your keys (for example, if you see the wrong key or you want to switch back to default encryption), you can reach out to your Customer Success Manager or see [Contacting Miro Support](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
