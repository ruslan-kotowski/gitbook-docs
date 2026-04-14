---
title: "\u8ACB\u6C42\u66F8\u306B\u3064\u3044\u3066"
article_id: 360021047619
translation_id: 360021047619
locale: ja
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

請求書は、当社の請求プロバイダーである Stripe によって発行され、購入内容、会社情報、領収書または請求書番号、および使用した支払い方法の詳細が含まれています。Miro の請求書にどのように料金、クレジット、および調整が表示されるかについての詳細をご覧ください。

> **対象**：Starter プラン、Business プラン
> **対象プラン：**管理者、支払い管理者

## 請求書の見つけ方

### お支払い関連のメール

[支払い設定] で、すべての請求関連のコミュニケーションを受け取るメールアドレスを指定できます。Stripe は領収書と請求書を作成し、それらを請求用のメールアドレスに送信します：

```
receipts+**********@stripe.com
invoice+statements+***************@stripe.com
```

### Miro のお支払い設定

Miro の請求設定で Stripe の請求書を確認できます。[請求書を検索してダウンロードする方法](01-how-to-find-and-download-an-invoice.md)についてはこちらをご覧ください。

## 請求書に表示される料金の理解

次の請求書には、ライセンスの追加や削除、またはプランの変更などの情報が表示されます。プランを変更すると、支払い設定に**更新**という名前の新しい請求書が表示されます。

### 日割り料金の表示方法

ライセンスを追加または削除する際には、明確にするために請求書に2つの追加項目が含まれます:**残り時間**と**未使用時間**。

- **残り時間**は、最近の変更後のライセンスの更新された数を反映しています。
- **未使用時間**は、変更前にあったライセンス数を表示します。

不明な請求が表示されている場合は、[ライセンス管理ガイド](../../administration/user-management/04-manage-extra-licenses.md)をご確認ください。

#### ライセンスの追加

現在のプランに含まれるライセンスを超えて追加した場合、各追加ライセンスについて請求期間終了までの日割り料金が適用されます。例えば、2021年3月23日にライセンスを1つ追加した場合、その日割り料金が請求書に表示されます。

![charge_for_an_additional_license.jpg](../../../../../../docs/plans-billing/billing-and-payments/images/21017592958994_charge%20for%20an%20additional%20license.jpg)*ライセンス追加の日割り料金*

#### ライセンスの削除

ライセンスの削除をスケジュールした場合、それは更新日に有効となります。詳細については、[Miro の月額および年額課金](04-miro-billing.md)をご覧ください。

#### プランの変更

Miro プランを切り替えたり、サブスクリプションを月次から年次に変更したりすると、次回の請求書の金額が調整されます。前プランの未使用期間のクレジットは、新しい請求書に適用されます。例えば、未使用の月次サブスクリプションによるクレジットは、新しい年次 サブスクリプションで利用することができます。

![amount_for_switch_to_yearly.jpg](../../../../../../docs/plans-billing/billing-and-payments/images/21017605966098_amount%20for%20switch%20to%20yearly.jpg)
*月次サブスクリプションでの未使用期間のクレジットが新しい年次サブスクリプションに適用されます*

## よくある質問

**Miro の所在地はどこですか？**

Miro の所在地は、すべての請求書と領収書に表示されています:
201 Spear Street Suite 1100, San Francisco, CA 94105, USA

**Miro の VAT ナンバーは請求書に表示されますか？**

米国を拠点とする Miro は、オランダのワンストップショップ スキームで EU の VAT に登録されています。Miro には正式な VAT 登録番号や特定の請求要件はありません。
