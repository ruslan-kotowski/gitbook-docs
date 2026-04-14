---
title: ボードの履歴：バージョン
article_id: 360021668819
translation_id: 360021668819
locale: ja
sidebar_position: 12
created_at: '2021-05-17T11:56:55Z'
updated_at: '2026-01-06T19:02:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: activity-list
availability:
  notes: '実行可能なユーザー：: ボード所有者、ボード共同所有者、ボードが配置されているチームのメンバーであるボード編集者ボードの内容をコピーする許可がある場合
    利用可能なプラン：: Starter、Business、Enterprise、Education 利用可能なプラットフォーム：: ブラウザー、デスクトップ、タブレットアプリ'
---

Miro ボードのすべてのバージョンは、ボードの履歴に自動的に保存されます。いつでも変更を確認し、復元することができます。

### 主な機能

- ボードは、変更が加えられた場合は毎時間、また各コラボレーション セッションの終了時にもバックアップされます
- 保存されたボード履歴のバージョンは、*90 日間*保存されます
- 元のボードは*変更されません*。復元されたバージョンは、*別の*ボードとして作成され、タイトルにはデフォルトで日付が表示されます

:::warning
予期しないネットワークの問題で、ボードのバックアップができない場合があります。一貫性のあるバックアップのために、安定したインターネット接続であることを確認してください。
:::

### ボードの以前のバージョンを復元する

以前のバージョンを復元するには、以下を実施してください。

1. ボードバーで縦の**三点リーダー**を選択します。
   **メイン**メニューが開きます。
2. **ボード** > **履歴**を選択します。
   **履歴**パネルが開きます。デフォルトで**アクティビティー**タブが開いています。
3. **バージョン**を選択します。
4. バージョンを選択します。
   **別のボードとして復元**モーダルが開きます。
5. （オプション）画面の指示に従います。
6. **復元**を選択します。

### 以前のボードバージョンの復元を制限または無効化する

- この機能は、[ボード所有者](../sharing-boards/01-board-access-rights.md)、共同所有者が利用可能で、ボードが配置されているチームのメンバーである[編集者](../sharing-boards/01-board-access-rights.md)に対して有効にできます。
- この機能は[ボードコンテンツの設定](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)に依存します。このオプションは、ボード所有者がボードコンテンツのコピーをチームメンバーに許可した場合のみ利用できます。これはボードの**共有**ボタン > **共有設定** > **アクセス権限**で設定できます。
- [コンテンツ管理者権限](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)は[Enterpriseプラン](../../plans-billing/miro-plans/04-enterprise-plan.md)で有効化されると、コンテンツ設定で無効化されていても、[ボードの所有権を自分に再割り当てする](../sharing-boards/01-board-access-rights.md)ことにより、会社の管理者はボードの**バージョン**にアクセスできます。

このオプションを使用する権限がない場合は、対応するメッセージが**バージョン**タブに表示されます。機能を有効にするには、ボードの所有者に連絡してください。

## よくある質問

**最近、私の[プランをアップグレードしました](../../plans-billing/manage-your-subscription-and-plan/03-upgrade-your-plan.md)。私のチームがFreeプランを利用していた時に作成されたボードのバージョンを復元できますか？**

はい、アップグレード後には、Freeプランにいた時に作成されたバージョンを復元できます。

**ボードの履歴にバージョンがありません。なぜですか？**

[無料プラン](../../plans-billing/miro-plans/09-free-plan.md)では、この機能はサポートされていないことにご注意ください。また、ボード上でバージョンを復元できる役割を持っていることを確認してください（[ボード所有者](../sharing-boards/01-board-access-rights.md)、[共同所有者](../sharing-boards/06-co-owners-of-boards-and-spaces.md)、または[編集者](../sharing-boards/01-board-access-rights.md)であり、ボードが配置されているプランのメンバーである必要があります）。さらに、ボードの所有者/共同所有者は、チームメンバーにボードコンテンツをコピーすることを許可する必要があります。
オブジェクトを削除した場合は、復元することもできます。詳しくは[こちらのガイド](../working-on-the-board/18-restoring-board-content.md)をご覧ください。
