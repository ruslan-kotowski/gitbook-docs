---
title: "Microsoft Purview \uBBFC\uAC10\uB3C4 \uB808\uC774\uBE14 \uAC00\uC838\uC624\
  \uAE30"
article_id: 22161930709010
translation_id: 22161930709010
locale: ko-kr
sidebar_position: 7
created_at: '2024-10-23T15:05:49Z'
updated_at: '2025-12-01T16:32:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Microsoft Purview를 사용하는 조직의 경우 여러 플랫폼 간의 일관된 데이터 보안 및 등급 분류 유지는 필수적입니다. Miro와 Microsoft Purview의 통합은 관리자가 Microsoft Purview에서 민감도 레이블을 직접 Miro로 가져올 수 있도록 하여 두 플랫폼 간의 분류 스키마 관리를 간소화합니다.

이 통합을 활용함으로써 조직은 Miro 내의 콘텐츠가 Microsoft Purview 프레임워크와 일관되게 분류되도록 할 수 있습니다. 이는 분류 레이블을 수동으로 다시 만들거나 업데이트하는 운영 부담을 줄일 뿐만 아니라 데이터 보안을 강화합니다. Miro의 데이터 보호 기능을 Microsoft Purview와 일치시킴으로써 관리자들은 전체 디지털 생태계에서 민감 정보를 자신 있게 관리할 수 있습니다.

## Microsoft Purview 민감도 레이블 Miro에 가져오기

Miro에 설정된 데이터 분류가 없다면, Microsoft Purview에서 기존 민감도 레이블을 직접 가져와 Miro에서 데이터 등급 분류를 쉽게 설정할 수 있습니다.

이미 데이터 분류가 설정된 경우, Microsoft Purview에서 민감도 레이블을 가져와 Miro에서 기존 분류 레이블로 전환할 수 있습니다.

## Microsoft Purview에서 민감도 레이블 가져오기

### 사전 준비사항

- Microsoft Purview에서 민감도 레이블을 다룰 수 있는 필요한 역할이나 권한을 가지고 있는지 확인하세요.
- 보드 분류 수준의 세부 정보를 알고 있어야 하며, 이를 기반으로 보안 및 거버넌스 요구 사항에 따라 구성해야 합니다.
- [민감한 콘텐츠 관리자](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) 역할을 가지고 있어야 합니다. 민감한 콘텐츠 관리자 역할을 요청하려면 회사 관리자에게 문의하세요.

:::note
참고:
- Microsoft의 문서에 따르면, Microsoft Purview의 민감도 레이블 업데이트는 모든 앱과 서비스에 적용되기까지 최대 24시간이 소요될 수 있습니다. 변경 사항이 발생할 충분한 시간을 두고 민감도 레이블을 가져오세요. MS Purview에서 수행한 업데이트가 24시간 후에도 적용되지 않는 경우, Microsoft Purview 지원 팀에 문의하세요.
- Microsoft Purview에서 Miro로 최대 50개의 민감도 레이블을 가져올 수 있습니다.
- 기존 데이터 분류 구성이 이미 있는 경우, Microsoft Purview에서 민감도 레이블을 가져와 Miro의 기존 분류 레이블로 전환할 수 있습니다. 자세한 내용은 [Miro의 기존 데이터 분류 구성에 Microsoft Purview의 민감도 레이블 가져오기](08-import-microsoft-purview-sensitivity-labels.md)를 참조하세요.
:::

Microsoft Purview에서 민감도 레이블을 가져와 Miro에서 데이터 분류를 설정하려면 다음 단계를 수행하세요:

