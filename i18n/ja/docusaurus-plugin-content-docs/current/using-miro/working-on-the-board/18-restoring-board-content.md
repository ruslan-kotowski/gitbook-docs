---
title: "\u30DC\u30FC\u30C9\u30B3\u30F3\u30C6\u30F3\u30C4\u306E\u5FA9\u5143"
article_id: 360019838260
translation_id: 360019838260
locale: ja
sidebar_position: 18
created_at: '2021-02-24T08:56:24Z'
updated_at: '2026-01-06T19:00:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: delete-board
---

ボードコンテンツの復元機能があれば、誤ってコンテンツを削除しても、チームの生産性が損なわれることはありません。ボード編集者は、最近ボードから削除したオブジェクトを簡単に復元できます。

> **設定者：**[メールで](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md)個別にボードに招待された編集者、もしくは Miro の[プロジェクト](../sharing-boards/16-projects.md)や[チーム](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md)のメンバーとしてボードにアクセスできる編集者
> **利用可能な環境**：ブラウザー版、[デスクトップアプリ](../../getting-started/apps-for-devices/05-desktop-app.md)、[タブレットアプリ](../../getting-started/apps-for-devices/11-tablet-app.md)

> **⚠️** この機能は[ビジター](../sharing-boards/08-collaboration-with-visitors.md)は利用できません。

> ボードバージョンを復元する方法については、[こちらのガイド](../managing-boards/12-board-history-versions.md)をご覧ください。

### 復元可能なコンテンツ

- 現在のアクティブセッション中にボードから削除されたコンテンツ、またはセッションが終了した場合はコンテンツが削除されてから 30 分後
- ボードから削除された直近 1000 個のオブジェクト（コンテンツが削除されてから 30 分以上経って復元が行われた場合）
- 複数オブジェクトが選択され、同時に削除された場合、期限なくボードから削除された全てのコンテンツ（次の 1000 個のオブジェクトが削除されるまで）

### コンテンツの復元方法

削除したオブジェクトの復元方法を以下に示します。

1. 左下にある**[サイドバーを開く]**アイコンをクリックする。
2. 開いたボードの概要メニューにある **[ボード履歴]** アイコンをクリックする。
3. 復元したいオブジェクトの**[復元]**アイコンをクリックする。削除されたオブジェクトがボード上の削除前と同じ場所に再表示され、その部分が拡大表示される。

restore_board_content_restore_feature.jpg
削除されたオブジェクトの復元

### 制限

> **⚠️** なお、この操作では次のような例外ケースが起こり得ます。

- コンテンツが別の場所に復元される（例：[接続ライン](../essential-tools/05-connection-lines.md)を復元すると、接続されていた[付箋紙](../essential-tools/14-sticky-notes.md)が別の場所に復元される）
- 復元前は接続されていたオブジェクトの接続が失われる（例：[テーブル](../essential-tools/02-cards.md)から[カード](../advanced-tools/05-grid.md)を削除し、復元すると、カードは同じ場所に復元されるがテーブルとは接続されていない）
- 特定のコンテンツが復元できない。この機能には現在、以下に示すような機能制限がある。

- ボードから削除されたオブジェクトに接続されていた[ライン](../essential-tools/05-connection-lines.md)
- 削除されたテーブルのセル内テキスト（テーブルと一緒に削除されたテキストであれば復元可能）
- [ユーザー ストーリーマップ](../advanced-tools/07-user-story-mapping.md)（フレームワークとカードの両方）
- 別途[コメント](../facilitation-tools/asynchronous-tools/01-comments.md)投稿者削除

  ![mceclip0.png](../../../../../../docs/using-miro/working-on-the-board/images/21017605949842_mceclip0.png)
  *コンテンツが復元されていない場合に表示されるバナー*

原則として、オブジェクトを削除した直後に復元すれば、バッチ内のすべてのリンクも復元されます。ただし、ボードの外の外部オブジェクトとのリンクは復元されない可能性があります。

なお、[ボードの複製](../managing-boards/03-how-to-duplicate-a-board.md)は、元のボードで削除されたオブジェクトを復元するオプションには対応していません。

### よくある質問

1. *コンテンツが消えてしまいました。削除されたオブジェクトを復元するオプションが表示されません。*どうすればよいですか？
   - 一部のコンテンツは復元できませんのでご注意ください（上記の制限事項をご覧ください）。コンテンツに他の種類のウィジェットが含まれている場合は、以下をご確認ください。/span>
   - 開いたボードが正しいことを確認する
   - 似たような名前の[カスタムテンプレート](../../getting-started/start-here/your-first-board/02-custom-templates.md)のリストを確認する
   - ボードの[ミニマップ](21-work-smarter-not-harder.md)で、ボードの様々な場所にコンテンツがあるかどうかを確認する
   - 複数の Miro プロフィールをお持ちの場合、Miro の認証に正しいメールアドレスが使われているかを確認する
