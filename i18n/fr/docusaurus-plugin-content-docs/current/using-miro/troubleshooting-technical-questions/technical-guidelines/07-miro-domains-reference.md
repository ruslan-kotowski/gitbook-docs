---
title: "R\xE9f\xE9rence des domaines Miro"
article_id: 20857452690706
translation_id: 20857452690706
locale: fr
sidebar_position: 8
created_at: '2024-08-20T08:12:36Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Cet article de référence liste chaque domaine que Miro utilise dans son application SaaS.

:::note
Certaines applications tierces développées pour Miro, et les applications Miroverse, peuvent s’appuyer sur des domaines et des services externes que Miro ne contrôle pas.
:::

## Domaines de production mondiaux

Les organisations qui utilisent un réseau sécurisé doivent autoriser les domaines de production globaux suivants :

```
*.miro.com
Note : Incluez les dérivés, par exemple : *.api.miro.com | *.svc.miro.com
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

## Domaines de l’outillage de production

Les organisations qui utilisent un réseau sécurisé doivent autoriser les domaines d’outils de production suivants :

```
api.stigg.io
Note : Nécessaire pour la fonctionnalité Miro AI.
```

```
*api.stigg.io
Note : Nécessaire pour la fonctionnalité Miro AI.
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

## Domaines de production régionaux

Les organisations qui utilisent un réseau sécurisé doivent autoriser les domaines de production régionaux suivants.

:::note
En plus des domaines de production mondiaux et des domaines d'outillage, vous devez également autoriser les domaines de production régionaux pour la [résidence des données](../../../enterprise-administration/canvas-25-admin-features/data-residency/02-data-residency-at-miro.md) en Australie ou aux États-Unis, selon le cas.
:::

### Australie

```
*.au.miro.com
Note : Incluez les dérivés, par exemple : *.api.au.miro.com | *.svc.au.miro.com
```

```
*.au01.miro.com
```

### États-Unis

```
*.us.miro.com
Note : Incluez les dérivés, par exemple : *.api.us.miro.com | *.svc.us.miro.com
```

```
*.us01.miro.com
```
