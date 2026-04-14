---
title: "\u516C\u958B\u30DC\u30FC\u30C9\u306E\u30D1\u30B9\u30EF\u30FC\u30C9\u4FDD\u8B77"
article_id: 360014617239
translation_id: 360014617239
locale: ja
sidebar_position: 13
created_at: '2020-06-22T10:42:25Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
---

有料プランのパスワード保護機能を確認して、公開ボードのパスワードの設定方法をご覧ください。

> **実行可能なユーザー：**ボード所有者、[ボード共同所有者](06-co-owners-of-boards-and-spaces.md)、[コンテンツ管理者](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)権限を持つ Enterprise プランの会社の管理者
> **対象プラン：Starter、Business、Enterprise、Education
> **実行可能な環境：**ブラウザー、[デスクトップアプリ](../../getting-started/apps-for-devices/05-desktop-app.md)、[タブレットアプリ](../../getting-started/apps-for-devices/11-tablet-app.md)**

## 公開ボードのパスワード

公開リンクを使ってボードにビジターを招待することは、チームや会社以外のユーザーと即座に行える、一度限り、または短期間のコラボレーションのための素晴らしいオプションです。Miro を利用していないユーザーも公開ボードにアクセスできます。

Miro の公開ボードを共有する場合、パスワード設定によりセキュリティ層を追加できます。

### プランに基づいてパスワードを保護

パスワード保護やアクセス権限のレベルは、プランの種類によって異なります。

|  |  |  |  |
| --- | --- | --- | --- |
|  | **Free** | **Starter、Business** | **Enterprise** |
| **パスワードの有効化、変更、または削除** | ✘ | ✔  ボード所有者、共同所有者 | ✔  ボード所有者、共同所有者、会社の管理者* |
| **必須パスワードの有効化** | ✘ | ✘ | ✔  [必須パスワードの設定](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) |
| **複雑なパスワードを要求** | ✘ | ✘ | ✔  [複雑なパスワードを要求](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) |

*[コンテンツ管理者](../../enterprise-administration/managing-enterprise-teams-and-content/12-content-admin-permissions.md)権限の有効化が必要です。


> [️✏️ Enterprise プランの共有ポリシーの詳細についてはこちらをご覧ください。](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)

## ボードにパスワード保護を追加する方法

1. [リンクを知る全員]/span> のアクセス権を有効にする場合、**[パスワードを設定]** ボタン**をクリックします**

2. 8文字以上の強力な英数字のパスワードを入力し、**Setを**クリックします。

3. パスワードはクリップボードにコピーされます

*![3-1-720p-10fps-s4-r20.gif](../../../../../../docs/using-miro/sharing-boards/images/20257248240274_3-1-720p-10fps-s4-r20.gif)
リンクで共有されているボードのパスワード設定*

> [✏️ Enterprise プランの管理者は、サブスクリプションのすべてのボードに必須パスワードを設定することが可能です。](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)

## ユーザー向けのパスワード保護の機能

ボードのリンクを受け取り、開くと、ビジターはパスワードの入力を求められます。

![3-2-720p-10fps-s4-r20.gif](../../../../../../docs/using-miro/sharing-boards/images/20257248243730_3-2-720p-10fps-s4-r20.gif)

パスワードを入力すると、ボードにフルアクセスできるようになります。72 時間ごとにパスワードを再入力するだけでいいのです。

頻繁なログインが必要な場合、Miro の管理者が[セキュリティーを追加するために](../tools/troubleshooting/19-why-does-miro-keep-logging-me-out.md)アイドルセッション タイムアウトを有効にしている可能性があります。

ボードがパスワードで保護されている場合、そのボードはスター付きリストと最近のリストに表示されます。

ユーザーのセッションが終了すると、ボードは利用できなくなり、スター付きリストと最近使ったリストから削除されます。ユーザーがダイレクトリンクでボードを開き、ボードパスワードを再入力すると、ボードは関連リストに再び表示されます。

## 公開ボードのパスワード変更

パスワードを変更すると、現在ボードに参加している場合でも、すべてのボードのビジターが即座にアクセスできなくなります。

:::note
️ パスワードで保護されたボードへのリンクを共有できるユーザーは、ボード所有者や共同所有者でない限り、パスワードを変更することはできません。
:::

**公開ボードのパスワードを変更するには：**

1. 共有設定の「パスワードを編集/span>」 **をクリックし、「パスワードを変更」をクリックします。
![](../../../../../../docs/using-miro/sharing-boards/images/20235526720658_3-1.png)3-1.png
*共有設定でボードのパスワードを編集*
2. 確認ウィンドウが表示され、ボードへのアクセスを継続するために、新しいパスワードを既存の共同作業者と共有する必要があることを通知します。[パスワードを変更] をクリックします。**

![change_password.png](../../../../../../docs/using-miro/sharing-boards/images/20022115780754_change_password.png)
*パスワード変更の確認画面*
3. 英数字 8 文字以上の強力なパスワードを入力してください。
管理者がアカウントに特定のパスワード要件を設定している場合があります。パスワードを作成すると、必要な条件が明確に表示されます。
![パスワードを入力すると、必要なパスワードが表示されます。](../../../../../../docs/using-miro/sharing-boards/images/23762870609298_image.png)*パスワードを入力すると、必要なパスワードが表示されます。*

4. **パスワードの設定**］をクリックします。

:::note
パスワードを変更すると、現在ボードに参加している場合でも、すべてのボードのビジターが即座にアクセスできなくなります。
:::

## 公開リンクの無効化

[公開ボードの共有停止](03-sharing-boards-and-inviting-collaborators.md)はいつでもできますが、ボードのパスワードが自動的にリセットされるわけではありません。ビジターが同じパスワードでボードにアクセスできるようにするには、再度リンクでボードを共有する必要があります。

パスワードの変更については、公開ボードのパスワード変更をご覧ください。

## ボードのパスワードを忘れてしまいました

パスワードを忘れた場合、共有設定で簡単にボードのパスワードを変更することができます。


:::note
モバイルで利用するボードのパスワード保護設定は現在取り組み中です。
:::
