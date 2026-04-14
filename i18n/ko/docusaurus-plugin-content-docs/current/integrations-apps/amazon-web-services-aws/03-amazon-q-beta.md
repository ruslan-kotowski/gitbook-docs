---
title: Amazon Q (베타)
article_id: 31347586131346
translation_id: 31347586131346
locale: ko-kr
sidebar_position: 3
created_at: '2025-11-25T13:35:45Z'
updated_at: '2025-12-29T15:25:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: '실행 가능한 사용자: 보드 소유자, 보드 공동 소유자, 보드 편집자, 팀 구성원, 팀 관리자, 사용자 관리자, 콘텐츠 관리자, (설정)
    회사 관리자; Amazon Q 관리자 사용 가능 플랜: Business, Enterprise 사용 가능 플랫폼: 브라우저, 데스크톱'
---

Amazon Q 통합을 통해 팀은 회사 지식을 Miro AI 플랫폼으로 가져올 수 있으며, AI 팀원과 워크플로를 통해 중앙 집중화된 정보를 제공합니다. 기업 인텔리전스는 Miro 내에서 직접 제공되고 시각화됩니다.

:::note
Amazon Q 통합은 Miro AI 플랫폼에서만 사용할 수 있습니다. [여기에서 가입](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb)하면 접근 권한을 받을 수 있습니다. 조직에 Miro AI 플랫폼이 활성화되면 알림을 받게 됩니다.
:::

기업 지식은 종종 Slack, Confluence, Salesforce, Google Drive 및 내부 저장소와 같은 여러 도구에 분산되어 있어, 제품 관리자, 엔지니어링 리더, 기술 팀이 중요한 세부 정보를 검색하고 인사이트를 맞추는 데 소중한 시간을 소비하게 합니다.

다음의 Miro 및 Miro AI 기능은 Amazon Q 통합을 지원합니다:

- [**워크플로**](../../using-miro/miro-ai/04-flows-overview.md)
  분산된 정보를 명확한 산출물로 변환하는 워크플로를 시각화하여 팀이 인사이트를 행동으로 전환하는 방법을 자동화하고 표준화하도록 지원합니다.
- [**사이드킥**](../../using-miro/miro-ai/06-sidekicks-overview.md)
  보드 콘텐츠와 기업 데이터를 활용하여 새로운 산출물을 생성하고 즉각적인 인사이트를 제공하며, 아이디어 도출, 문서화 및 디자인을 가속화하는 에이전트와 함께 작업합니다.

## Amazon Q 통합 설정

[여기에서 가입](https://miro.com/integrations/aws/?utm_campaign=glb-26q4-nsp-pn-iw_o4-aws-ml-blog-no-sl&utm_source=partner-sourced&utm_medium=partner&utm_content=website&utm_term=amazonq&src=-partner_glb)하고, Miro에서 조직에 Miro AI 플랫폼이 활성화되었음을 확인 받은 후 다음 두 가지 절차를 완료하세요.

Miro와 아마존 Q 통합을 설정하려면, Amazon Q Business에서 Miro를 데이터 접근자로 추가한 다음, 관리자 콘솔에서 Amazon Q 인덱스를 Miro에 연결해야 합니다.

### Amazon Q Business에 Miro를 데이터 접근자로 추가하기

1. Amazon Q Business 콘솔의 내비게이션 창에서 **애플리케이션**을 클릭합니다.
2. 데이터 액세서를 추가하려는 애플리케이션을 클릭합니다.
3. 내비게이션 창에서 **데이터 액세서**를 클릭합니다.
4. **데이터 액세서 추가**를 클릭합니다.
5. **데이터 액세서** 항목에서 **Miro**에 대해 플러스 (**+**) 아이콘을 클릭합니다.
6. **외부 ID**로 Miro 조직 ID를 추가하세요.
   Miro 조직 ID를 얻으려면, Miro에서 관리자 콘솔로 이동하세요. 브라우저 URL 바에서 조직 ID를 복사합니다.
   ![](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/31367058137746_image.png)
   *관리자 콘솔에서 조직 ID를 찾으세요. 브라우저 URL 바에서 ID를 복사할 수 있습니다.*
7. **데이터 액세서 추가**를 클릭하세요.
8. 다음 세부 정보를 메모하세요. 각 값은 Miro 관리자 콘솔에서 설정을 완료하는 데 필요합니다:
   - 애플리케이션 ID
   - IdC 애플리케이션 ARN
   - Retriver ID
   - 애플리케이션 지역
   - IdC 애플리케이션 지역

### Amazon Q 인덱스를 Miro의 관리자 콘솔에 연결하기

1. Miro에서 **Admin Console** > **Apps & integrations** > **Apps** > **Add apps**로 이동합니다.
2. Amazon Q를 검색하고 찾습니다.

   > ✏️ Amazon Q를 이름으로 찾을 수 없다면, 다음 클라이언트 ID로 검색하세요: `1601842442647206821`.
3. 앱 프로필에서 앱을 **All teams** 또는 **Specific teams**에 추가할지 선택합니다.
4. 권한 페이지를 검토합니다.

   > ✏️ Amazon Q 앱은 Miro에서 개발 및 유지 관리되며, 특정 권한이 필요하지 않습니다.
5. **Add**를 클릭합니다.
6. **앱** > **앱 관리**로 이동합니다.
7. Amazon Q를 검색하여 찾습니다.
8. **설정**을 클릭합니다.
9. Amazon Q 데이터 접근자 세부 정보를 추가합니다. Amazon Q Business에 Miro를 데이터 접근자로 추가하기의 마지막 단계를 참조하세요.
10. **저장**을 클릭합니다.
    구성이 적용됩니다.
