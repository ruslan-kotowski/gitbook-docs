---
title: 감사 로그
article_id: 360017571434
translation_id: 360017571434
locale: ko-kr
sidebar_position: 1
created_at: '2019-02-11T10:09:04Z'
updated_at: '2026-03-12T09:21:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '사용 가능 대상: Enterprise 플랜 설정 가능한 사용자: 회사 관리자'
---

감사 로그를 통해 Miro 조직의 관리자는 사용자 활동을 추적할 수 있습니다. 이러한 로그는 문제를 조사하거나 중요한 이벤트(예: 글로벌 보안 설정 변경, 신규 사용자 초대, 새 보드 생성)의 상세 보고서를 받을 때 매우 유용합니다.

:::note
현재 이벤트는 Enterprise 구독을 시작한 시점부터 기록되며 기본적으로 180일 동안 저장됩니다:
a) 다른 플랜에서 Enterprise 플랜으로 업그레이드할 경우, 업그레이드 시점부터 이벤트가 기록됩니다.
b) 일부 팀을 Enterprise 구독으로 이전할 경우, 그들의 데이터는 구독에 포함된 시점부터 기록됩니다.
:::

## 감사 로그 접근

감사 로그에 접근하려면 다음 단계를 따르세요:

1. **회사 설정**으로 이동하세요.
2. 왼쪽 패널에서 **보안** > **감사 로그**를 클릭하세요.
3. **날짜 범위**, **행위자**, **이벤트 카테고리**, 특정 **이벤트**를 선택하여 감사 로그를 필터링할 수 있습니다.

필터링 조건에 맞는 이벤트를 미리 보려면 View events 버튼을 클릭하세요. 시간은 **ISO 8601** 형식으로 **로컬** 시간대에 표시됩니다. **세부 사항** 열의 세 점 아이콘을 클릭하여 특정 이벤트의 세부 정보를 볼 수 있습니다.

:::note
최근 90일 동안 발생한 이벤트만 미리 볼 수 있습니다.
:::

## 감사 로그 내보내기

로그를 **CSV** 파일 형식으로 내보낼 수 있습니다.

CSV 내보내기 파일에서, 이벤트 날짜 및 시간은 ISO 8601 형식과 UTC 시간대로 제공됩니다. 한 번에 내보낼 수 있는 기록의 수에는 제한이 없으나, 많은 데이터를 내보낼수록 파일을 준비하는 데 시간이 더 걸립니다. 또한, 테이블 작업을 위한 인기 애플리케이션들이 열 수 있는 데이터의 양에는 제한이 있다는 점에 유의하세요.

로그를 내보내려면 **CSV로 내보내기** 버튼을 클릭하세요.

내보낸 파일 세부 정보가 아래에 표시됩니다. 파일 다운로드가 준비되면, CSV 다운로드 버튼을 클릭할 수 있습니다. 파일은 24시간 동안 다운로드할 수 있습니다.

:::note
현재는 한 번에 한 개의 내보내기 파일만 각 조직에서 다운로드할 수 있습니다. **CSV로 내보내기** 버튼을 클릭하면 현재 내보내기 파일이 대체됩니다.
:::

## API를 통한 감사 로그 접근

