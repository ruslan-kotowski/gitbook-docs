---
title: Auth0 SSOの設定方法
article_id: 360022496573
translation_id: 360022496573
locale: ja
sidebar_position: 3
created_at: '2019-05-01T18:33:32Z'
updated_at: '2025-02-26T11:43:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '利用可能なプラン：: Business、Enterprise 設定者：: 会社の管理者'
---

*ブラウザーの新しいシークレットモードのウィンドウを開いて、これらの機能を設定されることを強くお勧めします。**そうすることで、標準ウィンドウでセッションを続行し、もしも誤った設定があった場合に SSO 認証をオフにすることができます。*

実際に SSO を有効にする前にテストインスタンスを設定したい場合は、営業担当者または Miro のお客様担当者にご連絡ください。SSO 設定者のみがこのテストインスタンスに追加されます。

## テナント内での Miro のアプリケーションの作成

1. **アプリケーション** リストでアプリケーションを作成します。
   create_application_button.jpg
   *Auth0 アプリケーション セクション*
2. アプリケーション タイプは **[通常の Web アプリケーション]** を選択します。
   application_types_list.jpg
   *アプリケーション タイプのリスト*
3. **[設定]** タブに移動し、以下のように、一覧表示されているオプションが正確に選択されていることを確認します。
   ![mceclip0.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725482002_mceclip0.png)


   |  |  |
   | --- | --- |
   | **トークン エンドポイントの認証方法** | POST |
   | **許可されたコールバック URL** | `https://miro.com/sso/saml` |
   | **アプリケーション ログイン URI** | `https://miro.com/sso/saml` |
   | **許可された発信元（CORS）** | `https://miro.com/` |
   | **JWT の有効期限** | 36000 (デフォルトで設定) |
4. **[詳細設定を表示]** をクリックします。
   ![mceclip1.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017725485074_mceclip1.png)

   次に **[証明書]** に移動し、x509 署名証明書をコピーします。
   copy_the_certificate.jpg
   *Auth0 の詳細設定タブ*
5. Miro に切り替えて、アカウント SSO 設定（Business プランの管理者は **[セキュリティ]** タブに設定が表示され、Enterprise プランの管理者は **[Enterprise のインテグレーション]** タブに移動する必要があります）を開き、以下のスクリーンショットに示すように、**x509 署名証明書**をそれぞれのフィールドに貼り付けます。
   certificate_in_Miro_SSO_settings.jpg
   *SAML 設定の Miro の**セキュリティ**タブ*

## アプリケーションに SAML を設定

1. Auth0 アプリケーション設定ページに戻り、**[アドオン]** タブと **SAML2** アドオンのトグルを有効にします。
   add-ons_catalog.jpg
   *Auth0 アドオンカタログ*

   リクエスト設定とアプリケーション コールバック URL/em> が表示されたポップアップ ウィンドウが表示されます。
   add-on_settings.jpg
   *アドオン設定タブ*/strong>
2. **URL**が **`https://miro.com/sso/saml` に設定されていることを確認します**

   リクエストの設定/strong>は、次のように設定する必要があります。

   ```
    "nameIdentifierFormat": "urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress"、
    "nameIdentifierProbes"：[
    "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/emailaddress"
   ```
3. タブを **[使用状況]** に切り替えて、**ID プロバイダーのログイン URL** をコピーします。
   ![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017695812626_mceclip2.png)mceclip2.png
   *Auth0 の ID プロバイダーのログイン URL フィールド*
4. 再度 Miro に切り替えて、**SAML ログイン URL** フィールドに URL を貼り付けます。
5. Miro のプランに設定を適用するには、**[保存]** をクリックします。

## 設定の確認

これで、Auth0 コンソールに戻り、アドオンの **[設定]** タブに切り替えることができます。[デバッグ] をクリックして、ログイン試行をトリガーします。

debug.jpg
ログイン試行のトリガー

これにより、IDP ログイン試行が開始され、結果を確認することができます。

何らかの問題が発生した場合、お気軽に[サポートチームまでご連絡](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)ください。

## MiroでのSSO設定のテスト

1. 上記の手順を完了し、SSO 設定を構成します。
2. [**SSO 設定をテスト**] ボタンをクリックします。
3. 結果を確認してください。

- 問題が見つからなければ、「**SSO 設定のテストに成功しました**」という確認メッセージが表示されます。
- 問題が見つかった場合、「**SSO 設定のテストに失敗しました**」という確認メッセージが表示され、その後に詳細なエラーメッセージが表示されます。

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*MiroでのSSO設定のテスト*
