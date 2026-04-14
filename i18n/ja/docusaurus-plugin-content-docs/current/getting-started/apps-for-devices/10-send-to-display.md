---
title: "\u30C7\u30A3\u30B9\u30D7\u30EC\u30A4\u306B\u9001\u4FE1"
article_id: 4406230245010
translation_id: 7697537347218
locale: ja
sidebar_position: 10
created_at: '2022-09-19T08:12:47Z'
updated_at: '2026-04-10T12:06:12Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: interactive-displays
---

数秒でコラボレーションを開始します。ディスプレイへの送信機能を使用すると、インタラクティブディスプレイで Miro ボードを起動します。

> ***Miro UI の段階的な展開***
> Miro は、ボードのユーザー インターフェイスをより万人に向けた直感的なものにし、プロジェクトを進化させたスペースを導入します。すべての Miro アカウントに対して、数週間かけて順次展開されます。
>
> すでに強化された UI とスペースをお使いの場合、この記事では変更されたツールの場所が分かる場合もあります。
>
> 最新のドキュメントを見るには、[Miro の新しいシンプル化されたユーザー インターフェイス](../../using-miro/working-on-the-board/02-miro's-new-simplified-user-interface.md)をご覧ください。
>
> 展開が完了次第、この記事は更新されます。

インタラクティブディスプレイで Miro をセットアップする[方法をご覧ください](07-interactive-displays.md)。

## ディスプレイに送信を使用する方法

1. インタラクティブ ディスプレイで、Miro アプリを開くか、ブラウザーを開いて [miro.com/displays](https://miro.com/displays/) に移動します。
2. 個人のデバイスで Miro ボードを開きます。

**ラップトップまたはタブレットから**

1. ラップトップまたはタブレットのボードバーで縦の三点リーダーを選択します。
   すると、**メイン**メニューが開きます。
2. **インタラクティブ ディスプレイに送信**を選択します。
3. インタラクティブ ディスプレイに表示される独自のペアリングコードを入力します。これにより、ラップトップまたはタブレットからディスプレイにボードが送信されます。

**モバイルデバイスから**

:::note
モバイルデバイスをご利用の場合、まず[iOS](https://apps.apple.com/us/app/miro-collaborative-whiteboard/id1180074773)または[Android](https://play.google.com/store/apps/details?id=com.realtimeboard&hl=en&gl=US)用のMiroモバイルアプリをダウンロードしてください。
:::

1. モバイルデバイスの Miro ボードから、右上の **設定** アイコンをタップします。
   **![board_settings.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967840616850_board%20settings.jpg)**
   *モバイルアプリでボードの設定を開く*
2. **インタラクティブディスプレイに送信**をタップします。
   **![send_to_interactive_display.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967865515794_send%20to%20interactive%20display.jpg)**
   ***モバイルアプリでインタラクティブディスプレイに送信するオプション***
3. インタラクティブ ディスプレイに表示される独自のペアリングコードを入力します。これにより、モバイルデバイスからディスプレイにボードが送信されます。
   ![enter_code.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4967892004114_enter%20code.jpg)
   *コードを入力するオプション*

:::tip
セッションが終了したら、データ保護のため、ディスプレイからログアウトする必要があります。忘れた場合、非アクティブになってから 15 分後に自動的にログアウトされます。
:::

## トラブルシューティング

Windows デスクトップアプリにディスプレイへの送信画面が表示されない場合は、以下のトラブルシューティング手順をお試しください。

1. [デスクトップ用 Miro アプリ](https://miro.com/apps/)をインストールする。
2. Miro デスクトップアプリのアイコンを右クリックし、**プロパティ**を選択する。
   ![properties.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4949111804946_properties.jpg)*Miro アプリのプロパティ*
3. **ショートカット**タブに切り替え、**ターゲット**フィールドの CLI 引数に以下のフラグを追加し、[OK] をクリックして変更を適用します。

   ```
   --public-device
   ```

   ![target_field.jpg](../../../../../../docs/getting-started/apps-for-devices/images/4949083211538_target%20field.jpg)*Miro プロパティのショートカットタブ*
4. これで、アプリを起動するたびに、デフォルトでディスプレイに送信オプションが表示されるようになります。

:::tip
Miroがサポートする[ディスプレイの種類](07-interactive-displays.md)を詳しく知ることができ、 [ハイブリッドコラボレーションに最適なディスプレイの選び方について読むことができます。](09-selecting-the-right-interactive-display-for-hybrid-collaboration.md)
:::
