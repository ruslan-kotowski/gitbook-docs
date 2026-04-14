---
title: "Microsoft Sentinel \uD1B5\uD569"
article_id: 31325908249362
translation_id: 31325908249362
locale: ko-kr
sidebar_position: 1
created_at: '2025-11-24T18:16:15Z'
updated_at: '2025-12-16T15:49:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: audit-logs
---

## 개요

[Miro](https://miro.com/) 커넥터는 [Miro REST API](https://developers.miro.com/reference/overview)를 사용하여 Miro의 감사 로그와 콘텐츠 활동 로그를 Microsoft Sentinel로 수집합니다. 이는 Miro 워크스페이스의 활동 모니터링을 Microsoft Sentinel에서 중앙 집중화하여 보안 위협 탐지, 사건 조사 및 규정 준수를 위한 보고에 활용됩니다.

## 데이터 커넥터

이 솔루션에는 두 개의 데이터 커넥터가 포함되어 있습니다.

| 커넥터 | 플랜 요구사항 | 캡처하는 내용 | 참고 자료 |
| --- | --- | --- | --- |
| **Miro 감사 로그 (Enterprise 플랜)** | Enterprise 플랜 | 조직 전체의 감사 이벤트를 포함하여 사용자 인증, 콘텐츠 접근, 팀 변경, 관리 작업 등을 포함합니다. | [API 문서](https://developers.miro.com/reference/enterprise-get-audit-logs) | [감사 로그 개요](https://developers.miro.com/reference/audit-logs) |
| **Miro 콘텐츠 로그 (Enterprise 플랜 + Enterprise Guard)** | Enterprise 플랜 + Enterprise Guard 애드온 | 준법 감시 및 eDiscovery를 위한 항목 생성, 업데이트 및 삭제를 포함한 콘텐츠 활동 추적. | [API 문서](https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch) | [콘텐츠 로그 개요](https://developers.miro.com/reference/board-content-logs) |

## 전제 조건

### 일반 요구사항

- 활성화된 Microsoft Sentinel 워크스페이스.
- Miro 조직의 회사 관리자 역할.
- Miro OAuth 액세스 토큰(만료되지 않음).

### 연결기별 요구 사항

#### 감사 로그 연결기를 위한 요구 사항

- Miro Enterprise 플랜.
- OAuth 범위: `auditlogs:read`.
- 액세스 토큰.

#### 내용 로그 연결기를 위한 요구 사항

- Miro Enterprise 플랜 + Enterprise Guard 애드온.
- OAuth 범위: `contentlogs:export`.
- 액세스 토큰.
- Miro 조직 ID.

## 설치

Miro 커넥터를 설정하는 방법은 두 가지가 있습니다.

- **옵션 1 (권장):** 엔터프라이즈 통합 사용. 자동 토큰 생성으로 가장 간단한 설정.
- **옵션 2 (대안):** 맞춤형 OAuth 애플리케이션 생성. OAuth 앱 구성에 대한 더 많은 제어 가능.

**참고:** 옵션 1을 사용하는 경우 통합이 귀하의 조직에서 가장 많은 사용자가 있는 팀에 자동으로 연결됩니다. 옵션 2를 사용하는 경우, 앱을 설치할 팀을 선택할 수 있습니다. 그러나 팀 선택은 로그 수집에 영향을 미치지 않으며, 두 옵션 모두 조직 전체의 로그 접근을 제공합니다. 모든 팀의 통합 관련 이벤트가 로그에 포함됩니다.

### 옵션 1: Enterprise 통합 사용 (권장)

대부분의 사용자에게 가장 간단한 옵션입니다. Miro의 Enterprise 통합 설정을 통해 자동으로 OAuth 애플리케이션을 생성하고 액세스 토큰을 생성합니다.

#### 감사 로그 커넥터용

1. [Miro 회사 설정](https://miro.com/app/settings/)을 엽니다.
2. **앱 및 통합** 섹션을 확장합니다.
3. **Enterprise 통합**을 클릭합니다.
4. **SIEM** 토글을 활성화합니다.
5. **액세스 토큰** 값을 복사합니다.
6. 토큰을 안전하게 저장합니다.

#### 콘텐츠 로그 연결기용

1. [Miro 회사 설정](https://miro.com/app/settings/)을 엽니다.
2. **앱 및 통합** 섹션을 확장합니다.
3. **Enterprise 통합**을 클릭합니다.
4. **eDiscovery** 토글을 활성화합니다.
5. 나타나는 **액세스 토큰** 값을 복사합니다.
6. 브라우저 URL에서 **조직 ID** 확인하기:
   - 브라우저 URL을 확인하여 조직 ID를 찾습니다.
   - URL 형식은 다음과 같습니다: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - URL에서 조직 ID(숫자 값)를 복사합니다.
7. 토큰과 조직 ID를 안전하게 저장하세요.

### 옵션 2: 맞춤형 OAuth 애플리케이션 사용 (대안)

이 옵션은 OAuth 애플리케이션 구성에 대한 더 많은 제어를 제공합니다. 스코프를 맞춤 설정하거나 여러 통합을 관리하거나 수동 OAuth 앱 관리를 선호할 때 사용합니다.

#### 1단계: Miro OAuth 애플리케이션 생성

1. Miro 계정에 로그인합니다.
2. [Miro 앱 설정](https://miro.com/app/settings/user-profile/apps)으로 이동합니다.
3. **새 앱 만들기**를 클릭합니다.
4. 앱 생성 시, **만료되지 않는 액세스 토큰** 옵션을 선택합니다 ([OAuth 토큰에 대한 자세한 정보](https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens)).
5. 필요한 OAuth 범위를 활성화합니다:
   - `auditlogs:read` 감사 로그 커넥터용.
   - `contentlogs:export` 콘텐츠 로그 커넥터용 (Enterprise Guard 필요).
6. **앱 설치 및 OAuth 토큰 받기**를 클릭합니다.
7. **액세스 토큰**을 복사해 안전하게 보관합니다.

자세한 OAuth 설정 지침은 [OAuth 시작 방법](https://developers.miro.com/docs/getting-started-with-oauth)을 참조하세요.

#### 2단계: 조직 ID 얻기 (콘텐츠 로그 전용)

1. [Miro 회사 설정](https://miro.com/app/settings/)으로 이동합니다.
2. 브라우저의 URL을 확인하여 조직 ID를 찾습니다:
   - URL 형식은 다음과 같습니다: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - URL에서 조직 ID(숫자 값)을 복사합니다.

### Microsoft Sentinel에 솔루션 배포

1. Microsoft Sentinel에서 **콘텐츠 허브**로 이동합니다.
2. **"Miro"**를 검색하고 솔루션을 클릭합니다.
3. **설치**를 클릭하고 배포 마법사를 따릅니다.
4. 로그 분석 워크스페이스를 선택합니다.
5. 설치를 완료합니다.

### 데이터 커넥터 구성

#### Miro 감사 로그 커넥터

1. Microsoft Sentinel에서 **데이터 커넥터**로 이동합니다.
2. **Miro 감사 로그 (Enterprise 플랜)**을 찾아 **커넥터 페이지 열기**를 클릭합니다.
3. **연결**을 클릭합니다.
4. **접근 토큰**을 입력합니다.
5. **연결**을 클릭하여 커넥터를 활성화합니다.

#### Miro 콘텐츠 로그 커넥터

1. Microsoft Sentinel에서 **데이터 커넥터**로 이동합니다.
2. **Miro 콘텐츠 로그(Enterprise Plan + Enterprise Guard)**를 찾아 **커넥터 페이지 열기**를 클릭합니다.
3. **연결**을 클릭합니다.
4. **조직 ID**를 입력합니다.
5. **액세스 토큰**을 입력합니다.
6. **연결**을 클릭하여 커넥터를 활성화합니다.

데이터 수집은 커넥터 활성화 후 5-10분 이내에 시작됩니다.

## 데이터 테이블

### MiroAuditLogs_CL

조직 수준 감사 이벤트 포함:

- 사용자 인증 및 접근.
- 콘텐츠 작업.
- 팀 및 조직 변경.
- 사용자 프로필 수정.
- 관리자 작업.

**주요 열**

| 열 | 설명 |
| --- | --- |
| `TimeGenerated` | 이벤트 타임스탬프. |
| `event` | 특정 액션이나 활동을 식별하는 이벤트 이름. |
| `logType` | 로그 항목의 유형. |
| `category` | 관련 이벤트를 그룹화하는 이벤트 카테고리. |
| `createdBy_email` | 이벤트를 발생시킨 사용자. |
| `context_ip` | 이벤트의 IP 주소. |
| `details` | 이벤트별 추가 정보 (JSON). |

### MiroContentLogs_CL

콘텐츠 레벨의 활동 로그에는 다음이 포함됩니다:

- 사용자 속성과 타임스탬프를 포함한 항목 수준의 작업.
- 상태 전환 및 수정.
- 규정 준수 및 eDiscovery를 위한 활동 추적.

**주요 열**

| 열 | 설명 |
| --- | --- |
| `TimeGenerated` | 이벤트 타임스탬프 |
| `actionType` | 콘텐츠에 수행된 작업 유형. |
| `actor_email` | 작업을 수행한 사용자. |
| `itemType` | 영향을 받은 콘텐츠 아이템 유형. |
| `contentId` | 콘텐츠의 고유 식별자. |
| `state` | 아이템 상태 정보 (JSON). |

## 샘플 쿼리

### 최근 감사 이벤트 보기

```
MiroAuditLogs_CL
| sort by TimeGenerated desc
| project TimeGenerated, event, category, createdBy_email, context_ip
| take 20
```

### 사용자별 및 이벤트 유형별 활동

```
MiroAuditLogs_CL
| summarize EventCount = count() by createdBy_email, event, category
| order by EventCount desc
```

### 사용자별 콘텐츠 변경사항

```
MiroContentLogs_CL
| where TimeGenerated > ago(7d)
| summarize Changes = count() by actor_email, actionType
| order by Changes desc
```

### 시간에 따른 이벤트 추세

```
MiroAuditLogs_CL
| summarize count() by event, bin(TimeGenerated, 1h)
| render timechart
```

### 가장 활동적인 사용자 (콘텐츠 변경)

```
MiroContentLogs_CL
| where TimeGenerated > ago(30d)
| summarize TotalActions = count() by actor_email
| top 10 by TotalActions desc
```

## 문제 해결

### 데이터가 나타나지 않음

- 액세스 토큰이 유효하고 올바른 범위를 가지고 있는지 확인합니다.
- 콘텐츠 로그의 경우, 조직이 Enterprise Guard 애드온을 확인합니다.
- 조직 ID가 정확한지 확인합니다 (콘텐츠 로그용).
- 초기 데이터 수집을 위해 5–10분 기다립니다.
- **데이터 커넥터** 페이지에서 커넥터 상태를 확인합니다.

### 인증 오류

#### 옵션 1(엔터프라이즈 통합 토글 사용)을 사용하는 경우

- [Miro 회사 설정](https://miro.com/app/settings/)으로 이동하여 **앱 및 통합**을 확장하고 **엔터프라이즈 통합**을 클릭합니다.
- 토글(감사 로그의 SIEM, 콘텐츠 로그의 eDiscovery)이 여전히 활성화되어 있는지 확인합니다.
- 다른 관리자가 토글을 비활성화한 경우, 토큰이 무효화됩니다.
- 토글을 다시 활성화하여 새 토큰을 생성하고 커넥터 구성을 업데이트합니다.
- Miro에서 회사 관리자 역할을 갖고 있는지 확인합니다.

#### 옵션 2(맞춤형 OAuth 앱)를 사용하는 경우

- 토큰이 [Miro 앱 설정](https://miro.com/app/settings/user-profile/apps)에서 해지되지 않았는지 확인하세요.
- OAuth 애플리케이션에 필요한 범위가 활성화되어 있는지 확인하세요.
- 필요 시 토큰을 재생성하고 커넥터 설정을 업데이트하세요.
- Miro에서 회사 관리자 역할을 가지고 있는지 확인하세요.

### 콘텐츠 로그가 작동하지 않음

- Miro 플랜에 **Enterprise Guard** 애드온이 포함되어 있는지 확인하세요 (기본 Enterprise 플랜에는 제공되지 않습니다).
- OAuth 범위 `contentlogs:export`가 활성화되어 있는지 확인하세요.
- 조직 ID가 올바른지 다시 확인하세요.
- Enterprise Guard로 업그레이드가 필요하면 Miro 계정 관리자에게 연락하세요.

## 리소스

### Miro 도움말 센터 리소스

- **Miro 감사 로그:** `../security-integrations/security-management/01-audit-logs.md
- **Miro 콘텐츠 로그:** `../canvas-25-admin-features/ediscovery/06-content-logs-overview.md
- **Miro Sentinel 통합 가이드:** `01-microsoft-sentinel-integration.md`.

### Miro 개발자 문서

- **Enterprise API 시작하기:** `https://developers.miro.com/docs/getting-started-with-enterprise-api`.
- **OAuth 시작하기:** `https://developers.miro.com/docs/getting-started-with-oauth`.
- **OAuth 토큰 인증:** `https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens`.
- **감사 로그 API:** `https://developers.miro.com/reference/enterprise-get-audit-logs`.
- **콘텐츠 로그 API:** `https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch`.
- **API 참조:** `https://developers.miro.com/reference`.

### Microsoft Sentinel

- **Microsoft Sentinel 문서:** `https://docs.microsoft.com/azure/sentinel/`.
