---
title: "Zoom \u7528 Miro \u30A2\u30D7\u30EA\uFF08\u7BA1\u7406\u8005\u30AC\u30A4\u30C9\
  \uFF09"
article_id: 360022039379
translation_id: 360022039379
locale: ja
sidebar_position: 1
created_at: '2021-05-28T04:43:09Z'
updated_at: '2025-02-26T11:51:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: zoom
---

Zoom に Miro を埋め込んで機能する Zoom 用 Miro アプリは、チームがオールインワンのデジタル会議室を構築し、会議やワークショップで効果的にコラボレーションを行うことを可能にします。このアプリは、Zoom に Miro のコラボレーション機能を統合し、ゲストユーザーのオンボーディングの簡略化に特に力を発揮します。Miro の新規ユーザーには、登録不要でアクセスできるホワイトボードを提供します。

このガイドでは、Zoom と Miro の管理者が Zoom 用 Miro アプリ をユーザーが利用できるようにする手順を示します。

:::note
[「Zoom 用 Miro アプリ（ユーザーガイド）」](02-miro-app-for-zoom-user-guide.md)も併せてご覧ください。
:::

> **利用可能なプラン：** すべての Miro プラン、すべての Zoom プラン
> *Zoom の Business と Enterprise プランでは、管理者による Miro アプリの事前承認が必要となる場合があります
> **利用可能ソフトウェア/span>：デスクトップ版**

## Zoom 用 Miro アプリ を Zoom で有効化する手順

### アプリを検出できるようにする

1. アカウント設定の編集権限のある管理者として、Zoom Web ポータルにログインします。
2. ナビゲーションパネルで、**[Account Management]（アカウント管理）** > **[Account Settings]（アカウント設定）**をクリックします。
3. **[Zoom Apps]（Zoom アプリ）**タブをクリックします。
4. **[Zoom Apps Quick Launch Button]（Zoom アプリクイック起動ボタン）**が有効になっていることを確認します。これにより、あなたのアカウントのユーザーは、デスクトップクライアントの Zoom Appsボタン![](../../../../../../docs/integrations-apps/zoom/images/21017682787474_mceclip0.png) mceclip0 alt.pngをalt 見ることができます。
5. 設定が無効になっている場合は、トグルをクリックして有効にします。検証ダイアログが表示されたら、**Turn On**を クリックして変更を検証します。

さらに、Zoom では、特定のグループやユーザーにだけ Zoom アプリを有効化する手順を紹介しています。詳細については、こちら/span>の Zoom ヘルプセンターをご覧ください[。](https://support.zoom.us/hc/articles/360061555152)

Zoom_apps_quick_launch.jpg
Zoom アプリのクイック起動ボタンの有効化

これにより、アカウントのユーザーの、Zoom のメインクライアントの上部バーと、会議クライアントの下部バーで Zoom アプリが有効になります。

### Zoom でアプリを事前承認する手順

お客様が、Zoom ビジネスプランかエンタープライズ プランの管理者の場合、[ユーザーのアクセスを許可するため、](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA)こちらで Miro アプリの事前承認が必要になる場合があります。

![事前承認_ミロ_アプリ.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653155474_pre-approve%20Miro%20app.jpg)*Miroアプリの事前承認*

### アプリのインストールを許可するアカウント上のユーザーを選択する

Miro アプリの事前承認に加えて、アプリのインストールを許可するユーザーやグループを選択することができます。

allow_users_to_install_the_app.jpg
/span>Miro アプリのインストールを許可するユーザーやグループの選択

Miro アプリを承認して会社のアカウントにインストールすると、ユーザーは Zoom クライアントから Miro アプリにアクセスしてインストールできるようになります。

詳細については、[Zoom のドキュメント](https://support.zoom.us/hc/articles/360061555152)をご覧ください。

## Zoom 用 Miro アプリを Miro で有効化する手順

> **設定者：**Enterpriseプランの会社の管理者

[Enterprise プラン](../../plans-billing/miro-plans/04-enterprise-plan.md)で、承認されたアプリにのみインストールを制限している場合は、**[会社設定] > [アプリ] > [アプリの管理]** で、承認されたアプリ一覧に Zoom 用 Miro アプリが含まれていることを確認してください。アプリを許可リストに追加するには、アプリを検索して有効化するための検索窓に ClientID の「3074457354625507111」を貼り付けます。

approve_Zoom_on_Enterprise_plan.jpg
会社の設定の承認済みアプリのインストール

## ユーザーがアプリをインストールする方法

ユーザーは、Zoom 用 Miro アプリを、[Zoom マーケットプレイス](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA)か [Miro マーケットプレイス](https://miro.com/marketplace/zoom-app/)で見つることができます。

インストールの手順は、Zoom 用 Miro アプリを承認することから始まります。

install_Miro_app_for_Zoom.jpg
/span>Zoom アカウントへの Miro のアクセスの承認

認証されると、アプリはユーザーをZoomデスクトップアプリにリダイレクトし、新しくインストールされたMiroアプリを表示します。**アプリを追加するには、Zoomアカウントにログインする必要があります。**.

Miro ユーザーが**自分のボードを表示するには、**Miro にログインする必要があります。Miro にログインすると、システムブラウザーにリダイレクトされ、Miro にログインするか、Miro でアプリを直接承認するよう要求されます。ここでは、アクセス権を持つすべてのチームにアプリをインストールすることを選択できます。

install_Zoom_for_a_Miro_team.jpg
Miro チームの 1 つにアプリをインストール/span>

その後、Zoom デスクトップアプリに再度リダイレクトされ、既存のすべてのチームやボードを含む Miro のダッシュボードが表示されます。

![Miro_dashboard_in_Zoom.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653159442_Miro%20dashboard%20in%20Zoom.jpg)*ユーザーはダッシュボードからボードを選択し、Zoom内で開くことができるようになります。*

## ボードの共有アクセス設定について

ユーザーは、Zoom 会議でボードを共有するための適切なアクセス権限を定義できます。選択肢は4つ：**Zoomにいる人なら誰でも編集/コメント投稿/閲覧**、または**プライベート**（つまり、共有設定はMiro側で設定されているものと同じになります**）が可能**です。

board_embed_sharing_settings.jpg

*ボードのアクセス権限の設定*

アクセス設定のオプションは、組織全体のアクセスコントロールに従います。[Enterprise プラン](../../plans-billing/miro-plans/04-enterprise-plan.md)でボード埋め込み用の公開リンクによる共有が制限されている場合、ユーザーはこのオプションを利用できません。さらに詳しい情報：インテグレーションの埋め込みに関する Enterprise 共有ポリシーの管理

publi_editing_is_turned_off.jpg
/span>会社の管理者が公開編集を無効にしている場合の表示

## よくある質問

1. *Zoom用Miroアプリはどのようなデータにアクセスしているのですか？*
   - Zoom用Miroアプリは、ボードを特定のユーザーに関連付けるために、ユーザーのプロフィール情報を要求しています。ビデオ、音声、チャット、会議ファイルなどの会議コンテンツにはアクセス**しない**ため、Zoom のアクティブアプリの通知に表示されません。
2. *アプリはタブレットやモバイルデバイスにインストールできますか？*
   - いいえ、Zoom用のMiroアプリはデスクトップでのみ利用可能です。
3. *Zoom AppsはどのOSに対応していますか？*
   - Mac OSとWindows。
4. *Zoom Appsを使用するには、どのバージョンのZoomが必要ですか？*
   バージョン：3.
