---
title: Mural에서 Miro로 가져오기 가이드 – PDF
article_id: 22856050009362
translation_id: 22856050009362
locale: ko-kr
sidebar_position: 2
created_at: '2024-11-25T14:36:20Z'
updated_at: '2026-01-19T14:43:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  roles: 편집 권한이 있는 사용자
  plans: business, education, enterprise, starter
  platforms: 브라우저, 데스크톱
---

기존 Mural 보드를 Mural에서 PDF 파일로 내보낸 후, 그러한 PDF를 Miro로 가져와 사용할 수 있습니다. 이 문서는 PDF 가져오기를 통해 최상의 결과를 얻기 위한 가이드를 제공하고, 가져오기 절차를 설명하며, 이 방법을 사용하여 다양한 Mural 요소가 Miro로 가져올 때 기대할 수 있는 내용을 설명합니다.

PDF 가져오기 방법은 복사-붙여넣기 또는 API 기반 가져오기를 통해 잘 전달되지 않는 콘텐츠에 특히 효과적입니다. Miro의 PDF 가져오기는 Mural PDF 내의 도형과 그 좌표를 분석하여 원래의 레이아웃을 재구성하려고 합니다. 예를 들어, 교차하는 선은 테이블 구조로 해석될 수 있습니다.

일부 객체는 Miro로 가져온 후 다르게 나타날 수 있으며, 정확한 스타일링이나 레이아웃은 Miro 내에서 수동으로 조정하거나 다시 생성해야 할 수 있습니다. 일반적으로 복잡한 스타일링이 덜한 단순한 콘텐츠는 더 정확한 가져오기 결과를 가져오게 됩니다.

## Mural에서 가져오기 지침

PDF로 Mural 콘텐츠를 가져올 때 최상의 결과를 얻으려면 가져오기 도구가 작동하는 방식과 어떤 콘텐츠가 가장 효과적으로 전송되는지를 이해하면 도움이 됩니다. PDF 가져오기 도구는 주로 기본 도형과 선을 매칭합니다.

:::note
**참고:** Miro로 콘텐츠를 가져오기 위해서는 Mural 콘텐츠가 Mural의 제한된 무료 라이선스 하에 있어야 합니다.
:::

Mural 요소 간의 명확한 간격은 Miro 가져오기 도구가 콘텐츠를 더 정확하게 분석할 수 있게 해줍니다. 많은 요소가 서로 가까이 몰려 있는 Mural 보드는 혼합되거나 덜 정확한 가져오기 결과를 낼 수 있습니다.

가장 높은 충실도로 가져오려면 PDF로 전환할 때 Mural 콘텐츠에 **다음 속성이 포함되지 않도록** 확인하세요. 이러한 속성은 잘 전환되지 않을 수 있습니다:

- 사용자 지정 글꼴
- 기본 도형을 변형하는 복잡한 스타일(예: 많이 둥글린 사각형 모서리, 독특하게 구부러진 화살표)
- 중첩된 여러 도형과 선
- 회전된 요소

:::tip
**팁:** Mural 콘텐츠의 정확한 스타일, 복잡한 레이아웃, 혹은 정확한 좌표를 유지하려면 가장 신뢰할 수 있는 방법은 Mural 콘텐츠를 정적 이미지 (예: PNG, JPG)로 내보낸 후, 해당 이미지를 Miro 보드로 가져오는 것입니다.
:::

## Mural 보드를 PDF로 Miro에 가져오기

이 섹션에서는 PDF 가져오기 기능을 사용하여 Mural 콘텐츠를 Miro로 가져오는 방법을 설명합니다.

### PDF 가져오기 전제 조건

가져오기 프로세스를 시작하기 전에 다음 전제 조건을 충족해야 합니다.

- Mural에서 원본 보드를 PDF로 내보내기 위해 편집 액세스 권한이 있어야 합니다.
- 콘텐츠를 가져오려는 Miro의 대상 보드에 편집 액세스 권한이 있어야 합니다.
- 이미 Mural 보드를 PDF 파일로 다운로드해야 합니다.

