---
title: Lucidspark 보드를 Miro로 가져오기
article_id: 9549014537490
translation_id: 9549014537490
locale: ko-kr
sidebar_position: 7
created_at: '2023-01-12T09:05:07Z'
updated_at: '2026-01-19T14:30:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: '사람: Lucidspark 및 Miro 보드에 대한 편집 권한이 있는 모든 사용자 플랜: Free, Starter, Business,
    Education, 그리고 Enterprise 플랫폼: 브라우저, 데스크톱'
---

Miro로 Lucidspark 콘텐츠를 원활하게 마이그레이션하여 더욱 강력한 협업 경험을 즐기세요. 이 가이드는 보드를 가져오는 방법과 프로세스 중에 예상할 수 있는 내용을 설명합니다.

> **경고:** 가져온 콘텐츠 편집은 단방향입니다. Miro에서 변경한 내용은 Lucidspark로 동기화되지 않습니다.

> **참고:** Free 또는 Restricted 라이선스 하에 있는 Lucidspark 보드를 마이그레이션 할 수 있습니다.

## PDF 내보내기를 통한 Lucidspark 보드 가져오기 방법

PDF 내보내기 방법을 사용하여 Lucidspark 보드를 Miro로 가져오려면 다음 단계를 따르세요:

1. **Lucidspark**에서 Miro로 가져오고자 하는 콘텐츠를 PDF로 내보내기 해야 합니다.
2. Miro **홈** 대시보드에서 **+ 새로 만들기**를 클릭하세요.
3. **가져오기**를 선택한 후 **Lucidspark에서 가져오기**를 선택하세요.
   **Lucidspark에서 가져오기** 모달이 열립니다. 여러 개의 Lucidspark PDF를 일괄 가져오기가 가능합니다.
4. 모달에 제공된 화면의 지시를 따르세요.
5. **보드 가져오기**를 선택하세요.
6. 가져온 콘텐츠를 검토하고 필요한 조정을 하세요. Lucidspark와 Miro는 유사한 기능을 제공하지만, 스타일과 서식에서 차이가 있을 수 있습니다. 개체가 어떻게 변환되는지에 대한 가이드를 보려면 [Miro에서 Lucidspark 객체가 나타나는 방식 (일괄 PDF 가져오기 방법)](#lucidspark-object-mapping-bulk-import)를 참조하세요.

## 대안 방법: 콘텐츠 복사 및 붙여넣기

더 적은 양의 콘텐츠를 빠르게 처리하려면, Lucidspark 보드에서 개체를 직접 복사해 Miro 보드에 붙여넣을 수 있습니다.

> **참고:** Lucidspark와 Miro 보드에 편집 권한이 있는 사용자는 Lucidspark에서 콘텐츠를 복사해 Miro로 붙여넣을 수 있습니다. 이 방법으로 객체가 어떻게 변환되는지에 대한 자세한 내용은 [Lucidspark 객체가 Miro에서 어떻게 나타나는지 (복사/붙여넣기 방법)](#lucidspark-object-mapping-copy-paste)을 참조하세요.

## Lucidspark 객체가 Miro에서 어떻게 나타나는지 (복사/붙여넣기 방법)

이 표는 Lucidspark에서 콘텐츠를 직접 복사하고 Miro에 붙여넣을 때 객체가 어떻게 변환되는지를 종합적으로 비교합니다.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Azure 카드 | Azure 카드는 Miro 카드로 마이그레이션됩니다: 1. Miro에서 Azure 통합을 설정하세요. 2. Miro 카드를 [Azure 카드](../../integrations-apps/microsoft/03-azure-cards.md)로 변환합니다. |
| 공동 작업자와 공유 | 🟠 수동으로 재생성할 수 있습니다 |
| 댓글 | 🟠 수동으로 재생성할 수 있습니다 |
| 커넥터 및 구분 기호 | 커넥터 |
| 컨테이너 | 도형 |
| 파일 및 URL에서 가져온 문서 | 🟠 수동으로 재생성 가능 |
| 문서 URL (PDF) | 임베드된 문서 |
| 그리기 | 이미지 |
| 동적 테이블 | 테이블 |
| 이모티콘 | 이미지 |
| 프레임 | 프레임 |
| 툴바에서 GIF | 이미지 |
| 파일에서 GIF | 이미지 |
| URL에서 GIF | GIF |
| 이미지 | 이미지 |
| Jira 카드 | Jira 카드는 Miro 카드로 마이그레이션됩니다:  1. Miro에서 Jira 통합 설정 2. Miro 카드를 [Jira 카드](../../integrations-apps/atlassian/03-jira-cards.md)로 변환하세요. |
| Lucid 카드 | 카드 |
| 마인드맵 | 마인드맵 |
| 도형 | 도형 |
| 스티커 메모 | 스티커 메모 |
| 테이블 | 테이블 |
| 텍스트 | 텍스트 |
| 타임라인 | 🟠 수동으로 재생성 가능 |
| 동영상 및 기타 URL | 미리 보기 |

## Lucidspark 객체가 Miro에서 어떻게 나타나는지 (일괄 PDF 가져오기 방법)

이 표는 콘텐츠를 PDF로 일괄 가져온 후 Lucidspark와 Miro 간의 객체 비교를 포괄적으로 제공합니다.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Azure 카드 | 이미지 |
| 공동 작업자 및 공유 | 🟠 수동으로 재생성 가능 |
| 댓글 | 🟠 수동으로 재생성 가능 |
| 연결선 및 구분선 | 연결선 |
| 컨테이너 | 도형 |
| 문서 | 🟠 수동으로 재생성 가능 |
| 그리기 | 선 |
| 동적 테이블 | 도형과 연결선 |
| 이모티콘 | 이미지 |
| 프레임 | 프레임과 도형 |
| GIF | 이미지 |
| 이미지 | 이미지 |
| Jira 카드 | 도형 |
| Lucid 카드 | 도형 |
| 마인드맵 | 도형과 연결선 |
| 도형 | 도형 |
| 스티커 메모 | 스티커 메모 |
| 테이블 | 테이블/도형과 연결선 |
| 텍스트 | 텍스트 |
| 타임라인 | 도형 및 연결선 |
| 동영상 및 기타 URL | 🟠 수동으로 재구성할 수 있음 |

## 가져오기 제한 사항

Lucidspark과 Miro는 유사한 기능을 제공하지만, 가져올 때 다음의 차이점과 제한 사항에 유의하십시오:

- Miro 텍스트 박스에는 스페이스를 포함하여 최대 6,000자까지 수용할 수 있습니다. 그 이상의 텍스트는 잘라내기됩니다.
- 색상과 스타일은 Miro에서 가장 가까운 매치로 매핑됩니다.
- Lucidspark에서의 투명도 값은 가져오기 시 정확하게 추출되지 않습니다.
- Miro 스티커 메모는 회전, 색상 팔레트 조정, 또는 Lucidspark에서 적용된 텍스트 글머리 기호를 지원하지 않습니다.

## 도움 받기

> **참고:** Lucidspark 마이그레이션과 관련된 추가 질문 및 지원은 [Miro 지원](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)에 연락하거나 직접 Miro 고객 성공 매니저에게 문의하세요.
