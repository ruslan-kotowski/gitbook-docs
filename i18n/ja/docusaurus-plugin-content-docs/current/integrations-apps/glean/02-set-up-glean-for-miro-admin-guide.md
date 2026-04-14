---
title: "Miro \u7528 Glean \u3092\u8A2D\u5B9A\uFF08\u7BA1\u7406\u8005\u30AC\u30A4\u30C9\
  \uFF09"
article_id: 27581463837330
translation_id: 27581463837330
locale: ja
sidebar_position: 2
created_at: '2025-06-23T10:52:57Z'
updated_at: '2026-01-02T09:57:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

前提条件

1. あなたは**Miro 組織管理者**および**Glean 管理者**です。
2. Glean で、**OAuth クライアント ID を登録**します。詳しくは[Glean ドキュメント](https://developers.glean.com/api-info/client/authentication/oauth)を参照してください。
3. ユーザーレベルのプライバシー設定**チャット履歴を最大 30 日間保存を許可する**を有効にします。

## Glean アプリをインストールする

まず、Glean アプリを Miro マーケットプレイスから組織の該当チームにインストールしてください。

1. 「**会社**」設定に移動し、「**アプリとインテグレーション**」をクリックします。
2. 「**アプリ**」タブで「**アプリ追加**」をクリックし、マーケットプレイスを開きます。
3. 「Glean」を検索します。また、そのクライアント ID を検索バーに貼り付けて見つけることもできます: `1202342442818548396`。
4. アプリのプロフィールから、アプリを追加する場所を選択します。「**すべてのチーム**」または「**特定のチーム...**」から選べます。
5. 権限ページを確認します。「Glean」アプリはMiroによって開発・管理されており、特定の権限を求めません。
6. **追加**を選択してインストールを完了します。

## シングルサインオン設定 (Okta)

組織がOktaをシングルサインオン（SSO）プロバイダーとして使用している場合は、次のセクションに進む前にOkta OpenID Connect (OIDC) Webアプリケーションを作成する必要があります。

1. こちらの[ドキュメント](https://help.okta.com/en-us/content/topics/apps/apps_app_integration_wizard_oidc.htm)に記載されている手順に従って、新しいOktaアプリを作成します。
   1. **OIDC - OpenID Connect** をログイン方法として選択します。
   2. **Web アプリケーション** をアプリケーションタイプとして選択します。
   3. **Grant type** > **Core grants** 設定で **Refresh Token** が有効になっていることを確認します。
   4. **Sign-in redirect URIs** に `https://integrations.miro.com/api/external-auth/oauth2/callback` を追加します。
   5. **保存** を選択します。
2. クライアント認証情報セクションから**ClientId**と**Client Secret**をコピーしてください。これらはインテグレーション設定を完了するために次のセクションで必要になります。

## シングルサインオン（SSO）の設定

アプリの設定を行うには、以下の手順に従ってください。

1. **Apps & Integrations**ページから**Manage apps**へ移動します。
2. インストール済みアプリのリストから「Glean」を見つけて、その**設定**をクリックします。アプリが見つからない場合は、クライアントID（`1202342442818548396`）で検索して、まず承認してください。
3. 設定で**SSO プロバイダー**を選択します。
   1. Okta
   2. Azure
   3. Google
4. 必要な SSO の詳細を入力します。
   1. Okta: **Glean ベース URL**、**Okta アプリの詳細 (認証サーバー URL**、**アクセストークン URL**、**クライアント ID**、**クライアント シークレット)**。
   2. Azure: **Glean ベース URL**。
   3. Google: **Glean ベース URL**。
5. **保存**をクリックして構成を適用します。

:::note
Azure を使用している場合、Microsoft Entra 管理者が Microsoft Entra 管理センターで Glean アプリに対して「組織を代表して同意する」を選択し、ユーザーが正しく認証できるようにしてください。
:::

## Glean 管理者コンソールの設定

Miro で Glean を使用する前に、Glean 管理者コンソールで OAuth トークンベースのアクセスを設定する必要があります。

1. **Glean管理者コンソール**を開き、**設定** > **サードパーティアクセス（OAuth）**へ移動します。
2. **IDP設定済みOAuth**セクションで、**APIアクセス用のIDP OAuthを有効にする**を有効にします。
3. **設定を管理**をクリックし、**SSOプロバイダー**を選択します。
4. SSOプロバイダーに基づいてプロバイダーの詳細を入力します。
   - **Okta**
     - 認証サーバーURL: `https://<subdomain>.okta.com`
     - 許可されたクライアントID: 前のセクションで作成したOktaアプリのクライアントID。
     - そのほかのフォームの項目は空白のままにしておいてかまいません。
   - **Azure**
     - 発行者サブドメイン: `https://login.microsoftonline.com/<tenant-id>/v2.0`
     - 許可されたクライアント ID: `a49fdb25-3b5f-4d3b-bedf-6da7be2b4bf4`
   - **GSuite**
     - 許可されたクライアント ID: `1062019541050-pf2ndc9f3o4lrmkupj3cj0fep5hkecns.apps.googleusercontent.com`
5. 設定を適用するには**保存**を選択します。

> ⏰ **注:** Glean 管理者コンソールで変更が反映されるまで最大30分かかることがあります。

セキュリティー

データとセキュリティーに関する詳細については、[このセキュリティー文書](https://docs.google.com/document/d/1lGLF7eASQb2uMRmMEAaH-GzFhyz4UKfwMeqSQOSYPdM/edit?tab=t.0#heading=h.gu9ng058yy7y)をご覧ください。
