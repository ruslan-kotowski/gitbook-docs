---
title: 지역 간 데이터 이동 시 사용자 경험
article_id: 25075857856658
translation_id: 25075857856658
locale: ko-kr
sidebar_position: 4
created_at: '2025-03-04T08:51:38Z'
updated_at: '2025-05-09T08:47:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '실행 가능한 사용자: 전체 사용자 어떤 플랜: Enterprise 어떤 플랫폼: 브라우저, 데스크톱, 모바일'
---

이 문서에서는 [automated">자동화된](../../canvas-25-admin-features/data-residency/05-move-data-between-regions-–-automated-migration.md) 및 [수동 내보내기 및 가져오기](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md) 마이그레이션 모두에 대해 크로스 리전 데이터 마이그레이션 동안의 사용자 경험을 설명합니다.

## 자동화된 마이그레이션 중 사용자 경험 (베타)

다음 섹션에서는 지역 간 데이터 자동 이동 전, 중, 후의 예상 사항을 설명합니다.

### 자동화된 마이그레이션 이전

마이그레이션 2주 전, Enterprise 조직 내의 모든 사용자는 다음과 같은 알림을 받습니다.

- **제품 내 배너**
  마이그레이션 날짜 및 예상 기간이 로컬 시간대로 표시됩니다
- **이메일 알림**
  Enterprise 조직의 모든 사용자에게 예정된 유지 보수 작업을 안내합니다.

:::note
여러 Miro 계정의 멤버인 경우, 마이그레이션 중에도 다른 계정에 계속 접근할 수 있습니다.
:::

### 자동화된 마이그레이션 중

자동 마이그레이션에는 약 8시간의 다운타임이 필요합니다.

자동화된 마이그레이션 중에는 보드, 팀, 설정을 포함하여 Enterprise 조직 데이터를 액세스할 수 없습니다.

Miro 대시보드는 조직의 데이터 마이그레이션이 진행 중임을 알리는 알림을 표시합니다. 마이그레이션 과정 중에 조직 보드, 팀 또는 설정에 액세스할 수 없습니다.

:::tip
여러 조직의 멤버인 경우, 대시보드에서 다른 조직으로 전환하여 Miro를 계속 사용할 수 있습니다.
:::

### 자동 마이그레이션 후

마이그레이션이 성공적으로 완료되면 확인 이메일을 받게 됩니다. Miro 대시보드에 성공적인 마이그레이션을 확인하는 메시지가 나타납니다.

마이그레이션이 실패하면 이메일 알림을 받게 됩니다. [miro.com](https://miro.com)에서 로그인하여 계속해서 EU 지역에서 Miro를 사용할 수 있습니다.

### 자동 마이그레이션 후 보드 리디렉션

이전에 북마크한 보드는 자동으로 새로운 지역으로 리디렉션되며 업데이트된 URL을 사용합니다.

## 수동 내보내기 및 가져오기 동안의 사용자 경험

사용자는 소스 지역에서 보드 백업을 수동으로 내보내고, 타겟 지역에 백업을 가져와야 합니다.

**추가 정보:** [지역 간 데이터 이동 – 수동 내보내기 및 가져오기](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md)를 참조하세요.

## 지역 간 협업

Miro의 사용자는 지역적입니다. 다른 지역의 조직 사용자와 협업하려면 각 지역에 해당하는 사용자 프로필을 보유해야 합니다.

예를 들어, EU 지역 사용자이고 AU 지역 조직의 사용자와 협업하려면, [au.miro.com](https://au.miro.com/)에서 별도의 사용자 프로필을 만들어야 합니다.
