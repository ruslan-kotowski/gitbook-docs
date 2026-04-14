---
title: "Looker \uD1B5\uD569 \uC124\uC815"
article_id: 25112862440978
translation_id: 25112862440978
locale: ko-kr
sidebar_position: 4
created_at: '2025-03-05T14:00:46Z'
updated_at: '2025-06-04T08:30:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: looker
---

:::note
Miro + Looker 통합에 대한 종합적인 관리자 문서와 상세 정보는 [Looker 관리자 문서](https://docs.google.com/document/d/1AUCQWRwDICLygwVmwSxXpz7RmRivPit0EIKgBMIkT6A/edit?usp=sharing)를 참조하십시오.
:::

Miro와 **Looker** 통합을 설정하려면 Looker에서 OAuth 앱을 등록해야 합니다.

## 전제 조건

- **회사 관리자**가 Miro 조직에 대해 Looker를 승인했는지 확인합니다.

## Looker에서 OAuth 앱 등록하기

1. **Looker 마켓플레이스**에서 **API Explorer 확장**을 찾아 선택합니다.
2. **설치** 선택.
3. **홈** > **애플리케이션** > **API 확장**으로 이동합니다.
4. **OAuth 앱 등록**을 찾아 선택합니다.
5. **실행**을 선택하세요.
6. 메뉴가 열리면 요청 데이터를 추가할 수 있습니다.
   다음 값을 추가합니다.
   - **client_guid**: `15609152-a12a-4fa1-b364-337e7896d25d`
   - **본문**:

   ```
     "redirect_uri": "https://integrations.miro.com/api/contenthub/public/oauth/callback"
     display_name: Miro
     설명 Miro Looker 통합
     "활성화": 참,

   }
   ```
7. **API 엔드포인트가 데이터를 변경할 것임을 이해합니다**를 선택하세요.
8. **실행** 선택
9. 성공적인 실행은 본문과 함께 **HTTP 200** 응답 코드를 반환합니다.
   - 반환된 본문에 `"enabled":false`가 포함된 경우, 6단계와 동일한 값으로 Update OAuth App API를 실행하세요.

Looker 통합이 Miro에 성공적으로 설정되었습니다.

## 추가 정보

- [Looker API 참조](https://developers.looker.com/api/explorer/4.0/methods/Auth/register_oauth_client_app) (외부).
