---
title: OKTA SSO の設定方法
article_id: 360023901054
translation_id: 360023901054
locale: ja
sidebar_position: 7
created_at: '2019-05-31T11:32:41Z'
updated_at: '2025-11-25T16:05:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '利用可能なプラン：: [エンタープライズ](../../../plans-billing/miro-plans/04-enterprise-plan.md),[ビジネス](../../../plans-billing/miro-plans/06-business-plan.md)プラン
    設定者：: 会社の管理者'
---

> *お使いのブラウザーのシークレットモードのウィンドウを新たに開けて、SSO を設定することを強くお勧めします。*そうすることで、セッションを標準ウィンドウに保ち、誤った設定があった場合に、SSO 認証をオフにすることができます。

[本番環境で SSO を有効にする前にテストインスタンスを設定したい場合は、サポートチームまでご連絡ください。](https://help.miro.com/hc/requests/new?referer=help-center-article)SSO 設定者のみがこのテストインスタンスに追加されます。

> **⚠️ ルール、サポートされている機能、Miro 側でのオプション設定については、SSO に関する主要記事を**[**こちら**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)**でご覧ください。**

## Okta のセットアップ

### アプリの追加と設定

**[アプリケーション]** タブをクリックして、**[Browser App Catalogue（アプリのカタログを参照）]** を選択します。

browse_app_catalog.jpg
Okta のアプリケーション セクション

セットアップを簡略化するための事前設定がなされたアプリのリストから、必要なアプリを見つけて、**[Add]（追加）**をクリックします：

Miro_pre-configured_app.jpg
Okta アプリカタログ内の Miro

ギャラリーアプリにお好みのラベルを付け（他のステップは任意）、**[Next]（次へ）**をクリックして **[Sign-On options]（サインオンオプション）**タブに切り替えます：

general_settings.jpg
Miro アプリの一般設定

**サインオンオプション**では、予想される値はすべて入力されているため、データを追加する必要はありません。

:::warning
希望する値を追加することもできますが、**デフォルトのリレー状態**は*空欄*のままにしておきます。Miro のスタンドアローン アプリでは、認証手順にエンドユーザーのブラウザーへのリダイレクトを採用しており、その際に、固有のリレー状態の値が生成されるためです。この設定でデフォルトの値を使用すると、Okta は Miro のデータを上書きし、ユーザーは Miro のブラウザー版だけにアクセスし、デバイス（デスクトップ、タブレット、モバイル）のスタンドアローン アプリにアクセスすることはできません。
:::

sign-on_options.jpg
サインオン方法

**[Finish]（終了）**をクリックします。必要に応じて、後でフィールドに戻って編集することができます。

### ユーザー名の形式

> **アプリケーションのユーザー名の形式**は、デフォルトで **Okta ユーザー名**に設定されているため、ユーザー名がメールアドレス形式であれば問題ありません。また、ユーザー名を**メールアドレス**に設定することもできます。

:::warning
メールアドレスは、Miro 側でユーザーを認識するためのプライマリー ID として使用されており、SCIM が有効化されていない限り、Okta 側で更新するべきではありません。SCIM を使用せずにエンドユーザーのメールアドレスを更新する必要がある場合は、Miro の[サポートチーム](https://help.miro.com/hc/requests/new?)にご連絡ください。
:::

### プロフィール画像の設定（オプション）

ProfilePicture などのカスタマイズ可能な属性の設定は、別の手順として捉えます。プロフィール画像を設定するには、こちらの[ガイド](https://drive.google.com/file/d/1go4BJWzFpQS5R04WdN1Q4O5Dy93k4wGp/view)に従って、Okta 側の属性を設定してから、Miro 側の [ProfilePicture の要件を有効化](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)します。

## Miro の設定

**SMAL 署名証明書**までスクロールダウンして、IDP メタデータを取得します。発行済みの証明書がない場合は、先に証明書を作成します。

その後、**[Actions]（アクション）**をクリックして、以下の通り **[View IdP metadata]（IdP メタデータを表示）**を選択します：

view_Idp_metadata.jpg
IdP メタデータの取得

情報を containsAll した別のタブが表示されます。&lt;ds:X509Certificate&gt; で始まる行の証明書をコピーし、Miro SSO 設定セクションの「Key x509 Certificate」（X.509 証明書）/span>の**入力欄に貼り付けます。**

certificate_in_Miro_SSO_settings.jpg
/span>Miro SSO 設定セクションの主な X.509 証明書

メタデータページに戻り、**SingleSignOnService** の行の **Location=** の後にある URL をコピーして、**[SAML ログイン URL]** に貼り付けます。

これで設定は完了です。

Miro の設定の最終ステップとして、ドメインを追加し、それを確認します。オプション設定を行うこともできます。

何か問題が生じた場合は、[一般的なケースのリストとその解決方法](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)をご覧ください。

## MiroでのSSO設定のテスト

1. 上記の手順を完了し、SSO 設定を構成します。
2. [**SSO 設定をテスト**] ボタンをクリックします。
3. 結果を確認してください。

- 問題が見つからなければ、「**SSO 設定のテストに成功しました**」という確認メッセージが表示されます。
- 問題が見つかった場合、「**SSO 設定のテストに失敗しました**」という確認メッセージが表示され、その後に詳細なエラーメッセージが表示されます。

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*MiroでのSSO設定のテスト*
