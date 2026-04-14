---
title: "\u4F01\u696D\u6A5F\u5BC6\u30C7\u30FC\u30BF\u691C\u51FA\u306E\u975E\u30A2\u30AF\
  \u30C6\u30A3\u30D6\u5316\uFF08\u30D9\u30FC\u30BF\u7248\uFF09"
article_id: 23760380385042
translation_id: 23760380385042
locale: ja
sidebar_position: 17
created_at: '2025-01-07T12:24:40Z'
updated_at: '2025-11-25T16:22:17Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

ビジネス機密データ検出を非アクティブ化すると、Miro の内蔵機械学習ラベルを使用した一般的なカテゴリの機密ビジネス情報のシームレスな特定とラベル付けが無効になります。

ビジネス機密データ検出ラベルを自動機密分類で使用している場合、ビジネス機密データ検出機能を非アクティブ化することはできません。これは、ビジネス機密データ検出を非アクティブ化すると、自動機密分類やコンテンツに適用されるガードレールに影響を与える可能性があるためです。非アクティブ化するには、まず自動機密分類からすべてのビジネス機密データ検出ラベルを削除する必要があります。一度ビジネス機密データ検出を非アクティブ化すると、管理者は自動機密分類でビジネス機密データ検出ラベルを設定する能力を失い、データ検出概要ページやコンテンツ エクスプローラーで関連するボードや一致を閲覧することができなくなります。

企業機密データの検出を非アクティブ化するには、次の手順を実行します。

:::note
企業機密データ検出を非アクティブ化するには、[機密コンテンツ管理者](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)の権限が必要です。機密コンテンツ管理者権限の申請については、会社の管理者にお問い合わせください。
:::

1. [Miro 設定](https://miro.com/app/settings)にアクセスします。
2. 左側のペインで、**Enterprise Guard**の下にある**データ検出**をクリックします。
3. **データ検出**ページで、**設定**タブをクリックします。
4. **ビジネス・センシティブ**セクションで、**管理**ボタンをクリックします。
5. スライドアウトパネルで**無効化**をクリックします。
