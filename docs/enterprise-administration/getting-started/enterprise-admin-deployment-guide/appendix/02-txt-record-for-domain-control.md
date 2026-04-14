---
title: TXT record for Domain Control
article_id: 21918939001234
sidebar_position: 2
created_at: '2024-10-11T10:01:26Z'
updated_at: '2025-01-16T09:39:16Z'
draft: false
---

To verify your domain with Domain Control, use the following specifications to compose your TXT record:

- **Alias** | **Host** | **Name**
  - If domain, leave blank.
  - If subdomain:

    ```
    @
    ```
- **Answer** | **Description** | **Value**

  ```
  “miro-verification=[INSERT VERIFICATION CODE]”
  ```
- **Time to live (TTL)**

  ```
  86400
  ```
