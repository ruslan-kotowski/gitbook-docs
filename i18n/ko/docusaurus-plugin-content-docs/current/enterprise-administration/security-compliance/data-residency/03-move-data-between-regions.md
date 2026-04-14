---
title: 지역 간 데이터 이동
article_id: 23161744899986
translation_id: 23161744899986
locale: ko-kr
sidebar_position: 3
created_at: '2024-12-09T10:05:15Z'
updated_at: '2025-11-25T16:22:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '실행 가능한 사용자: 회사 관리자 해당 플랜: Enterprise 지원 플랫폼: 브라우저, 데스크톱'
---

Miro 고객은 현재 지역 외부에서 [데이터 레지던시](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md)가 필요할 수 있습니다. 유럽 연합(EU) 외부에서는 호주(AU)와 미국(US)에서 데이터 레지던시를 제공합니다.

## 지역 간 데이터 이동 옵션

데이터 레지던시 이동 프로세스는 크로스-리전 마이그레이션이라고 합니다. 조직을 새로운 지역으로 마이그레이션하려면, Miro는 다음 경로를 제공합니다:

- **수동 내보내기 및 가져오기**
  Miro 지원이 새로운 지역에 새 조직을 설정합니다. 회사 관리자가 모든 조직과 팀 설정을 재구성하고 사용자를 다시 초대합니다. 최종 사용자는 이전 지역에서 Miro 보드를 수동으로 다운로드하고 새 지역에 업로드합니다. 자세한 내용은 [지역 간 데이터 이동 - 수동 내보내기 및 가져오기](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md)를 참조하세요.
- **자동 데이터 마이그레이션**
  Miro 서비스와 함께 유료로 이용 가능하며, 조직 전체의 콘텐츠, 콘텐츠 계층 구조, 사용자, 설정을 포함하여 자동으로 마이그레이션합니다. 자세한 내용은 [지역 간 데이터 이동 – 자동 마이그레이션](../../canvas-25-admin-features/data-residency/05-move-data-between-regions-–-automated-migration.md)을 참조하세요.
  > ✏️ 자동 데이터 마이그레이션은 현재 [EKM 엔터프라이즈](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md)에는 제공되지 않습니다.

어떤 마이그레이션 경로가 최적인지 결정하려면 귀하의 전담 Miro 연락 담당자에게 문의하거나 [support@miro.com](mailto:support@miro.com)으로 이메일을 보내세요.

## 지역 간 데이터 이동 옵션 비교

다음 테이블은 지역 간 데이터 이동을 위한 자동 및 수동 옵션을 비교합니다:

|  | 자동화 | 수동 |
| --- | --- | --- |
| 비용 | Miro 서비스와의 유료 계약. | 추가 비용 없음. 회사 관리자와 최종 사용자가 보드 콘텐츠를 한 지역에서 다른 지역으로 이동합니다. |
| 범위 | 대부분의 조직 및 데이터를 아래 데이터를 포함하여 이동합니다. 포함된 데이터의 전체 목록은 [관리자 자동화 문서]를 참조하세요.  - 조직 데이터 - 사용자 프로필 - 팀 및 팀 설정 - 팀 멤버십 - 보드 - 감사 로그 - 데이터 등급 분류 - 콘텐츠 보안 설정 | 관리자는 조직 설정을 다시 구성하고, 팀을 재생성하며, 팀 설정을 적용하고, 사용자를 재초대하며, 라이선스를 지정하고, 앱과 통합을 재설치해야 합니다. 최종 사용자는 보드를 새 지역으로 수동으로 이동해야 합니다. |
| 소요 시간 | 대체로 8시간 미만의 다운타임이며, 조직과 데이터가 새로운 지역으로 이동됩니다. | 회사 관리자가 수동 설정을 얼마나 빨리 완료하고, 최종 사용자가 보드를 얼마나 빨리 이동하느냐에 따라 달라집니다. |
