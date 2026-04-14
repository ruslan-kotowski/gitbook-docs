---
title: 2 要素認証（2FA）
article_id: 27356474050834
translation_id: 27356474050834
locale: ja
sidebar_position: 1
created_at: '2025-06-12T12:01:03Z'
updated_at: '2025-06-24T08:19:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: '実行可能なユーザー：: チームの管理者、会社の管理者 利用可能なプラン：: Starter、Business、Education、Enterprise
    利用可能なプラットフォーム：: ブラウザー、デスクトップ、モバイル'
---

2 要素認証（2FA）は、ユーザーがアカウントにアクセスする前に、2 つの異なる確認方法を提供するよう要求することで、オンラインアカウントに追加のセキュリティレイヤーを加えます。

Miro の管理者は、チームの 2FA を有効化でき、チームメンバーの 2FA をリセットすることができます。ユーザーはデバイスを30日間信頼するオプションがあります。

:::note
この記事では、Starter、Business、Education プランにおける2FAについて説明します。Enterprise の 2FA について学ぶには、[2 要素認証（2FA）（管理者ガイド）](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)をご覧ください。
:::

## 2 要素認証を有効化する

Starter プランと Education プランの場合、チームの管理者ロールを持つことを確認してください。

Business プランの場合、会社の管理者の役割を持っていることを確認してください。

以下の手順に従ってください。

1. Miro のダッシュボードから、右上にある自分のアバターをクリックし、**管理者コンソール**を選択します。
2. (Starter) **セキュリティ** > **管理者権限**に移動します。
   **[アクセス権限]**に移動します。
   **Security** > **認証** に移動します。
3. **2 要素認証 (2FA)** の下で、**ログイン時に 2 要素認証を要求する** をオンにします。

## ユーザー向けの 2 要素認証（2FA）設定

2FA を有効にしているチームでは、ユーザーはメールアドレスとパスワードに加えて、認証アプリを使用して認証しなければなりません。

[2 要素認証（2FA）– ユーザーガイド](02-two-factor-authentication-2fa-–-user-guide.md)をご覧いただき、ユーザーとして 2FA を設定する方法を学んでください。

## 信頼済みデバイス

ユーザーが 2FA で Miro にログインするとき、デバイスを信頼することを選択できます。

信頼されたデバイスを使用してログインする場合、ユーザーはそのデバイスが信頼されているため、最初の要素での認証だけを求められ、2 番目の要素はスキップされます。

![](../../../../../../docs/administration/security-compliance/images/27358547112978_image.png)

*2FA の信頼できるデバイスはデフォルトで有効化されています。*

ログイン時に、**このデバイスを30日間信頼する**がデフォルトで選択されていますが、ユーザーはオプションで選択を解除できます。

> 信頼デバイス期間は Enterprise プランでのみ変更可能です。詳細は、[2 要素認証（2FA）（管理者ガイド）](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)をご覧ください。

ユーザーが誤って信頼してしまったデバイスの信頼を解除するには、すべての場所から自分自身をログアウトすることができます。**プロフィール**に移動し、**プロフィールの設定**の下で、**すべての場所からログアウト**をクリックします。

## 2 要素認証をリセット

ユーザーが第 2 要素へのアクセスを失った場合、管理者に 2FA のリセットを依頼できます。

Starter と Education プランのユーザーの 2FA をリセットするには、チームの管理者の役割を持っていることを確認してください。

Business プランのユーザーに対して 2FA をリセットするには、会社の管理者の役割を持っていることを確認してください。

以下の手順に従ってください。

1. Miro のダッシュボードから右上のアバターをクリックし、**管理者コンソール**を選択します。
2. **ユーザー** >**すべてのユーザー** に移動します。
3. ユーザーを見つけてから、行の最後にある**三点リーダー**を選択します。
4. **2 要素認証をリセット**をクリックします。
   ユーザーがメールでリセットの手順を受け取ります。
