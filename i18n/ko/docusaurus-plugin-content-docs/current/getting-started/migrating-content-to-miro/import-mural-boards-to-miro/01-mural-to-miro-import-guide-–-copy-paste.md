---
title: Mural에서 Miro로 복사/붙여넣기 가이드
article_id: 22957521683986
translation_id: 22957521683986
locale: ko-kr
sidebar_position: 1
created_at: '2024-11-29T13:36:36Z'
updated_at: '2025-11-25T15:49:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: '사용자: 편집 권한이 있는 사용자 플랜: Free, Starter, Business, Enterprise, Education 플랫폼:
    브라우저, 데스크톱, 모바일'
---

Mural 보드의 콘텐츠를 복사-붙여넣기 방법을 사용해 Miro로 전송할 수 있습니다. 이 가이드는 이 가져오기 방법에 대한 모범 사례를 제공하고, 단계별 프로세스를 설명하며, Miro에 다양한 객체를 붙여넣었을 때의 모양과 동작에 관해 기대할 수 있는 것들을 자세히 설명합니다.

## Mural에서 가져오기 지침

이 지침을 따르면 Mural에서 Miro로 콘텐츠를 옮길 때 최상의 결과를 얻을 수 있습니다.

구조화된 데이터의 경우, Mural 마인드맵과 같은 데이터를 복사-붙여넣기 방식으로 처리하면 요소 간의 연결이 끊어지지 않아야 합니다.

> Miro로 콘텐츠를 가져오기 위해서는, Mural의 콘텐츠가 제한된 무료 라이선스나 Full 라이선스를 가지고 있어야 합니다.

[Mural에서 Miro로 가져오기 가이드(PDF)](02-mural-to-miro-import-guide-–-pdf.md)에서 지원하지 않는 개별 위젯을 가져오거나 PDF 방법으로 가져올 때 높은 정확도로 가져오지 못하는 위젯의 경우, 복사-붙여넣기 방법을 사용하는 것도 추천합니다.

복사-붙여넣기 방법에는 일부 제한 사항이 있습니다: URL을 통해 연결된 것이 아닌 Mural에 처음 업로드된 특정 스타일 속성과 이미지가 클립보드에 복사되지 않으므로 Miro로 전송되지 않습니다.

## Mural 콘텐츠를 Miro로 복사하여 붙여넣기

다음 절차는 Mural 보드에서 콘텐츠를 복사하여 Miro 보드에 붙여넣는 방법을 설명합니다.

**조건**

Mural의 원본 보드와 Miro의 대상 보드에 모두 편집 권한이 있는지 확인하세요.

Mural 보드에서 콘텐츠를 복사하여 Miro 보드에 붙여넣기:

1. Mural에서 복사하려는 객체를 선택하세요.
   > 💡 보드의 모든 오브젝트를 선택하려면 **Ctrl+A** (Windows) 또는 **Cmd+A** (Mac) 키보드 단축키를 사용하세요.
2. 선택한 객체를 복사하려면 키보드 단축키 **Ctrl+C** (Windows) 또는 **Cmd+C** (Mac)를 사용하세요.
   Mural 객체가 이제 클립보드에 복사되었습니다.
3. Miro에서 콘텐츠를 붙여넣고자 하는 보드를 엽니다. 키보드 단축키 **Ctrl+V** (Windows) 또는 **Cmd+V** (Mac)을 사용해 붙여넣으세요.

   Mural에서 Miro로 콘텐츠를 성공적으로 복사하여 붙여넣었습니다.
   > ✏️ Mural에서 복사한 콘텐츠는 Miro에서 일부 수동 조정이 필요할 수 있습니다. 붙여넣기 후 스타일이나 서식이 다르게 나타날 수 있습니다.

## 붙여넣기 후 객체 외형

Mural 객체는 일반적으로 Miro로 페이스트될 때 원래 상태에서 약간의 변화가 발생합니다. 이 섹션에서는 일반적인 객체에 대한 기대 결과를 설명하고, 적용 가능한 모범 사례를 제공합니다.