**추가 정보:** Mural에서 내보내기 관련 지침은 Mural의 문서 [내보내기 및 다운로드](https://support.mural.co/s/article/export-and-download-your-mural-s-content) (외부 링크)를 참조하세요.

### PDF 가져오기

Mural PDF 파일을 Miro에 가져오려면 다음 단계를 따르세요:

1. Miro 대시보드에서 **+ 새로 만들기** 버튼을 클릭합니다.
2. 드롭다운 메뉴에서 **가져오기**를 선택한 다음, **Mural에서 가져오기**를 선택합니다.
   **Mural에서 보드 가져오기** 모달 대화 상자가 열립니다.
3. 모달의 화면 안내에 따라 진행하세요. Mural PDF 파일을 업로드하라는 프롬프트가 표시됩니다.
   가져온 콘텐츠를 특정 Miro 스페이스에 추가하도록 선택할 수 있습니다. 스페이스를 지정하지 않으면 가져온 콘텐츠는 기본 팀 영역에 추가됩니다.
4. 파일을 업로드하고 옵션을 설정한 후 **보드 가져오기**를 선택하세요.
   가져오기 프로세스가 시작됩니다. 가져오기가 완료되면 Miro에서 이메일 알림을 받게 됩니다.

이제 Mural 콘텐츠를 PDF를 통해 Miro로 성공적으로 가져왔습니다.

## 예상 결과

Mural 객체가 PDF를 통해 Miro로 가져오면 플랫폼 간의 차이와 PDF 변환의 특성 때문에 스타일과 형식에서 몇 가지 변형이 발생할 수 있습니다. 이 섹션에서는 일반적인 Mural 객체에 대한 전형적인 가져오기 결과를 설명하고 몇 가지 모범 사례를 제공합니다.

### 지역

Mural 내보내기에서 가장 바깥쪽 지역은 일반적으로 Miro 프레임으로 가져옵니다. 다른 내부 지역은 보통 Miro의 일반적인 도형으로 가져옵니다.

:::note
**참고:** 중첩된 지역(지역 내에 또 다른 지역)이 가져오기 중에 잘못 식별되거나 구조화될 수 있습니다. PDF 가져오기 도구는 위젯의 상하관계를 시각적 좌표에 의존하여 결정하는데, 이 과정에서 복잡한 중첩으로 인해 모호해질 수 있습니다.
:::

### 커넥터

PDF 임포터는 주로 실선 연결선을 인식하고 재생성합니다. 점선이나 파선 연결선은 예상한 대로 임포트되지 않을 수 있습니다.

만약 Mural의 연결선에 텍스트가 직접적으로 라인 위에 포함되어 있다면, PDF 임포터는 이를 텍스트 객체가 근처에 있는 두 개의 개별적인 선으로 해석할 수 있으며, 이는 단일 텍스트 포함 연결선과는 다르게 임포트될 수 있습니다.

![A connector with text that the PDF importer breaks into two lines.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*PDF 임포터가 두 개의 선으로 "분리"한 텍스트 포함 연결선.*

### 그림

Mural에서의 손 그림 요소들은 일반적으로 Miro에서 선이나 곡선 집합체로 임포트됩니다.

복잡한 그림의 경우, PDF 가져오기가 의도하지 않은 연결선으로 인식하여 그림의 일부를 인근 또는 겹치는 객체와 잘못 연결할 수 있습니다.

![A drawing may import as linked to a nearby or overlapping object.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*그림이 인근 또는 겹치는 객체와 연결되어 가져올 수 있습니다.*

### GIF

PDF 가져오기는 Mural에서 GIF를 인식하지만, 정지 이미지(주로 GIF의 첫 번째 프레임)로 가져옵니다.

:::note
**참고:** PDF 파일 형식 자체는 애니메이션 GIF를 지원하지 않습니다. 이는 PDF의 제한 사항이며, Miro 가져오기의 문제가 아닙니다.
:::

### 이미지

Mural 보드에서 가져온 이미지는 Miro에서 이미지로 가져옵니다. 그러나 Mural과 Miro의 좌표 시스템 차이와 PDF 변환 과정 때문에 보드 내의 정확한 위치가 약간 변경될 수 있습니다.

### 목록

Mural의 목록(번호 목록 및 글머리 기호 목록)은 일반적으로 Miro에서도 목록으로 가져옵니다. 최상의 결과를 얻으려면 Mural에서 목록에 기본 표시(정렬된 목록의 표준 번호와 정렬되지 않은 목록의 기본 글머리 기호)를 사용하세요.

![A numbered list, and a bulleted list, with default markers, numerals and bullets respectively.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*번호 목록과 글머리 기호 목록이 기본 번호와 글머리 기호가 적용된 예입니다.*

### 마인드맵

PDF 가져오기 방법은 하나의 루트 노드와 모든 노드에 보이는 테두리가 있는 마인드맵에 가장 적합합니다. 루트가 여러 개이거나 테두리가 숨겨진 복잡한 마인드맵은 정확하게 가져오기 어려울 수 있습니다.

![A basic Mind map is easier to import as PDF.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*기본적인 마인드맵은 PDF로 가져오기 더 수월합니다*

PDF 가져오기는 종종 많은 선과 객체가 밀집되어 있는 마인드맵을 정확히 해석하기 어렵습니다. 만약 PDF 마인드맵이 제대로 가져와지지 않는다면, Mural에서 Miro로 마인드맵 콘텐츠를 직접 복사하여 붙여넣기를 시도해 보세요. 복사-붙여넣기 방법은 Miro에서 스타일과 크기를 수동으로 조정해야 할 수도 있지만, 일부 마인드맵의 경우 전체적인 구조의 충실도가 더 높을 수 있습니다.

### 도형

PDF 가져오기는 기본 Mural 도형(예: 사각형, 타원, 삼각형)을 편집 가능한 Miro 도형으로 가져오도록 설계되었습니다.

![Only basic shapes import as editable content.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*기본 도형만 편집 가능한 콘텐츠로 가져옵니다*

Mural에서 가져온 고급, 맞춤형 또는 스타일이 잘 적용된 도형 및 회전된 도형은 편집 가능한 Miro 도형이 아닌 정적 이미지로 가져올 수 있습니다.

### 스티커 메모

일반적인 Mural 스티커 메모는 대개 Miro 스티커 메모로 가져옵니다. 가장 높은 퀄리티를 유지하려면 기본 종횡비(예: 3x3 또는 5x3 일반 크기)의 Mural 스티커 메모를 사용하세요.

![Sticky notes with the default size can be easily imported.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*기본 크기의 스티커 메모는 쉽게 가져올 수 있습니다*

:::note
**참고:** Mural에서 가져온 원형 스티커 메모는 Miro에서 기본 원형 스티커 메모 객체가 없으므로 일반 도형으로 가져옵니다.
:::

스티커 메모가 겹치거나 회전된 경우, 높은 정확도로 가져오지 못할 수 있으며, Miro에서 수동으로 위치를 조정해야 할 수 있습니다.

![Import results vary for rotated sticky notes, and sticky notes that overlap.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*회전된 스티커 메모와 겹쳐진 스티커 메모의 가져오기 결과는 다를 수 있습니다.*

### 테이블

분명한 그리드 라인이 있는 단순한 Mural 테이블은 일반적으로 높은 정확도로 Miro 테이블로 가져오거나 테이블 구조를 형성하는 도형과 선들의 모음으로 불러올 수 있습니다.

복잡한 기하학적 구조의 테이블은 분리된 선과 텍스트 상자의 시리즈로 가져올 수 있습니다. 테이블을 가져올 때 최상의 결과를 얻으려면 Mural 내보내기의 테이블에 다음 속성이 **없도록** 하세요:

- 병합된 셀
- 보이지 않거나 숨겨진 테두리
- 셀이나 테이블 테두리의 둥근 모서리

![Complex tables do not import with high fidelity.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*복잡한 테이블은 높은 완성도로 가져올 수 없습니다.*

### 텍스트

Mural의 텍스트 객체는 일반적으로 Miro에서 편집 가능한 텍스트로 가져와지며, 이는 종종 원래 Mural 텍스트 상자에 대응하는 단일 텍스트 블록이나 도형 안에 위치합니다.

텍스트를 가장 높은 수준으로 가져오려면 Mural에서 기본 글꼴과 표준 여백을 사용하는 것이 좋습니다.

:::note
**참고:** 가져온 후 글꼴 크기가 달라질 수 있으며 Miro에서 수동으로 조정해야 할 수도 있습니다.
:::

커스텀 글꼴이나 복잡한 스타일링(예: 하나의 텍스트 박스 내 여러 스타일 사용)이 있는 텍스트는 PDF 가져오기 기능에 의해 여러 작은 텍스트 블록으로 나뉠 수 있습니다.
