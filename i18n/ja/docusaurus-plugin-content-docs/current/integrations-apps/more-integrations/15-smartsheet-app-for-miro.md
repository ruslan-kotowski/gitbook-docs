---
title: "Miro \u7528 Smartsheet \u30A2\u30D7\u30EA"
article_id: 5753415785618
translation_id: 5753415785618
locale: ja
sidebar_position: 16
created_at: '2022-05-25T06:41:50Z'
updated_at: '2025-01-13T14:57:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: smartsheet
---

主な機能：

- Miro から Smartsheet 内の新規または既存のシートの行に付箋をエクスポートする
- Smartsheet から Miro のボードにカードとして行をインポートする
- Miro と Smartsheet の両方で、双方向同期して、作業を更新する

> **利用可能なプラン：**すべての Miro プラン
> ブラウザ版（デスクトップ

:::warning
Safari でアプリを動作させるには、ブラウザー設定で、**[サイト越えトラッキングを防ぐ]** オプションをオフにします。
:::

### アプリのインストール方法

アプリは、Miro のマーケットプレイスからインストールすることができます。Miro の Smartsheet を検索し、**[アプリを取得]** をクリックします。/span>Smartsheet アプリを追加するチームを選択するためのページにリダイレクトされます。ピッカーでチームを選択し、[インストールして認証] をクリックします。

:::warning
管理者以外のユーザーは、設定で許可されていなければ、このアプリをインストールすることはできません。
⚠️ Enterprise プランの会社の管理者は、設定でアプリを承認する必要があります。/strong>/span>詳細はこちらをご覧ください。
:::

installing_smartsheet_app.jpg
Miro のチームを選択してアプリをインストール

をインストールすることもできます。 **をインストールすることもできます。**をインストールすることもできます：

1. 作成バーで、**ツール、メディア、インテグレーション** **（+）を**選択します。**ツール、メディア、インテグレーション」**パネルが開きます。
2. **ツール]**タブで検索し、[Smartsheet] を選択します。
   **Smartsheet**モーダルが開き、許可を求めるプロンプトが表示されます。

![スマートシートエントリーポイント.png](../../../../../../docs/integrations-apps/more-integrations/images/21537438852626_smartsheet-entry-point.png)
/span>Miro のボード内からアプリをインストール

**Miro と Smartsheet アカウントを接続するかどうかを確認するメッセージが表示されたら、Smartsheet アカウントにログインし、アプリへのアクセスを許可します。**

allow_access_to_Miro.jpg
**アプリが Smartsheet アカウントへのアクセスを許可**

### Miro の付箋やカードを Smartsheet の行にエクスポートする方法

1. ツールバーで Smartsheet アプリを開きます。Smartsheet にまだログインしていない場合は、まずこれを行う必要があります。次に、変換する付箋を選択します。
2. 付箋のコンテンツを追加する Smartsheet のワークスペース、シート（新規または既存）、行を選択します。また、新しいシートを作成し、新しいシートに付箋をエクスポートすることもできます。
3. 最後に、**[Smartsheet の行に変換]** を選択します。これで、コンテンツは Smartsheet にエクスポートされます。付箋は、自動的に Smartsheet のカードに変換されます。
   Smartsheet から Miro に対応する行をインポートしない限り（近日公開予定）、カードは Smartsheet と同期しません。以下の Miro に Smartsheet のデータをインポート/span>する方法をご覧ください。
   smartsheet_export.gif
   Miro から Smartsheet に付箋をエクスポート/span>

### Miro に Smartsheet の行をインポートする方法

1. Miro で Smartsheet アプリを開き、タブを **[Miro から変換]** から **[Smartsheet から選択]** に変更します。
2. **[Smartsheet から選択]** をクリックすると、既存のシートとともにピッカーが表示されます。特定のワークスペースに基づいて行をフィルタリングし、シートを選択するオプションがあります。
3. チェックボックスをオンにして [インポート] **を**選択し、インポートする行をすべて選択します。
4. 行はカードとしてインポートされます。
   import_from_smartsheet.gif
   *Smartsheet から Miro へデータをインポート*
5. カードを選択し、[展開] アイコンをクリックして変更を適用し、**[変更を保存]** をクリックすることで、Miro 内で直接行を編集することができます。カードへの更新は、Miro と Smartsheet に反映されます。/span>
   edit_Smartsheet_card.gif
   Miro で Smartsheet のカードを編集/span>
