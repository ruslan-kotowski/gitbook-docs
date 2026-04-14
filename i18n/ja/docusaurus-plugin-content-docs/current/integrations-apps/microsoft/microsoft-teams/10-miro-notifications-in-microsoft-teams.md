---
title: "Microsoft Teams\u306EMiro\u901A\u77E5"
article_id: 4403762338450
translation_id: 4403762338450
locale: ja
sidebar_position: 10
created_at: '2021-07-15T05:59:22Z'
updated_at: '2025-04-24T13:52:02Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: ms-teams
---

Miro の通知を Microsoft Teams (MS Teams) 内のチャットメッセージとして受け取ります。アプリを切り替えることなく、常に情報を入手し、ボードを共有し、仕事をすばやく管理できます。

![](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/22451245005458_mceclip0.png)
*Microsoft TeamsチャットのMiro通知*

Miro通知を使用すると、MS Teamsチャットで以下のイベントを直接追跡できます：

- ボードが自分と共有されたとき
- ボードにコメント投稿者
- コメント投稿者
- ボードへのアクセス要求を受け取り、即座に承認または拒否することができます。
- 招待者の登録

### Microsoft TeamsでMiro通知を設定する方法

#### 前提条件

Miro for Microsoft Teamsが有効になっていることを確認してください。方法については、[Miro for Microsoft Teamsの概要を](06-miro-for-microsoft-teams-overview.md)ご覧ください。

#### 手続き

Miro通知をMicrosoft Teamsに追加するには、以下の手順に従ってください：

1. Microsoft Teamsで、Miroとのチャットを開きます。
2. メッセージバーに「Connect」と入力してください。![](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/22452689633554_mceclip1.png)
   **MiroとMS Teamsの接続**
3. **Miroアカウントに接続を**選択します。
   **Microsoft Teamsのインストールと認証]**モーダルが別タブで開きます。
4. 追跡したいチームを選択します。
   ![](../../../../../../../docs/integrations-apps/microsoft/microsoft-teams/images/22454855305362_mceclip2.png)
   **Microsoft Teamsで追跡するMiroチームの選択**
5. **インストールと認証を**選択します。
   Miro との MS Teams チャットでは、Miro からの挨拶メッセージがセットアップ完了を示します。

   MS TeamsでMiro通知の設定が完了しました。
   > ✏️ 通知は選択したMiroチームのみに送られます。複数のチームを追跡するには、追跡したいチームごとにセットアップ手順を繰り返します。

### よくある質問

**チームへの通知が届かなくなったのはなぜですか？**

以前にMS TeamsでMiroの通知を設定し、通知の受信を停止した場合は、設定の手順を繰り返してください。問題が解決しない場合は、Miroサポートにご連絡ください。

**Miroボードの変更の概要を知ることはできますか？**

現在、MS Teams の Miro 通知では変更サマリーを利用できません。しかし、この機能は現在バックログにあります。