### 영역

Mural에서 Miro로 복사하여 붙여넣기 할 때 영역이 프레임과 도형으로 변경됩니다.

Mural의 영역을 투명도 100%로 설정하면 Miro에 붙여넣었을 때 투명하지만 눈에 보이는 테두리가 나타납니다. Mural 영역에 제목이 있으면, 이 제목은 Miro에서 프레임 제목으로 나타나고 행동합니다.

![제목과 100% 투명한 배경 및 테두리를 가진 Mural 영역.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*제목과 100% 투명한 배경 및 테두리가 있는 Mural 프리폼 영역*

![Mural에서 Miro로 붙여넣기 된 영역.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mural에서 Miro로 복사된 영역*

### 커넥터

Mural의 커넥터가 Miro 커넥터로 복사됩니다.

연결선 레이블의 경우 수직 및 수평 위치가 Miro에 가운데 맞춤으로 붙여넣어집니다. Miro는 커넥터 레이블에 대해 중앙 위치만 지원합니다.

Miro는 *실선*, *점선*, *대시 선*을 지원합니다. 추가적으로 Mural에는 *점선* 커넥터 유형이 포함됩니다. Miro의 맵 유형은 Mural에서 붙여넣으면 다음과 같이 매핑됩니다: *solid*는 *solid*로, Mural의 *loosely dashed* 유형은 Miro의 *dashed* 유형으로 매핑됩니다. 다른 직접적인 일치 (점으로 연결된)를 비롯하여 모두 유지됩니다.

Miro는 각 유형의 Mural 커넥터 곡선을 지원하지만, Miro에서의 외형은 약간 다를 수 있습니다.

![Mural 커넥터 곡선.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mural 커넥터 곡선*

![Miro 커넥터 곡선.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Miro 커넥터 곡선*

### GIF 및 이미지

원래 URL에서 Mural에 추가된 GIF와 이미지는 Miro에 복사해 붙여넣을 수 있습니다.

:::note
장치에서 직접 업로드되거나 Mural의 툴바에서 추가된 GIF 또는 이미지는 이 방법으로 Miro에 복사 및 붙여넣기할 수 없습니다.
:::

### 마인드맵

Mural에서 마인드맵을 복사하여 Miro 마인드맵으로 붙여넣기, 루트 노드와 각 하위 노드 및 그들의 텍스트 포함.

루트 노드의 스타일은 대부분 유지됩니다. 그러나 도형의 반지름은 다를 수 있으며, 텍스트 글꼴 크기는 Mural에서 Miro로 유지되지 않습니다.

Mural의 하위 노드가 Miro의 텍스트 노드로 붙여넣기 되며, 스타일링은 유지되지 않습니다.

마인드맵의 커넥터 색상과 두께도 달라질 수 있습니다.

![Mural에서 복사한 마인드맵](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)
*Mural에서 마인드맵 복사됨*

![Mural에서 Miro로 복사한 마인드맵.](https://help.miro.com/hc/article_attachments/27740802360210)

*마인드맵 복사/붙여넣기 완료*

마인드맵에 여러 수준의 노드가 있는 Mural의 경우 Miro에 붙여넣을 때 노드 순서가 변경될 수 있습니다.

![Mural에서 여러 노드 레벨로 구성된 마인드맵.](https://help.miro.com/hc/article_attachments/27740802361490)

*노드 레벨이 여러 개인 Mural의 마인드맵*

![Mural에서 Miro로 복사한 여러 노드 레벨이 있는 마인드맵입니다.](https://help.miro.com/hc/article_attachments/27740802363154)

*Mural에서 Miro로 복사된 여러 노드 레벨의 마인드맵*

:::tip
Mural에서 Miro로 복사한 마인드맵은 원래의 크기가 변할 수 있습니다. 마인드맵을 붙여넣은 후 크기를 조정하려면 Miro 보드에서 수동으로 늘릴 수 있습니다.
:::

### 도형

Mural에서 복사한 도형은 일반적으로 Miro 도형으로 붙여넣기 됩니다. Miro는 Mural의 대부분의 도형을 직접 지원합니다.

그러나 Mural에는 Miro에서 직접적인 동등한 형태가 없는 16가지 특정 도형이 포함되어 있습니다. 이 도형들은 Miro에 사각형으로 붙여넣어집니다.

![Mural에서 Miro로 복사하여 붙여 넣을 때 사각형으로 변하는 모든 16개의 도형입니다.](https://help.miro.com/hc/article_attachments/27740802365074)

*Mural에서 Miro로 복사하여 붙여넣기할 때 직사각형으로 변하는 16개의 도형*

### 스티커 메모

Mural의 스티커 메모를 Miro 스티커 메모로 붙여넣습니다.

Miro는 스티커 메모 색상 및 불투명도를 Miro에서 가능한 가장 가까운 매치로 매핑합니다.

Mural 스티커 메모를 Miro로 복사 붙여넣기 할 때 다음과 같은 차이점도 나타날 수 있습니다:

- Mural에서 가져온 원형 스티커 메모가 Miro에서는 정사각형 스티커 메모로 붙여넣어집니다.
- 스티커 메모 내의 목록은 인터랙티브 목록으로 보존되지 않지만, 각각의 항목은 Miro 스티커 메모 안에서 개별적인 줄에 나타납니다.
- 텍스트 글꼴 크기는 유지되지 않으며, Miro의 스티커 메모는 콘텐츠와 스티커 메모 크기에 따라 글꼴 크기를 자동으로 설정합니다.
- 무럴에서 스티커 메모에 적용된 회전은 붙여넣기 시 보존되지 않습니다.

![Mural에 복사된 스티커 메모.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*스티커 메모가 Mural에 복사되었습니다*

![Mural에서 Miro로 복사한 스티커 메모.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Miro에 복사된 스티커 메모*

### 테이블

Mural에서 테이블을 Miro 테이블로 붙여넣기.

Mural에서 Miro로 테이블을 복사할 때 다음과 같은 차이점이 나타날 수 있습니다. 이 항목들 각각에 대해, Miro에 붙여넣은 후 수동으로 기본 설정을 복원할 수 있습니다.

- Mural에서 객체(영역, 도형, 이미지 등) 위에 위치한 테이블은 Miro에 붙여넣으면 해당 객체 뒤에 일부가 숨길 수 있습니다. 레이어를 조정해야 할 수 있습니다 (맨 앞으로 가져오기).
- 테두리 색상은 무시되며 테두리는 회색으로 붙여넣기가 됩니다.
- 배경 투명도는 무시됩니다. Mural의 투명한 셀은 Miro에서 흰색 셀로 붙여넣어집니다. 그러나 배경색 자체가 (투명하지 않은 경우) 일반적으로 유지됩니다.
- 텍스트 글꼴 패밀리는 무시되며, 텍스트는 Miro의 기본 테이블 글꼴(RobertPro)로 붙여넣기가 됩니다.
- 테이블 셀 내에서는 굵게 또는 기울임 같은 인라인 텍스트 서식이 무시됩니다.

![Mural에 복사된 혼합 서식이 있는 표.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mural에 복사된 혼합 서식 테이블*

![Mural에서 Miro로 혼합 서식을 복사한 표.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Miro에 복사한 표를 붙여넣었을 때 서식이 섞여 표시될 수 있습니다*

### 텍스트

Mural의 텍스트 오브젝트가 Miro의 텍스트 오브젝트로 붙여넣어집니다. 원래 Mural 글꼴 모음이 보존되지 않습니다. Miro는 Mural 글꼴 패밀리를 Miro에서 사용 가능한 가장 유사한 글꼴로 매핑하고, Miro 보드에서 최적의 결과를 얻기 위해 붙여넣은 텍스트의 크기를 조정합니다.
