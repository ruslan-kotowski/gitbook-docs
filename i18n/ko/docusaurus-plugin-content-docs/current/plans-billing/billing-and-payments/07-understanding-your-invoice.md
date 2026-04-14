---
title: "\uCCAD\uAD6C\uC11C \uC774\uD574\uD558\uAE30"
article_id: 360021047619
translation_id: 360021047619
locale: ko-kr
sidebar_position: 7
created_at: '2021-04-13T06:37:58Z'
updated_at: '2025-10-10T07:52:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

귀하의 인보이스는 Stripe 결제 제공업체가 생성하며, 구매 내역, 회사 세부 정보, 영수증 또는 인보이스 번호, 사용된 결제 수단을 포함하고 있습니다. Miro 청구서에서 요금, 크레딧 및 조정의 표시 방법에 대해 자세히 알아보세요.

> **사용 가능 대상**:
> Starter 플랜, Business 플랜
> **관련 대상:** 관리자, 결제 관리자

## 청구서 찾기 위치

### 결제 이메일

결제 설정에서 모든 청구 관련 커뮤니케이션을 받을 이메일 주소를 지정할 수 있습니다. Stripe는 청구 이메일 주소로 영수증과 청구서를 발송합니다:

```
receipts+**********@stripe.com
invoice+statements+***************@stripe.com
```

### Miro 결제 설정

설정에서 Stripe 인보이스를 찾을 수 있습니다. [송장 찾기 및 다운로드 방법](01-how-to-find-and-download-an-invoice.md)에 대해 알아보세요.

## 청구서 요금 이해하기

다음 인보이스에는 라이선스를 추가하거나 제거하거나 플랜을 변경하는 등의 변경 사항이 표시됩니다. 플랜을 변경하면 결제 설정에 **갱신**이라는 새 인보이스가 생성됩니다.

### 청구서에 일할 계산된 요금 표시

라이선스를 추가하거나 제거할 때마다 명확성을 위해 인보이스에 두 가지 추가 정보가 포함됩니다: **남은 시간** 및 **사용하지 않은 시간**.

- **잔여 시간**은 최근 변경 후 업데이트된 라이선스 수를 반영합니다.
- **사용하지 않은 시간**은 변경하기 전의 라이선스 수를 표시합니다.

이해가 되지 않는 청구가 발생한 경우, [Managing extra licenses">추가 라이선스 관리 가이드](../../administration/user-management/04-manage-extra-licenses.md).

#### 라이선스 추가

현재 플랜에 포함된 것보다 더 많은 라이선스를 추가하는 경우, 청구 기간이 끝날 때까지 각 추가 라이선스에 대해 일할 계산된 금액이 청구됩니다. 예를 들어, 2021년 3월 23일에 라이선스를 추가하면, 일할 계산된 요금이 청구됩니다.

![charge_for_an_additional_license.jpg](../../../../../../docs/plans-billing/billing-and-payments/images/21017592958994_charge%20for%20an%20additional%20license.jpg)*라이선스 추가에 대한 비례 요금*

#### 라이선스 제거

라이선스 제거를 예약하신 경우, 이는 갱신일에 적용됩니다. 자세한 내용은 [Miro 월별 및 연간 결제](04-miro-billing.md)를 참조하세요.

#### 플랜 변경

Miro 플랜을 전환하거나 월간 구독에서 연간 구독으로 변경하면 다음 청구서의 비용이 조정됩니다. 이전 플랜에서 사용하지 않은 시간에 대한 크레딧은 새로운 청구서에 적용됩니다. 예를 들어, 사용하지 않은 월간 구독의 크레딧은 새로운 연간 구독에 사용할 수 있습니다.

![amount_for_switch_to_yearly.jpg](../../../../../../docs/plans-billing/billing-and-payments/images/21017605966098_amount%20for%20switch%20to%20yearly.jpg)
*월간 구독의 사용하지 않은 시간이 연간 구독에 적용됩니다*

## 자주 묻는 질문

**Miro 회사 주소는 무엇인가요?**

Miro의 모든 송장과 영수증에서 사업자 주소를 확인할 수 있습니다:
201 스피어 스트리트 스위트 1100 샌프란시스코, CA, 미국 94105

**Miro 부가세가 청구서에 표시되나요?**

Miro는 미국에 본사를 두고 있으며 네덜란드에서 One Stop Shop 제도를 통해 EU VAT에 등록되어 있습니다. Miro에는 공식적인 VAT ID 번호나 특정 청구서 요구사항이 없습니다.
