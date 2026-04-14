---
title: ブラウザーで WASM がサポートされているか確認する方法
article_id: 33769132852498
translation_id: 33769132852498
locale: ja
sidebar_position: 3
created_at: '2026-03-04T12:47:24Z'
updated_at: '2026-03-16T13:02:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '実施者: すべてのユーザー 利用可能なプラン: Free, Starter, Business, Enterprise, Education 対象プラットフォーム:
    ブラウザー'
---

WebAssembly (WASM) は、組織のコンプライアンスや古い環境での非サポートなどの理由で無効化されることがあります。

> **ヒント:** [WebAssembly の比較表](https://webassembly.org/features/?categories=browsers)では、ブラウザーでサポートされる WASM 機能を確認できます。

ブラウザーが WASM をサポートしているか確認できます。

以下の手順を実施してください。

1. 開発者ツールを開きます。
   - ブラウザー内で:
     - (MacOS) Chrome, Edge, Firefox: `⌘ + ⌥ + I`
     - (Linux, Windows) Chrome, Edge, Firefox: `Ctrl + Shift + I`, または `F12`
     - (MacOS) Safari: **設定** > **詳細**に行きます。**メニューバーに"開発"メニューを表示** | **Web開発者向けの機能を表示**を有効にします。**開発**> **JavaScriptコンソールを表示**を開きます。
   - Miroのデスクトップアプリで:
     - 左上で**ヘルプ** > **開発者ツールを開く**をクリックします。
2. DevTools で **Console** タブをクリックします。
3. コンソール入力欄に `typeof WebAssembly` を入力または貼り付けます。
4. キーボードで **ENTER** を押します。
5. 結果を解釈します：
   - コンソールが `undefined` と返す場合、WebAssembly はサポートされていないか、無効化されています。
   - コンソールが`object`を返す場合、WebAssemblyはサポートされています。![](../../../../../../../docs/using-miro/troubleshooting-technical-questions/technical-guidelines/images/33770259460626_image.png)
     *DevToolsのコンソールは、*`object`*を表示し、ブラウザでWASMが利用可能であることを示します。*

     > **注意:** コンソールが`object`を返し、まだMiroにアクセスできない場合は、他の[可能な問題とトラブルシューティング](../troubleshooting)を確認するか、[Miroサポート](../../tools/troubleshooting/06-contacting-miro-support.md)に連絡してください。
