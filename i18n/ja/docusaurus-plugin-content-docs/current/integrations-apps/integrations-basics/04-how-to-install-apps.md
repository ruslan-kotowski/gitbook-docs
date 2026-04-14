---
title: アプリのインストール方法
article_id: 360017731093
translation_id: 360017731093
locale: ja
sidebar_position: 4
created_at: '2019-02-11T10:12:46Z'
updated_at: '2025-08-05T07:54:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'ユーザー: 全ユーザー プラン: すべてのプラン プラットフォーム: ブラウザー、デスクトップアプリ チームの管理者は、管理者以外のユーザーによるインストールを制限することができます。Enterprise
    プランの会社の管理者は、承認されたアプリのみへの制限をさらに強化することができます。'
---

Miro マーケットプレイスからアプリをインストールすることで、Miro の機能を拡張できます。この記事では、アプリのインストールとアンインストール、アプリ権限の理解、カスタムインテグレーションの作成の概要について案内します。

## Miro マーケットプレイスからアプリをインストール

[Miro マーケットプレイス](https://miro.com/marketplace/)は、Miro エクスペリエンスを向上させるためのアプリを発見して追加するための中心的なハブです。アプリは、ボードから直接、またはマーケットプレイスのウェブサイトを訪問してインストールすることができます。

![Miro_marketplace.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021611044242_Miro%20marketplace.jpg)*Miro マーケットプレイス*

ユーザーがアプリを追加する主な方法は 2 つあります：

1. **ボードから:**作成ツールバーの**ツール、メディア、インテグレーション（＋）**アイコンをクリックし、「マーケットプレイスタブ」の「統合を検索」検索ボックスを使用します。アプリがすでにリストにある場合は、クリックして追加してください。このパネルから利用可能なアプリを閲覧することもできます。
   ![marketplace-add-apps.png](../../../../../../docs/integrations-apps/integrations-basics/images/21260776452626_marketplace-add-apps.png)*作成ツールバーのマーケットプレイス*
2. **マーケットプレイスのウェブサイトから:**また、この[Miro マーケットプレイス](https://miro.com/marketplace/)のウェブサイトに直接アクセスして、アプリをブラウズおよびインストールすることもできます。

**会社の管理者の方へ:**
適用されるプランの会社の管理者は、チームの設定を通じて、チーム全体にアプリをインストールすることもできます。これを行うには、**チーム設定** > **アプリとインテグレーション** > **アプリをインストール** に移動します。このセクションでは、アプリをチーム全体に一元管理および展開することができます。

![apps_and_integrations_page.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021832338450_apps%20and%20integrations%20page.jpg)*管理者用のチーム設定におけるインストール済みアプリのセクション*

## アプリをアンインストールする

チーム設定からアプリを管理およびアンインストールすることができます。管理者以外のユーザーは、チームの設定によってアプリのアンインストールに制限がある場合があります。

:::warning
管理者以外のユーザーは、チーム設定で管理者によりアプリのインストールが許可されていない場合、アプリをアンインストールできません。
:::

チームのアプリを管理するには、**チーム設定 > アプリとインテグレーション** に移動してください。このページには、現在チームまたは個人的にインストールされているすべてのアプリが表示されます。

![apps_settings.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021898097682_apps%20settings.jpg)*[チーム設定] 内の [アプリとインテグレーション]*

アプリをアンインストールするには、以下の手順に従ってください：

1. **アプリとインテグレーション**リストから、削除したいアプリを選択します。
2. **チームに対してアンインストールする** または **アンインストールする** をクリックします。利用可能なオプションは、アプリのインストール方法と管理者権限によって異なります。

![uninstall_an_app.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021797466258_uninstall%20an%20app.jpg)*アプリをアンインストールするオプション*

## アプリのインストール権限

チームと会社の管理者は、誰がアプリをインストールできるか、どのアプリが組織で利用可能かを管理するためのさまざまなコントロールを持ち、セキュリティとコンプライアンスを確保します。

チームの管理者は、管理者以外のチームメンバーがアプリをインストールできるかどうかを設定できます。この設定は**チーム設定 > アプリとインテグレーション**のアプリ管理オプションで見つけることができます。

![allow_non-admins_to_install_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021903025170_allow%20non-admins%20to%20install%20apps.jpg)*チーム設定での「管理者以外にアプリのインストールを許可する」オプション*

Enterprise プランの[ユーザー](../../plans-billing/miro-plans/04-enterprise-plan.md)向けに、会社の管理者はより詳細なコントロールにアクセスできます。彼らは**会社の設定** > **アプリ**を通じて**承認済みアプリ**を管理できます。この機能により、管理者は会社が承認したアプリケーションのリストを作成し、この承認リストにないアプリをユーザーがインストールすることを制限できるようになります。[Enterprise プランのアプリ検索とインストール設定の管理について詳しく知る](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md)。

![Enterprise_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021890162962_Enterprise%20apps.jpg)*Enterprise の会社設定で承認済みアプリを管理*

## カスタムインテグレーションと開発者プラットフォーム

Miro マーケットプレイスにない特定の機能が必要な場合は、[Miro 開発者プラットフォーム](https://miro.com/api/)を使用して、自分専用のカスタマイズされたソリューションを作成できます。このプラットフォームは、REST API、Web プラグイン、埋め込み機能を含む強力なツールを提供し、あなたのニーズに合わせた強力なインテグレーションを構築するのに役立ちます。

カスタムインテグレーションを開発する際に考慮すべき重要なポイントは次のとおりです。

- **始め方:**[開発者チームを作成](https://developers.miro.com/)してアプリの構築を開始できます。標準の開発者チームは開発およびテスト目的で使用され、一部の制限があります。
  - チーム内で最大 5 人のユーザー。
  - 1 つのチームのボード数は最大 3 件。
  - ボードに透かしが表示されます。
  - ボードのエクスポート機能は利用できません。
- **Enterprise プランの開発者：**お客様の組織が[Enterprise プラン](../../plans-billing/miro-plans/04-enterprise-plan.md)をご利用の場合、サブスクリプションの一部として開発者チームを作成できます。これらの開発者チームは標準のものに比べて制限がなく、すべてのEnterprise級のセキュリティ機能を享受できます。[Enterprise プランの開発者チームについて詳しく知る](../../enterprise-administration/managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md)。

さらなる情報やサポートが必要な場合、他の開発者との交流を求める場合は、[開発者プラットフォーム フォーラム](https://community.miro.com/developer-platform-forum-57)をご覧ください。
