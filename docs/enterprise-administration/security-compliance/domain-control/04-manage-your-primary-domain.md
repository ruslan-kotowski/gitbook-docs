---
title: Manage your corporate domain
article_id: 34249718672274
sidebar_position: 3
created_at: '2026-03-23T15:02:45Z'
updated_at: '2026-03-27T15:52:53Z'
draft: false
user_segment_id: null
user_segment: Everyone
---

Your corporate domain helps Miro identify who belongs to your organization (internal users) and who does not (external users). Users with email addresses from your coprporate or verified domains are treated as internal, while those from other domains are treated as external, even if they are assigned a paid license.

## What is a corporate domain

A corporate domain is the main email domain your organization uses, for example, `yourcompany.com`. Miro uses your corporate domain together with any verified domains to determine whether a user belongs to your organization.

## How your corporate domain is set

Miro automatically assigns a corporate domain when your organization is created or upgraded to a Business or Enterprise plan. This domain is based on the email address of the organization creator. For example, if the creator’s email is `john.smith@example.com`, Miro sets `example.com` as the corporate domain.

For organizations created before domain management was introduced, Miro may assign a corporate domain based on the email domain of the first Company Admin. You can keep this domain, verify it, or contact Support if it needs to be changed.

## Manage your corporate domain

To view and manage your domains, go to **Company settings → Domain management**.

The domain marked with the building icon indicates your current corporate domain.

## Change or delete your corporate domain

Each organization can have only one corporate domain at a time.

You can only delete your corporate domain if another verified domain is available. When you delete it, one of your verified domains becomes the new corporate domain.

If no other verified domain is available, contact Miro Support to change or remove your corporate domain.

## Add and verify additional domains

If your organization uses more than one email domain, you can add and verify additional domains. Verified domains are also treated as internal domains, ensuring all users with company email addresses are recognized as part of your organization.

## External users and licenses

Users with email addresses outside your corporate or verified domains are treated as external users. External users can still be invited as Members and assigned licenses. They:

- remain classified as external
- access content based on assigned teams
- appear in the user list as Members

## FAQs

### Can I have more than one corporate domain?

No. Each organization can have only one corporate domain. You can add multiple verified domains.

### Do I need to verify my corporate domain?

No. Miro assigns a corporate domain automatically. However, verification is required to enable features such as Single Sign-on (SSO) and domain control policies.

### Why do I already see a corporate domain?

Miro may have automatically assigned a corporate domain based on your organization’s first Company Admin. This helps identify internal users from the start.

### What if my domain is already claimed by another organization?

You can still have a corporate domain assigned, but you may need to contact Support to verify or update the domain.

### What if my organization was created using a personal email, for example, Gmail?

Miro cannot automatically identify a company domain in this case. Users are treated as external until a corporate domain is added and verified.
