---
title: AWS SSO の設定方法
article_id: 360014798100
translation_id: 360014798100
locale: ja
sidebar_position: 4
created_at: '2020-07-01T20:03:44Z'
updated_at: '2025-02-26T11:33:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '利用可能なプラン：: [エンタープライズ](../../../plans-billing/miro-plans/04-enterprise-plan.md),[ビジネス](../../../plans-billing/miro-plans/06-business-plan.md)プラン
    設定者：: 会社の管理者'
---

> *お使いのブラウザーのシークレットモードのウィンドウを新たに開けて、SSO を設定することを強くお勧めします。*そうすることで、セッションを標準ウィンドウに保ち、誤った設定があった場合に、SSO 認証をオフにすることができます。

実際に SSO を有効にする前にテストインスタンスを設定したい場合は、アカウント担当者または営業担当者にご連絡ください。SSO 設定者のみがこのテストインスタンスに追加されます。

> **⚠️ ルール、サポートされている機能、Miro 側でのオプション設定については、SSO に関する主要記事を**[**こちら**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)**でご覧ください。**

## 前提条件

Miro を使用して AWS SSO アクセスを設定するには、以下が必要になります。

1. アプリケーションを管理するための IAM アクセス権限がある AWS SSO コンソールへのアクセス
2. Miro の Enterprise、または Business プランの会社レベルの管理者権限

## 設定手順

1. AWS SSO の設定ページで、新しいアプリケーションを追加し、**Miro** を検索します。  Miro アプリケーションを追加する際に、表示名と詳細情報を更新することができます。
   application_catalog.jpg
   /em>AWS SSO アプリケーション カタログ/span>
2. 別のブラウザーウィンドウで Miro のダッシュボードにログインします。別のシークレットモードのブラウザーウィンドウを開けることをお勧めします。/span>
3. 右上のプロフィールアイコンをクリックし、**[設定]** に移動します。左側のパネルで、左上のドロップダウン メニューから正しいチームを選択していることを確認します。
4. 左側のパネルで、**[Enterprise のインテグレーション]**（Business プランのユーザーの場合は **[セキュリティー]**）に移動し、**SSO/SAML を有効にする**オプションに切り替えます。AWS SSO から SAML ログイン URL に以下の値を入力します。

application_configuration_page.jpg
AWS SSO アプリケーションの設定ページ

5. AWS SSO SAML メタデータファイルをダウンロードして、X509 認証を **x509 キー認証**にコピー＆ペーストします。Miro の設定は、以下のようになるはずです。

Miro_SSO_settings.jpg
Miro SSO の構成設定

6. Miro の SSO 設定で、会社のメールドメイン名を**ドメイン**の値に入力します。 会社のドメインが少なくとも 1 つ追加されていることを確認します。
7. **[保存する]** をクリックして、変更内容を保存します。
8. AWS SSO のウェブコンソールで Miro のアプリケーションに戻ります。アプリケーション メタデータで、次の値が入力されていることを確認します。カスタム アプリケーションを作成する代わりに Miro アプリケーションを検索して追加すると、それは自動的に取り込まれるはずです。
9. |  |  |
   | --- | --- |
   | **フィールド** | **値** |
   | アプリケーション ACS URL | [https://miro.com/sso/saml](https://Miro.com/sso/saml) |
   | アプリケーション SAML オーディエンス | https://miro.com/ |
10. **[変更を保存]** を選択します。
11. AWS SSO コンソールのアプリケーションの [割り当て済みユーザー] で、アプリケーションに[ユーザーを割り当てます](https://docs.aws.amazon.com/singlesignon/latest/userguide/assignuserstoapp.html)。

以上でSSO の設定が完了しました。

Miro の自動プロビジョニングを有効化したい場合は、こちらの記事をご覧ください。

## テスト中

次のセクションを使用して、SSO のインテグレーションを検証します。検証前に、検証を行うユーザーが、AWS SSO と Miro の両方からログアウトしていることを確認してから、以下の手順を実行してください。ユーザーはディレクトリーに存在するか、Miro の Enterprise または Business プランのメンバーであるか、ユーザーがアプリケーションに割り当てられているかのいずれかでない限り、SSO を使用してログインすることはできません。/span>

### AWS SSO から IdP を起動した SSO の検証

1. Miro のアプリケーションに割り当てられたユーザーの資格情報を使用して、AWS SSO エンドユーザー ポータルにアクセスします。
2. アプリケーションの一覧で、Miro アプリケーションを選択して、Miro にログインを開始します。
3. ログインが成功すると、Miro のダッシュボードにログインされます。

### Miro からサービスプロバイダーを起動した SSO の検証

1. [https://miro.com/login/](https://Miro.com/login/)にアクセスし、**[SSO でログイン]** を選択します。次に、仕事用のメールアドレスを入力します。
2. AWS SSO ポータルに転送され、AWS SSO コンソールでアプリケーションに割り当てられたユーザーの資格情報を入力します。
3. ログインが成功した場合、Miro のダッシュボードにログインします。

### あるいは、Miroでテストすることもできます。

1. 上記の手順を完了し、SSO 設定を構成します。
2. [**SSO 設定をテスト**] ボタンをクリックします。
3. 結果を確認してください。
   1. 問題が見つからなければ、「**SSO 設定のテストに成功しました**」という確認メッセージが表示されます。
   2. 問題が見つかった場合、「**SSO 設定のテストに失敗しました**」という確認メッセージが表示され、その後に詳細なエラーメッセージが表示されます。![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*MiroからのSSO設定のテスト*

## トラブル シューティング

一般的なトラブルシューティングの問題については、[AWS SSO のトラブルシューティング ガイド](http://docs.aws.amazon.com/singlesignon/latest/userguide/troubleshooting.html)を参照してください。
