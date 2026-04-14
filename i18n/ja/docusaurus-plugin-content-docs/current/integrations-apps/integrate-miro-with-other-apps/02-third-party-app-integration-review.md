---
title: "\u30B5\u30FC\u30C9\u30D1\u30FC\u30C6\u30A3\u30FC\u88FD\u30A2\u30D7\u30EA\u306E\
  \u30A4\u30F3\u30C6\u30B0\u30EC\u30FC\u30B7\u30E7\u30F3\u306E\u30EC\u30D3\u30E5\u30FC"
article_id: 10525543208722
translation_id: 10525543208722
locale: ja
sidebar_position: 2
created_at: '2023-03-14T15:14:19Z'
updated_at: '2025-08-05T12:25:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: lasso
---

### ボードピッカーに警告メッセージが表示されるのはなぜですか？

埋め込むボードを選択する際に、以下のエラーメッセージが表示される場合、開いたインテグレーションはサードパーティーによって開発されたもので、Miro によるレビューが行われていません。

Board_Picker_warning_message.jpg
/em>/span>ボードピッカーの警告メッセージ

### このインテグレーションを行う場合、どのようなリスクがありますか？

ボードを埋め込む際、ボードにアクセスするためのリンク提供することになります。インテグレーションのレビューと承認が行われていない場合、そのサードパーティーのアプリがこのリンクを利用してボードにアクセスする可能性があります。

ボードを埋め込む際に提供するアクセスレベルによっては、サードパーティーのアプリにボードのコンテンツの閲覧や編集のアクセスが付与されてしまうことがあります。

### このアクセスを取り消すことはできますか？

ボード共有設定で、このインテグレーションによって生成されたリンクへのアクセスを取り消すことができます。[埋め込まれたボードへのアクセスを管理](01-user-permissions-for-boards-embedded-in-third-party-apps.md)する方法をご覧ください。

### Miro にインテグレーションのレビューをしてもらうにはどうしたらよいですか？

インテグレーションの開発者が、Miro によるレビューと承認を必要とする場合は、開発者ガイド「[Live Embed with BoardsPicker for registered users](https://developers.miro.com/docs/miro-live-embed-with-boardspicker-registered)」（登録ユーザー向けボードピッカーを使用したライブ埋め込み）をお読みください。
