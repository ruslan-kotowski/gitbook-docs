---
title: Miro for Microsoft Teams (管理者ガイド)
article_id: 4406387610002
translation_id: 4406387610002
locale: ja
sidebar_position: 1
created_at: '2021-09-09T10:28:14Z'
updated_at: '2025-11-25T16:07:14Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: slack-ms-teams
availability:
  notes: '利用可能なプラン：: 無料、Starter、Business、Education、Enterpriseプラン、Microsoft 365の全プラン'
---

:::note
アクセス許可とアクセス設定は、プランの種類によって異なります。Microsoft Teamsの外部ユーザーについての詳細は、[Microsoftのアプリポリシーを](https://learn.microsoft.com/microsoftteams/apps-external-users)参照してください。
:::

Microsoft Teams用のMiroインテグレーションを有効にして、組織内のコラボレーションを加速させましょう。Miro for Microsoft Teamsは、ユーザーがリアルタイムで通知を受け取ったり、Teamsのミーティング、チャンネル、チャット、カレンダーの招待に埋め込まれたMiroボードで共同作業を行ったりできるようにする、多くの体験を提供します。

Miroはまた、リンクの展開と検索メッセージの拡張機能によってアダプティブカードをサポートし、共有ボード上でより多くのコンテキストをユーザーに与え、迅速なボードアクセス管理を可能にします。

:::tip
Miroの[Microsoft Teamsインテグレーションについては](..)こちらをご覧ください。
:::

<iframe allowfullscreen="" frameborder="0" height="315" src="//www.youtube-nocookie.com/embed/6xab9nSnmAA" width="560"></iframe>
 *マイクロソフトチーム向けMiro*

## アプリ管理

:::warning
Microsoft管理者は、Microsoftアプリ管理カタログからMicrosoft Teams用のMiroインテグレーションを有効にする必要があります。Miro Enterprise管理者もMiroアプリ管理パネルからインテグレーションを有効にする必要があります。
:::

### Microsoft Teamsのアプリ管理

設定はアカウントごとに異なる可能性があります。[Microsoft Teamsでアプリを管理する方法については](https://learn.microsoft.com/microsoftteams/manage-apps)、こちらをご覧ください。

組織がインテグレーションを最大限に活用できるように、[Microsoftのアプリセットアップポリシーを](https://learn.microsoft.com/microsoftteams/teams-app-setup-policies)使用してMiroアプリを一括インストールして固定します。

### Miroのアプリ管理

Miro会社の設定 >**アプリで**、2つのMicrosoft Teamsアプリが表示されます：

- Miro for Microsoft Teams (タブインテグレーション) - Miroをカレンダー、Teamsミーティング、チャンネル、チャットに埋め込みます。
- Microsoft Teams（ボットインテグレーション） - ユーザー通知

Microsoft Teams（ボットのインテグレーション）をオフにすると、ユーザーは Microsoft Teams 内で Miro の通知を受け取らなくなります。

![Microsoft-Teams-Bot-Tab-Apps.png](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21017606037010_Microsoft-Teams-Bot-Tab-Apps.png)*Microsoft Teams アプリ*

## ボードの共有アクセス設定について

会議、カレンダーの招待、チャット、チャンネルでボードをタブとして追加する場合、ユーザーは適切な共有権限を定義することができます。Microsoft Teamsにボードをタブとして追加するには、Microsoft TeamsにMiroをタブとして追加するをご覧ください。[埋め込みボードのアクセス](../../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)設定についてはこちらをご覧ください。

### ボードのアクセス設定をする

アクセス設定のオプションは、組織全体のアクセスコントロールに従います。Enterprise プランでボード埋め込み用の共有が制限されている場合、そのオプションをユーザーが利用することはできません。詳しくは、[埋め込みインテグレーションのEnterprise共有ポリシーの管理 をご覧ください。](../../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)

![パブリ__編集_オフ.jpg](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/21017593055506_publi%D1%81%20editing%20is%20turned%20off.jpg)*会社の管理者が公開編集をオフにした場合の例*
