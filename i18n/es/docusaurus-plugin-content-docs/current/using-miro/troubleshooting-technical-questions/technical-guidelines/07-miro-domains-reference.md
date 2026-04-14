---
title: Referencia de dominios de Miro
article_id: 20857452690706
translation_id: 20857452690706
locale: es
sidebar_position: 8
created_at: '2024-08-20T08:12:36Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Este artículo de referencia enumera cada dominio que Miro utiliza en su aplicación SaaS.

:::note
Algunas aplicaciones de terceros desarrolladas para Miro, y las aplicaciones de Miroverse, pueden depender de dominios y servicios externos que Miro no controla.
:::

## Dominios de producción global

Las organizaciones que utilizan una red segura deben permitir los siguientes dominios de producción global:

```
*.miro.com
Nota: Incluye derivados, por ejemplo: *.api.miro.com | *.svc.miro.com
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

## Dominios de mecanización de producción

Las organizaciones que utilizan una red segura deben permitir los siguientes dominios de mecanización de producción:

```
api.stigg.io
Nota: Requerido para la funcionalidad de Miro AI.
```

```
*api.stigg.io
Nota: Requerido para la funcionalidad de Miro AI.
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

## Dominios regionales de producción

Las organizaciones que utilizan una red segura deben permitir los siguientes dominios regionales de producción.

:::note
Además de los dominios de producción global y los dominios de herramientas de producción, también debes permitir los dominios regionales de producción para la [residencia de datos](../../../enterprise-administration/canvas-25-admin-features/data-residency/02-data-residency-at-miro.md) en Australia o Estados Unidos, según corresponda.
:::

### Australia

```
*.au.miro.com
Nota: Incluye derivados, por ejemplo: *.api.au.miro.com | *.svc.au.miro.com
```

```
*.au01.miro.com
```

### Estados Unidos

```
*.us.miro.com
Nota: Incluye derivados, por ejemplo: *.api.us.miro.com | *.svc.us.miro.com
```

```
*.us01.miro.com
```
