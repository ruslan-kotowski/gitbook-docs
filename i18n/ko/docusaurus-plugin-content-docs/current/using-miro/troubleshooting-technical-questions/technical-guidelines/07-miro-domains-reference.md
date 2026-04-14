---
title: "Miro \uB3C4\uBA54\uC778 \uCC38\uC870"
article_id: 20857452690706
translation_id: 20857452690706
locale: ko-kr
sidebar_position: 8
created_at: '2024-08-20T08:12:36Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

이 참조 문서는 Miro가 SaaS 애플리케이션에서 사용하는 각 도메인을 나열합니다.

:::note
Miro와 Miroverse용으로 개발된 일부 서드파티 애플리케이션은 Miro가 제어하지 않는 외부 도메인 및 서비스에 의존할 수 있습니다.
:::

## 글로벌 생산 도메인

보안 네트워크를 사용하는 조직은 다음의 글로벌 프로덕션 도메인을 허용해야 합니다:

```
*.miro.com
메모: 파생 도메인을 포함해야 합니다. 예를 들어: *.api.miro.com | *.svc.miro.com
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

## 프로덕션 툴링 도메인

보안 네트워크를 사용하는 조직은 다음 제작 툴 도메인을 허용해야 합니다:

```
api.stigg.io
메모: Miro AI 기능에 필요합니다.
```

```
*api.stigg.io
메모: Miro AI 기능에 필요합니다.
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

## 지역 생산 도메인

보안 네트워크를 사용하는 조직은 다음 지역 생산 도메인을 허용해야 합니다.

:::note
글로벌 생산 도메인 및 생산 도구 도메인 외에도, 호주 또는 미국의 [데이터 레지던시](../../../enterprise-administration/canvas-25-admin-features/data-residency/02-data-residency-at-miro.md)에 해당하는 지역 생산 도메인을 허용해야 합니다.
:::

### 호주

```
*.au.miro.com
메모: 파생 도메인을 포함하세요. 예: *.api.au.miro.com | *.svc.au.miro.com
```

```
*.au01.miro.com
```

### 미국

```
*.us.miro.com
메모: 파생 도메인을 포함하세요. 예: *.api.us.miro.com | *.svc.us.miro.com
```

```
*.us01.miro.com
```
