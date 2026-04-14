---
title: Miro における Jira OAuth 1.0 の廃止
article_id: 28738797627538
translation_id: 28739475796754
locale: ja
sidebar_position: 13
created_at: '2025-08-13T12:34:30Z'
updated_at: '2025-10-20T14:49:06Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: '対象: 会社の管理者 プラン: Starter, Business, Enterprise, Education プラットフォーム: ブラウザ、デスクトップ'
---

Jira OAuth 1.0 認証は 2025年8月から廃止されます。

すでに Jira OAuth 2.0 に更新している組織はこの記事を無視できます。会社の管理者による措置は不要です。組織が OAuth 2.0 を使用していることを会社の管理者に確認できます。

:::warning
組織が OAuth 2.0 に更新していない場合、Jira Cloud、Server、Data Center を含め、Miro との Jira インテグレーションに支障が生じる可能性があります。
:::

組織内のチームを更新できるのは会社の管理者のみです。

中断が発生した場合、組織がOAuth 2.0認証にアップデートするまで、MiroとJiraの同期が停止します。既存のJiraカードはMiroボードに残ります。

中断とは、インポートが利用できず、カードは更新されず、詳細が読み込めず、プランナーの作成や更新が利用できないことを意味します。

中断を避けるために、Miroは会社の管理者が直ちにJira OAuth 2.0に更新することを推奨します。

:::tip
管理者はOAuthバージョンを確認することができます。
:::

## なぜOAuth 1.0は廃止されたのですか？

AtlassianはOAuth 1.0認証プロトコルを廃止し、サポートを終了しました。

**詳細情報:** （外部リンク）[REST API用OAuth 1.0a（廃止予定）](https://developer.atlassian.com/cloud/jira/platform/jira-rest-api-oauth-authentication/) をご覧ください。

## OAuthバージョンを確認する

Enterprise、Starter、Businessプランの管理者として、チームがOAuth 1.0またはOAuth 2.0を使用しているか確認できます。

以下の手順に従ってください:

1. Miro のダッシュボードから右上の自分のアバターをクリックして、**管理者コンソール**を選択します。
2. **チーム** > **[チーム名]**に移動します。
3. **アプリ**をクリックします。
4. **Jira カード**を見つけてクリックします。
5. **管理者設定** > **Jira 設定**に進みます。
   設定には、チームが使用している OAuth のバージョンが示されています。
6. （オプション）確認したい他のチームのためにステップ 1～5 を繰り返します。
7. OAuth 2.0 を使用していないチームがある場合は、会社の管理者に通知します。

## 会社の管理者を見つける

会社の管理者を特定するには、以下の手順に従ってください:

:::note
(Enterprise) チームのプライバシーが有効な場合、会社の管理者以外はメンバーリストを閲覧できません。
:::

1. Miroで**チームのプロフィール設定**に移動します。
2. **メンバー**ページを開きます。
3. **追加の役割**をクリックします。
4. **会社の管理者**の役割を持つユーザーを見つけます。

:::tip
チームがOAuth 2.0にアップグレードし、可能な中断を避けるために、この資料を会社の管理者と共有してください。
:::

## 会社の管理者がOAuth 2.0にアップグレードする

会社の管理者として、組織を OAuth 2.0 へアップグレードするための以下のリソースを利用できます。

- [OAuth 2.0 を使用して Jira Cloud へ接続する](https://help.miro.com/hc/articles/8588617184402)
- [OAuth 2.0 を使用して Jira Data Center へ接続する](https://help.miro.com/hc/articles/25753304280466)
- [組織内のチームをデフォルトの Jira 設定に接続する](https://help.miro.com/hc/articles/26438407676434)

## 暫定的なソリューション

もし現在のところ OAuth 2.0 が組織にとっての選択肢でない場合、Miro は[OAuth 1.0 を用いた暫定的なソリューション](https://help.miro.com/hc/articles/27689156602514)をご提供します。

しかしながら、Miro は、アトラシアンの最新基準に従う、最も安全で将来的に適した認証方法として、OAuth 2.0 へのアップグレードを推奨します。

## 追加のヘルプ

ご質問がある場合や、会社の管理者が不明な場合は、[Miro サポート](https://help.miro.com/hc/articles/360020185799)にお問い合わせください。