관리자는 [감사 로그 API](https://developers.miro.com/reference/audit-logs)나 지원되는 [보안 정보 및 이벤트 관리(SIEM) 통합](https://help.miro.com/hc/sections/4404757427090-Security-information-and-event-management-SIEM)을 사용해 프로그래밍 방식으로 감사 로그 데이터를 액세스하고 수집할 수 있습니다.

## 감사 로그 삭제

관리자는 감사 로그의 보유 정책을 설정할 수 있습니다. 30일, 90일, 180일, 또는 365일 중에서 선택할 수 있습니다.

:::warning
감사 로그가 삭제되면 복구할 수 없습니다.
:::

:::note
감사 로그의 무기한 보유는 사용되지 않습니다.
:::

삭제 기간을 설정하려면 다음을 수행하세요.

1. **회사 설정**으로 이동합니다.
2. 왼쪽 패널에서 **보안** > **감사 로그**를 클릭합니다.
3. **감사 로그**에서 **설정** 탭을 클릭합니다.
4. 드롭다운 목록에서 옵션을 선택합니다. 선택을 확인하라는 메시지가 표시됩니다.

## 감사 로그의 이벤트

감사 로그에는 다음과 같은 이벤트 카테고리에 대한 기록이 포함됩니다.

**관리**

- 회사 이름 변경
- 회사 로고 변경, 삭제
- 액세스 요청 생성
- 액세스 요청 거부
- 분석에서 사용자 활동 지표 사용 설정, 해제
- SSO/SAML 설정 사용 설정, 해제 또는 변경
- SCIM 사용 설정, 해제
- SCIM API 토큰 생성
- SCIM 알림 사용, 끄기
- 허용 목록 사용, 끄기, 변경[허용 목록](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)
- 허용된 도메인 외부 게스트와의 공유 사용, 끄기
- [공개 링크](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)로 공유 사용, 끄기
- [편집을 위한 공개 링크](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)로 공유 사용, 끄기
- [팀 개인정보 보호](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) 켜기, 끄기
- [도메인 제어](../../canvas-25-admin-features/domain-control/01-domain-control.md) 설정 켜기, 끄기, 업데이트
- [비활성화된 사용자 차단](../../user-management/02-block-deactivated-users.md) 켜기, 끄기
- 요청 [관리 설정](../../user-management/09-request-management-on-enterprise-plan.md) 변경 (ServiceNow 이메일이나 서비스 데스크 URL 변경 포함)
- 팀 생성 및 삭제
- 팀 이름 변경
- 팀 로고 변경 및 제거
- [팀 초대 설정 변경](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- [팀 공개 변경](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)
- [팀을 위한 게스트 활성화/비활성화](../../managing-enterprise-teams-and-content/07-team-management-on-enterprise-plan.md)
- [기본 보드 공유 설정 변경](../../../using-miro/sharing-boards/11-default-sharing-settings.md)
- [기본 프로젝트 공유 설정](../../../using-miro/sharing-boards/11-default-sharing-settings.md) 변경
- 앱 설치, 제거
- [앱 승인, 제한](../../../integrations-apps/integrations-basics/04-how-to-install-apps.md)
- [Miro AI 모더레이션](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md)

**사용자 관리**

- 새로운 팀 멤버 초대
- 멤버를 게스트로 전환
- 사용자를 풀 멤버로 전환
- 사용자를 회사 관리자로 승격, 회사 관리자 해임
- 사용자를 팀 관리자로 승격, 팀 관리자 해임
- 팀 또는 회사에서 사용자 삭제 (사용자가 팀을 떠나면, 그들은 행위자이자 영향을 받는 객체로 작용)
- 초대 취소
- 사용자 비활성화, 사용자 재활성화
- 사용자가 팀/회사에 참여

**보드**

- 보드 열기
- 보드 만들기, 삭제하기, 복원하기
- 보드 이름 변경하기
- 보드 설명 변경하기
- 보드 커버 변경하기
- 보드를 다른 팀으로 이동하기
- 보드를 프로젝트에 추가 및 제거하고 다른 프로젝트로 이동하기
- 보드 소유자 변경하기
- 뷰어/댓글 작성자/편집자와 보드 공유하기
- 보드에서 사용자 제거
- 보드 [공개 링크](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) 활성화, 비활성화, 변경
- 공개 보드의 [암호](../../../using-miro/sharing-boards/13-password-protection-for-public-boards.md) 활성화, 비활성화, 변경
- 보드를 회사와 [공유하기](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) 활성화, 비활성화, 변경
- 보드를 팀과 [공유하기](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md) 활성화, 비활성화, 변경
- 보드 내보내기,  보드에서 파일 다운로드.
- 상태 생성됨
- 상태 업데이트됨
- 상태 삭제됨
- 파일 업로드 (사용되지 않음, [콘텐츠 로그](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md)에서 이용 가능)

유의하세요, 감사 로그는 보드에서의 변경사항에 관련된 정보를 기록하지 않습니다.

**템플릿**

- 템플릿 열기
- 템플릿 생성, 삭제, 복원
- 템플릿 이름 변경
- 템플릿 소유자 변경
- 상태 생성됨
- 상태 업데이트됨
- 상태 삭제됨

**프로젝트**

- 프로젝트 만들기, 삭제하기
- 프로젝트 이름 변경
- 프로젝트를 사용자와 공유하기, 프로젝트 참여자 제거
- 프로젝트 팀 공유 활성화, 비활성화
- 프로젝트 소유자 변경

**로그인**

- 로그인
- 로그인 실패
- 로그아웃
- 프로필 잠금, 잠금 해제

:::warning
로그인 이벤트는 [비활성화된 사용자](../../user-management/01-deactivated-users.md)의 활동을 포함합니다.
:::

**프로필 세부 정보**

- 프로필 세부 정보 변경
- 이메일 주소 변경 요청
- 이메일 주소 변경

**프로젝트 플랜**

- 프로젝트 플랜 만들기
- 프로젝트 플랜 삭제하기
- 프로젝트 플랜 섹션 만들기
- 프로젝트 플랜 섹션 삭제하기
- 프로젝트 플랜 소유자 변경

**Miro AI**

- Miro AI 기능 사용하기

### 자주 묻는 질문

감사 로그를 자동으로 가져올 방법이 있나요?

네, [Splunk용 Miro 앱](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md)을 설정하여 Splunk에서 Miro 로그에 접근할 수 있습니다.