1. [Miro 설정](https://miro.com/app/settings)으로 이동합니다.
2. 왼쪽 창에서 **Enterprise Guard** 아래 **데이터 등급 분류**를 클릭합니다.
3. **분류** 페이지의 화면 하단에서 **시작하기**를 클릭합니다.
4. **Microsoft Purview에서 가져오기** 상자에서 **로그인**을 클릭합니다.
5. 새 탭에 나타나는 **Microsoft 로그인** 페이지에서 Microsoft 신원 정보를 입력하고 로그인하세요. Microsoft 계정에 로그인하면 탭이 자동으로 닫힙니다.
6. **등급 분류** 페이지의 **Microsoft Purview에서 가져오기** 상자에서 **가져오기**를 클릭합니다.
   그러면 **Microsoft Purview에서 등급 분류 가져오기** 페이지가 나타납니다.
7. Miro에서 분류 수준으로 사용할 Microsoft Purview 민감도 레이블의 체크박스를 선택한 후, **다음**을 클릭합니다.

   > ✏️ Microsoft 문서에 따르면 Microsoft Purview의 민감도 레이블 업데이트는 모든 앱과 서비스에 복제되기까지 최대 24시간이 걸릴 수 있습니다. 변경 사항을 적용할 충분한 시간을 확보한 후 민감도 레이블을 가져오세요. MS Purview에서 수행한 업데이트가 24시간이 지나도 복제되지 않으면 Microsoft Purview 지원 팀에 문의하시기 바랍니다.
8. **분류 수준 정의** 페이지에서 기본 분류 수준을 할당하거나 가이드라인을 추가 링크를 편집할 수 있습니다. 다음 테이블은 각 필드와 그 설명을 나열합니다.

   |  |  |
   | --- | --- |
   | **필드** | **설명** |
   | **가이드라인 링크** | 이 URL은 분류 수준에 적용되는 정책이나 지침에 대한 자세한 정보를 제공합니다. 이 페이지는 조직 내 사용자가 보드 분류 수준에 대해 더 많이 알 수 있도록 하며, 이를 어떻게 활용할 수 있는지에 대한 정보를 제공합니다. URL은 다음 형식으로 제공해야 합니다: `http://www.example.com`  사용자가 보드 분류 배지 옆의 **자세히 알아보기** 아이콘(물음표 아이콘)을 클릭하면, 이 URL이 새 브라우저 탭에 로드됩니다. |
   | **새 보드의 기본 수준으로 사용** | 새 보드를 위한 기본 분류 수준으로 설정하려면 이 체크박스를 선택하세요. |
   | **미리보기** | 보드 분류 배지와 설명, 더 알아보기 아이콘의 미리보기가 표시됩니다. 미리보기는 사용자에게 보드에서 보이는 분류 배지를 정확히 보여줍니다. |
9. 분류 수준 구성을 저장하려면 **완료**를 클릭합니다.
10. **다음**을 클릭합니다. 구성이 저장되지만, [**영향 검토**](https://help.miro.com/hc/articles/16494764223378) 페이지에서 **게시**를 클릭한 후에만 적용됩니다.

    그런 다음 다음 단계를 진행할 수 있습니다:

    - [자동 분류 정의](09-define-auto-classification.md). 선택 사항입니다. 자동 분류를 나중에 정의하려면 **다음**을 클릭하세요.
    - [가드레일 정의](05-define-guardrails.md). 이 단계는 선택 사항입니다. 나중에 가드레일을 정의하려면 **다음**을 클릭하세요.
    - [영향 검토](https://help.miro.com/hc/articles/16494764223378). 이 단계는 워크플로의 마지막 단계이며 필수입니다.

## Microsoft Purview에서 Miro의 기존 등급 분류 설정으로 민감도 레이블 가져오기

### **사전 준비 사항**

- Microsoft Purview에서 민감도 레이블을 처리할 수 있는 필수 역할이나 권한이 있는지 확인하세요.
- 보안 및 관리 요구 사항에 따라 구성하려는 보드의 분류 수준에 대한 세부 정보를 알고 있어야 합니다.
- [민감한 콘텐츠 관리자 역할](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)이 있어야 합니다. 민감한 콘텐츠 관리자 역할을 요청하려면 회사 관리자에게 문의하세요.

:::note
참고:
- Microsoft 문서에 따르면, Microsoft Purview의 민감도 레이블 업데이트는 모든 앱과 서비스에 복제되기까지 최대 24시간이 걸릴 수 있습니다. 변경 사항이 적용되도록 충분한 시간을 두고 그 후 민감도 레이블을 가져와야 합니다. MS Purview에서 업데이트가 24시간 후에도 복제되지 않으면 Microsoft Purview 지원 팀에 문의하세요.
- Microsoft Purview에서 Miro로 최대 50개의 민감도 레이블을 가져올 수 있습니다.
- 보유 정책에 사용되는 분류 수준은 전송할 수 없습니다. 진행하기 전에 분류 수준이 어떤 보유 정책에도 사용되지 않도록 확인하세요. 자세한 내용은 [보유 정책 편집](../content-lifecycle-management/11-edit-retention-policy.md)을 참고하세요.
:::

Microsoft Purview에서 미로로 민감도 레이블을 가져오고 기존 분류 레이블로 전송/매핑하려면 다음 단계를 수행하세요:

1. [Miro 설정](https://miro.com/app/settings)으로 이동합니다.
2. 왼쪽 창에서 **Enterprise Guard** 아래 **데이터 분류**를 클릭합니다.
3. **분류** 페이지에서 화면 상단의 **가져오기**를 클릭합니다.
4. 이미 Microsoft에 로그인되어 있으면 이 단계를 건너뛰고 다음 단계로 진행하세요.
   Microsoft에 로그인되어 있지 않으면, **로그인**을 클릭하세요. 새 탭에 나타나는 **Microsoft 로그인** 페이지에서 Microsoft 신원 정보를 입력하고 로그인하세요. Microsoft 계정에 로그인하면 해당 탭이 자동으로 닫힙니다.
5. **Import from Microsoft Purview** 상자에서, Miro로 민감도 레이블을 가져오려면 **가져오기**를 클릭하세요. **Import classification from Microsoft Purview** 페이지가 나타납니다.
6. **수준 가져오기** 페이지에서 Miro에서 분류 수준으로 사용할 Microsoft Purview 민감도 레이블의 체크박스를 선택한 후 **다음**을 클릭합니다. **기존 수준 전송** 페이지가 나타납니다.

   > ✏️ Microsoft의 문서에 따르면, Microsoft Purview의 민감도 레이블 업데이트가 모든 앱과 서비스에 복제되기까지 최대 24시간이 소요될 수 있습니다. 변경 사항이 적용될 충분한 시간을 두고 나서 민감도 레이블을 가져오세요. MS Purview에서의 업데이트가 24시간 후에도 복제되지 않은 경우, Microsoft Purview 지원 팀에 문의하세요.
7. 콘텐츠가 올바르게 분류되도록 보장하려면, 기존 Miro 분류 수준을 Microsoft Purview에서 새로 가져온 수준으로 이전해야 합니다. 왼쪽에 나열된 수준은 기존 Miro 분류 수준이며, 오른쪽 드롭다운 목록에 나열된 것은 가져온 Microsoft Purview 민감도 레이블입니다. 완료한 후, **다음**을 클릭합니다.
8. **분류 수준 정의** 페이지에서 기본 분류 수준을 할당하거나 지침에 대한 링크를 추가하기 위해 분류 수준을 편집할 수 있습니다. 다음 표에는 각 필드와 해당 설명이 나와 있습니다.

   |  |  |
   | --- | --- |
   | **필드** | **설명** |
   | **지침 링크** | 이 분류 수준에 적용되는 정책 또는 지침에 대해 더 많은 정보를 제공하는 URL입니다. 이 페이지는 조직의 사용자가 보드 분류 수준 및 그에 따라 작업하는 방법에 대해 더 알아볼 수 있도록 정보를 제공합니다. URL은 다음과 같은 포맷으로 제공해야 합니다: `http://www.example.com`  사용자가 보드 분류 배지 옆에 있는 **자세히 알아보기** 아이콘(물음표 아이콘)을 클릭하면 이 URL이 새 브라우저 탭에서 로드됩니다. |
   | **새 보드의 기본 수준으로 사용** | 이 분류 수준을 모든 새 보드의 기본 분류로 설정하려면 이 체크박스를 선택하세요. |
   | **미리보기** | 보드 분류 배지의 설명과 추가 정보 아이콘과 함께 미리보기를 표시합니다. 미리보기는 사용자가 보드에서 본 배지가 정확히 어떻게 나타나는지 보여줍니다. |

   분류 수준 구성을 저장하려면 **완료**를 클릭하세요.
9. **다음**을 클릭합니다. 설정은 저장되지만, [**영향 검토**](https://help.miro.com/hc/articles/16494764223378) 페이지에서 **게시**를 클릭해야만 적용됩니다.

   그런 다음 다음 단계 중 하나를 진행할 수 있습니다:

   - [자동 등급 분류 정의](09-define-auto-classification.md). 이는 선택 사항입니다. 자동 등급 분류를 나중에 정의하고 싶다면, **다음**을 클릭하세요.
   - [가드레일 정의](05-define-guardrails.md). 선택 사항입니다. 나중에 가드레일을 정의하고자 한다면, **다음**을 클릭하세요.
   - [영향 검토](https://help.miro.com/hc/articles/16494764223378). 이는 워크플로의 마지막 단계이며 필수입니다.

## Microsoft Purview에서 연결 해제

Purview에 연결된 경우, 등급 분류 이름을 추가하거나 편집하고, 분류 수준을 업데이트하는 등의 작업을 할 수 없습니다. 이러한 작업을 수행하려면 Microsoft Purview에서 연결을 해제해야 합니다.  Purview와 연결을 해제하면 Microsoft Purview에서 Miro로의 업데이트 가져오기를 할 수 없습니다.

Microsoft Purview에서 연결을 해제하려면 다음 단계를 수행하세요:

1. [Miro 설정](https://miro.com/app/settings)으로 이동합니다.
2. 왼쪽 패널에서 **Enterprise Guard** 아래 **데이터 분류**를 클릭합니다.
3. **분류** 페이지에서 화면 상단의 **마지막 가져오기** 버튼을 클릭한 후, **Purview 연결 해제**를 클릭합니다.
