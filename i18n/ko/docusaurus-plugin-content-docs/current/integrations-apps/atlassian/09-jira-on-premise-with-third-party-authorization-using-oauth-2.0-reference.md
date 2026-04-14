---
title: OAuth 2.0을 사용한 타사 인증을 포함한 Jira 온프레미스 참조
article_id: 26726425696530
translation_id: 26751147775378
locale: ko-kr
sidebar_position: 11
created_at: '2025-05-16T09:09:10Z'
updated_at: '2025-11-25T15:51:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '실행 가능한 사용자: 회사 관리자 어떤 플랜: Enterprise'
---

이 문서에서는 Jira와 Miro 통합을 위해 OAuth 2.0을 사용하는 타사 인증 서버 활용에 대한 기술 세부사항을 제공합니다.

연결 설정 방법을 알아보려면 [타사 인증 서버를 사용하여 Jira 온프레미스에 OAuth 2.0으로 연결](https://help.miro.com/hc/articles/25692796700306)을 참조하세요.

## 온프레미스 인증 및 OAuth 2.0을 사용하는 Miro와의 Jira 통합 작동 방식

다음 그래프는 Miro와 온프레미스 Jira 인증 서버 간의 통신 흐름을 보여줍니다.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*API 게이트웨이를 통한 온프레미스 인증 서버를 사용하는 Miro와 Jira 통합*

## 구성 매개변수

Miro와 Jira 간에 OAuth 2.0을 사용하는 타사 인증 서버를 통해 인증 흐름을 구성하려면 다음 매개변수를 지정해야 합니다.

- **인증 서버**
  - 인증 요청 URL
  - 토큰 요청 URL
  - 범위
- **승인 앱 구성**
  - 클라이언트 ID
  - 클라이언트 시크릿 키
- **Jira 인스턴스**
  - Jira 공개 URL
  - Jira 기본 URL; 내부 URL

> Miro는 등록된 앱을 기준으로 인증 서버가 유효성을 검사하는 리디렉션 URL을 제공합니다.

**추가 정보:** [OAuth 2.0을 사용하여 타사 인증 서버로 Jira 온프레미스에 연결하기](https://help.miro.com/hc/articles/25692796700306)를 참조하세요.

## Miro와 온프레미스 인증 서버 간의 사용자 인증 요청

Miro와 Jira 간의 통합을 위해 타사 인증 서버를 사용하는 경우, 다음 그래프는 사용자 인증 요청 흐름을 보여줍니다.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*사용자 인증 요청*

### 승인 요청

```
https://{authorization_URL}?
    response_type=코드&
    client_id={CLIENT_ID}&
    redirect_uri={Miro 리디렉션 URI}&
    scope={범위}&
    상태={state}
```

사용자는 구성을 통해 인증 요청에 매개변수를 키-값 쌍으로 추가할 수 있습니다.

### 토큰 요청

```
curl --요청 POST \
    --url '{토큰 요청 URL}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=authorization_code \
    --data 'client_id={CLIENT_ID}' \
    --data 'client_secret={CLIENT_SECRET}' \
    --data 'code={인증 코드 획득}' \
    --data 'redirect_uri={Miro 리디렉션 URI}' \
```

Miro가 인증 코드를 받으면, Miro는 상태를 제공하고 토큰 쌍을 요청합니다.

### 토큰 새로고침 교환

```
curl --request POST \
    --url '{token 요청 URL}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=refresh_token \
    --data 'client_id={CLIENT_ID}' \
    --data 'refresh_token={현재 유효한 리프레시 토큰}' \
```

토큰 새로고침 작업이 활성화되었는지 확인하고, API의 오프라인 액세스를 활성화하세요.

### Jira API 요청

```
curl --요청 가져오기 \
    --url {Jira Public URL}/rest/api/{apiversion}/... \
    --header 'authorization: Bearer {accessToken}" \
    --header 'content-type: application/json'
```

각 요청은 제공된 Jira 공개 URL을 기본 URL로 사용하고 사용자 액세스 토큰을 베어러 토큰으로 사용합니다.
