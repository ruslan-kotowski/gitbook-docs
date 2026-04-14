---
title: Miro domains reference
article_id: 20857452690706
sidebar_position: 8
created_at: '2024-08-20T08:12:36Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
---

This reference article lists each domain that Miro uses in its SaaS application.

:::note
Some third-party applications developed for Miro, and Miroverse applications, may rely on external domains and services that Miro does not control.
:::

## Global production domains

Organizations that use a secured network must allow the following global production domains:

```
*.miro.com
Note: Include derivatives, for example: *.api.miro.com | *.svc.miro.com
```

```
*.miro-apps.com
```

```
mirostatic.com
```

```
*.mirostatic.com
```

```
onlinewhiteboard.com
```

```
realtimeboard.com
```

```
*.realtimeboard.com
```

```
webwhiteboard.com
```

## Production tooling domains

Organizations that use a secured network must allow the following production tooling domains:

```
api.stigg.io
Note: Required for Miro AI functionality.
```

```
*api.stigg.io
Note: Required for Miro AI functionality.
```

```
braze.eu
```

```
*.braze.eu
```

```
browser.sentry-cdn.io
```

```
cdn.cookielaw.org
```

```
fonts.googleapis.com
```

```
fonts.gstatic.com
```

```
miroapp.github.io
```

```
realtimeboardhelp.zendesk.com
```

```
*.sentry.io
```

```
split.io
```

```
*.split.io
```

## Regional production domains

Organizations that use a secured network must allow the following regional production domains.

:::note
In addition to global production domains, and production tooling domains, you must also allow regional production domains for [data residency](../../../enterprise-administration/canvas-25-admin-features/data-residency/02-data-residency-at-miro.md) in Australia, or United States, whichever applies.
:::

### Australia

```
*.au.miro.com
Note: Include derivatives, for example: *.api.au.miro.com | *.svc.au.miro.com
```

```
*.au01.miro.com
```

### United States

```
*.us.miro.com
Note: Include derivatives, for example: *.api.us.miro.com | *.svc.us.miro.com
```

```
*.us01.miro.com
```
