---
title: "Enterprise \u30D7\u30E9\u30F3\u3067\u306E\u30DE\u30CD\u30FC\u30B8\u30C9\u30E6\
  \u30FC\u30B6\u30FC"
article_id: 6882052393618
translation_id: 6882052393618
locale: ja
sidebar_position: 6
created_at: '2022-07-29T11:04:13Z'
updated_at: '2026-02-26T14:01:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: user-management
---

Enterprise サブスクリプションでは、管理ユーザーとは、検証済みドメインの中にいるユーザーを指します。

ドメイン認証プロセスの詳細は、[ドメイン制御](../canvas-25-admin-features/domain-control/01-domain-control.md)に関する記事をご覧ください。

企業のユーザーを Enterprise 組織にプロビジョニングするには、ドメイン制御、SCIM、JIT、メールによる手動招待など、さまざまな方法があります。[詳細はこちら](13-user-provisioning-on-enterprise-plan.md)。

Enterprise プランの会社の管理者がマネージドユーザーを管理することができます。また、組織はユーザーが Miro にアクセスする方法や内容に対する方針と制御を確立し、ユーザー全体に対する所有権も持つことができます。例えば、チームへの割り当て、コンテンツの管理、アクティビティーの分析、ユーザーの削除が含まれます。

:::note
ユーザーの詳細には、**内部**または**外部**の分類があります。内部ユーザーは、検証済みドメインからのメールアドレスでログインしますが、外部ユーザーはそうではありません。詳細については、[内部および外部ユーザーに関するドメイン制御](../canvas-25-admin-features/domain-control/01-domain-control.md)をご覧ください。
:::

Miro では、以下のユーザー管理が可能です。

- ドメイン制御機能：
  - 企業ドメインに所属しているものの、Enterprise 組織にまだキャプチャーされていないユーザーについてのインサイトを取得
  - ドメインから Enterprise サブスクリプションにユーザーを自動キャプチャー
  - マネージドユーザーが、Enterprise 組織外に Miro のサブスクリプションを新規に作成するのを制限
- ライセンス管理
  - ユーザーがプランに対して[Advanced、Standard、Full（レガシー）、](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)または制限付きアクセスを持つべきかを定義しますし、管理されたユーザーのライセンスを変更します
- ユーザーアクセス
  - [非アクティブ化](01-deactivated-users.md)および[削除](10-remove-users-on-enterprise-plan.md)を Enterprise 組織からユーザーに対して行う
  - 組織内のチームへのユーザーアクセスを管理
  - [非アクティブ化されたマネージドユーザーのMiroへのアクセスをすべてブロックする](02-block-deactivated-users.md)
- 報告
  - 管理者の設定でEnterpriseプランに所属するマネージドユーザーを絞り込み、ユーザーの一覧表をCSVファイルとしてダウンロード
