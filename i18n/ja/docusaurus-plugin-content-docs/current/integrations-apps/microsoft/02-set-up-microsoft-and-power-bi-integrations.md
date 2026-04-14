---
title: Microsoft と Power BI のインテグレーションを設定する
article_id: 25132703621394
translation_id: 25132703621394
locale: ja
sidebar_position: 3
created_at: '2025-03-06T10:27:14Z'
updated_at: '2025-11-25T15:49:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
availability:
  notes: 包括的な管理者向け文書をお探しの場合、特に Miro の Microsoft や Power BI とのインテグレーションについて、詳細な図表や追加の
    FAQ を含む[Microsoft の管理者向け文書](https://docs.google.com/document/d/1Gw94z5Pc-elS-pRXKGZVBWKKNEIFR9y9yzAAkbXKwMM/edit?usp=sharing)や[Power
    BI の管理者向け文書](https://docs.google.com/document/d/1hMepF163jQF8LI-U8ES8DzHVMW4TltXDr14fJ2KU29k/edit?tab=t.0#heading=h.gu9ng058yy7y)をご参照ください。
---

この記事では、Microsoft または Power BI インテグレーションを Miro で設定する方法について説明します。

## Microsoft または Power BI インテグレーションを設定する

Microsoft または Power BI のインテグレーションを設定するには、Miro 内でユーザー自身の Microsoft または Power BI コンテンツを認証できるようにする必要があります。

### 前提条件

- Microsoft Entra の管理者アクセス権を持っていることを確認してください。
- 会社の管理者が、Miro 組織のために Microsoft または Power BI を承認しました（これは、組織がアプリのインストールを制限している場合、Miro 側のアプリ承認ポリシーを指します）。

### 手順

これらの手順は、Miro インテグレーションを許可するために Microsoft Entra を設定することに焦点を当てています。

1. **Entra** に管理者としてログインする
2. **エンタープライズ アプリケーション** > **同意と権限** に移動します。
3. **ユーザーが同意できないアプリに対して管理者に同意を求めることができます**では、**はい**を選択します。
4. **管理者承認リクエストを確認できる人**の下で、アプリケーションの管理者承認リクエストをレビューすることを許可する必要があるユーザー、役割、またはグループを選択します。

:::note
上記の手順 4 で指定された Entra 管理者は、その後 Microsoft Entra の**Enterprise アプリケーション > 管理者の同意要求**に移動して、組織の "Contenthub PowerBI Integration"（または同様の名前の）アプリケーションをレビューおよび承認することができます。
:::

## Microsoft または PowerBI インテグレーションを検証してください

Miro ボードにリンクをコピーして貼り付けます。

アプリが会社の管理者によって事前承認されている場合は、画面のモーダル指示に従ってください。MiroはあなたのアプリのコンテンツをiFrameとしてボードに追加します。

アプリが事前承認されていない場合、**追加と許可**モーダルが開き、会社の管理者にリクエストを送信できるようになります。リクエストを送信してください

会社の管理者が返信すると、通知が届きます。

**詳細:**[アプリ管理](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md)をご覧ください。
