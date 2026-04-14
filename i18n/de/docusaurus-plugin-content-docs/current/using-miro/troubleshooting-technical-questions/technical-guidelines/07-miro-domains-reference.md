---
title: Miro-Domains-Referenz
article_id: 20857452690706
translation_id: 20857452690706
locale: de
sidebar_position: 8
created_at: '2024-08-20T08:12:36Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dieser Referenzartikel listet alle Domains auf, die Miro in seiner SaaS-Anwendung verwendet.

:::note
Einige für Miro entwickelte Anwendungen von Drittanbietern und Miroverse-Anwendungen können auf externe Domains und Dienste zurückgreifen, die nicht von Miro kontrolliert werden.
:::

## Globale Produktionsdomains

Organisationen, die ein gesichertes Netzwerk nutzen, müssen die folgenden globalen Produktionsdomains zulassen:

```
*.miro.com
Inklusive Derivate wie: *.api.miro.com | *.svc.miro.com
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

## Produktionsdomains für Tools

Organisationen, die ein gesichertes Netzwerk verwenden, müssen die folgenden Produktionsdomains für Tools zulassen:

```
api.stigg.io
Hinweis: Erforderlich für Miro AI-Funktionalität.
```

```
*api.stigg.io
Hinweis: Erforderlich für Miro AI-Funktionalität.
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

## Regionale Produktionsdomains

Organisationen, die ein gesichertes Netzwerk nutzen, müssen die folgenden regionalen Produktionsdomains zulassen.

:::note
Zusätzlich zu den globalen Produktionsdomains und Produktionswerkzeug-Domains müssen Sie auch regionale Produktionsdomains für den [Ort der Datenspeicherung](../../../enterprise-administration/canvas-25-admin-features/data-residency/02-data-residency-at-miro.md) in Australien oder den Vereinigten Staaten zulassen, je nachdem, was zutrifft.
:::

### Australien

```
*.au.miro.com
Hinweis: Inklusive Derivate wie: *.api.au.miro.com | *.svc.au.miro.com
```

```
*.au01.miro.com
```

### USA

```
*.us.miro.com
Hinweis: Inklusive Derivate wie: *.api.us.miro.com | *.svc.us.miro.com
```

```
*.us01.miro.com
```
