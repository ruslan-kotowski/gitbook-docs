---
title: OneLogin SSO の設定方法
article_id: 360022547134
translation_id: 360022547134
locale: ja
sidebar_position: 8
created_at: '2019-05-07T13:32:16Z'
updated_at: '2025-02-26T11:22:04Z'
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

## Onelogin の設定

### アプリの追加と設定

OneLogin の**アプリ**カタログには、事前設定され使用可能な Miro アプリがあるため、Miro への OneLogin の設定は簡単です。

Miro_in_OneLogin_apps.jpg
OneLogin アプリカタログでの Miro

**[保存]** ボタンをクリックします。

save_button.jpg
OneLogin のアプリケーション設定タブ

## Miro の設定

設定を保存すると、アプリケーション設定にそのまま誘導されます。**[SSO]** タブに切り替えて、**ログイン URL** と **x509 証明書**を取得します。

sso_tab.jpg
SSO タブ

下に URL のリストが表示されます。**SAML 2.0 エンドポイント（HTTP）**の URL をコピーします。

SAML_endpoint.jpg

そして、Miro の*SAML ログイン URL* フィールドに****貼り付け****ます。

sign-in_URL.jpg
**Miro の SAML ログイン URL フィールド**

OneLogin アプリケーション SSO タブに戻り、**[詳細を表示]** をクリックして、**x509 証明書**をコピーします。

view_details.jpg
[詳細を表示] ボタン

copy_certificate.jpg
**x509 証明書のコピー**

Miro の **x509 証明書**フィールドに、証明書を貼り付けます。

certificate_in_Miro_SSO_settings.jpg
**Miro SSO 設定の x509 証明書フィールド**

Miro の設定の最終ステップとして、ドメインを追加し、それを確認します。オプション設定を行うこともできます。

設定はすべて完了しました。これで、ユーザーは SSO を利用して Miro でユーザー認証をすることができます。

何か問題が生じた場合は、[一般的なケースのリストとその解決方法](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)をご覧ください。

## MiroでのSSO設定のテスト

1. 上記の手順を完了し、SSO 設定を構成します。
2. [**SSO 設定をテスト**] ボタンをクリックします。
3. 結果を確認してください。

- 問題が見つからなければ、「**SSO 設定のテストに成功しました**」という確認メッセージが表示されます。
- 問題が見つかった場合、「**SSO 設定のテストに失敗しました**」という確認メッセージが表示され、その後に詳細なエラーメッセージが表示されます。

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*MiroでのSSO設定のテスト*
