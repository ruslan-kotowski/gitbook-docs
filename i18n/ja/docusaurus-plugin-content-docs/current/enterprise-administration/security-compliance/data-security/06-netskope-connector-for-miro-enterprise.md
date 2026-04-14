---
title: "Miro Enterprise \u7528\u306E Netskope \u30B3\u30CD\u30AF\u30BF\u30FC"
article_id: 4415711060498
translation_id: 4415711060498
locale: ja
sidebar_position: 6
created_at: '2022-01-19T06:23:42Z'
updated_at: '2025-02-26T11:27:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Miro の Netskope 用カスタムコネクターを使用して、データ漏洩に関わる事態を可視化し、Miro 内で以下のトラフィックを管理することができます。

- [ボードのバックアップのダウンロード](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md)

このガイドでは、Miro Enterprise プラン用に Netskope を設定する手順と、ユーザー エクスペリエンスについて説明します。

> **利用可能なプラン：**[Enterprise プラン](../../../plans-billing/miro-plans/04-enterprise-plan.md)

### Netskope での Miro アプリの新規作成

Netskope インスタンス内で、**[設定] > [セキュリティークラウド プラットフォーム] > [アプリの定義]** に移動し、**[新しいクラウドアプリ]** をクリックします。

new_cloud_app.jpg
![Netskope でクラウドアプリの作成](blob:https://miro.atlassian.net/8cb061a4-e184-4bd6-bb95-774cd34fc8e7#media-blob-url=true&id=78b7a8cb-792a-41da-bf16-b26ca4480059&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.08.43.png&size=181298&height=513&width=1028&alt=)

Netskope 内で新しいアプリを作成するには、次の JSON ファイルの **miro-activities-for-netskope.json** をインポートするよう求められます。

```
バージョン：3.

"ドメイン名": "miro.com"、
"uri_path": "/api/v1/boards/.+/"、
「http_method」：お大事に
"uri_param"：{ "key": "archive", "value": "true" }]、
"resp_code"：3.
"パターン": ""、
「アクティビティ名ダウンロード


"ドメイン名": "miro.com"、
"uri_path": "/api/v1/boards/.+/resources/.+/files/original"、
「http_method」：お大事に
"uri_param"：[],
"resp_code"：3.
"パターン": ""、
「アクティビティ名ダウンロード
```

アプリケーション名を入力し、**[Custom Connector]** オプションを選択して、**[IMPORT FROM FILE] > [Add To Activity List]** をクリックし、前の手順でダウンロードした **miro-activities-for-netskope.json** ファイルをアップロードします**。**

uploading_the_file.jpg
ファイルのアップロード

**miro-activities-for-netskope.json** ファイルをインポートすると、記録されたアクティビティが表示されます。これで、**[保存]** をクリックして Miro アプリを作成することができます。

save_the_app.jpg
![アプリの保存](blob:https://miro.atlassian.net/b9da4e19-b3b1-4c25-aed3-762f458fd639#media-blob-url=true&id=f7549007-0265-42e1-b946-a3e167124f12&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.26.58.png&size=209044&height=693&width=1028&alt=)

アプリが作成されると、それを選択して **[変更を適用]** をクリックする必要があります。

apply_changes.jpg
/strong>Miro アプリに変更を適用するオプション

![](blob:https://miro.atlassian.net/82b8ac6e-1952-44e7-a62f-cefb7dbee6ab#media-blob-url=true&id=975f42e8-de5d-4bbb-ae07-c243cce9bb2f&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.32.06.png&size=257154&height=575&width=1780&alt=)

### Netskope で Miro アプリの新しいポリシーを作成

アプリケーションが作成されると、ポリシーの作成に進むことができます。そのためには、**[ポリシー]** > **[リアルタイムの保護]** に移動して、**[新しいポリシー] > [クラウドアプリへのアクセス]** をクリックします。

create_a_policy.jpg
![Miro アプリ用ポリシーの作成](blob:https://miro.atlassian.net/d2ae8479-8f5c-4417-8b09-2b57ee344d90#media-blob-url=true&id=e9c82ee5-cdea-4b33-8491-9613a848be81&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.39.02.png&size=107320&height=321&width=635&alt=)

ここの**保存先**で、前の手順で作成した Miro アプリを提供し、**ポリシー名**を設定して **[保存]** をクリックする必要があります。

save_the_policy.jpg
/strong>ポリシーの保存

![](blob:https://miro.atlassian.net/abf26593-27ad-40f4-b3e5-731a9e58d062#media-blob-url=true&id=0edd2e23-2762-4173-8f3f-9a7bb74bf217&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2017.45.14.png&size=200430&height=722&width=1575&alt=)alt次に、ポリシーを配置する場所を選択してalt [保存] をクリックします。

move_policy.jpg
ポリシーを配置する場所を選択

最後に、**[変更を適用]** ボタンをクリックして変更を適用します。

applying_changes.jpg
変更の適用

![](blob:https://miro.atlassian.net/41cdf802-aa1c-4f9a-bd22-950ea6ad755e#media-blob-url=true&id=7f85d987-6550-4271-90da-c9273a0cbc9a&collection=contentId-2403139769&contextId=2403139769&mimeType=image%2Fpng&name=Screenshot%202021-12-16%20at%2019.29.17.png&size=157218&height=490&width=1576&alt=)

### イベントの可視化

設定が完了したら、**[Skope IT]** に移動し、カスタマイズされた Miro アプリでフィルタリングし、以下のように **[イベントを表示]** をクリックしてトラフィックを可視化できます。

see_events.jpg
トラフィックイベントを表示するオプション

### ユーザー エクスペリエンス

ダウンロード アクティビティーをブロックするユーザーは、Netskope クライアントがマシンにインストールされている必要があります。ユーザーがダウンロード バックアップ操作を試みると、Netskope はアクションをブロックし、メッセージ付きのネイティブ OS ポップアップを表示します。

alert.jpg
Miro ボードのバックアップのダウンロードが許可されていないユーザーに表示されるメッセージ
