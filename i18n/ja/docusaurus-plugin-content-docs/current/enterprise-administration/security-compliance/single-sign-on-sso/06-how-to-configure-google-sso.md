---
title: Google SSO の設定方法
article_id: 4716499382546
translation_id: 4716499382546
locale: ja
sidebar_position: 6
created_at: '2022-03-18T18:12:44Z'
updated_at: '2025-11-25T16:08:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '利用可能なプラン：: Business、Enterprise 設定者：: 会社の管理者'
---

> お使いのブラウザーのシークレットモードのウィンドウを新たに開けて、SSO を設定することを強くお勧めします。そうすることで、セッションを標準ウィンドウに保ち、誤った設定があった場合に、SSO 認証をオフにすることができます。

GoogleがGoogle Workspace Admin Console内に作成したインテグレーションアプリを使用すると、組織内でのMiroの設定がこれまで以上に簡単になります。このアプリを使用すると、Miroで使用するGoogle SSOや[SCIMユーザープロビジョニングを](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md)設定できます。

この記事では、Miroで使用するためのGoogle SSOの設定に焦点を当てます。

実際に SSO を有効にする前にテストインスタンスを設定したい場合は、アカウント担当者または営業担当者にご連絡ください。SSO 設定者のみがこのテストインスタンスに追加されます。

:::tip
ルール、サポートされる機能、オプションの構成設定については、Miro[SSOの記事を](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) 参照してください。
:::

[Miroを使用したGoogle SSOの](https://support.google.com/a/answer/14100608#zippy=%2Cstep-set-up-google-as-saml-identity-provider)設定については、Googleのヘルプセンターで詳細をお読みください。

## SAMLを使用したMiroのGoogle SSOの設定

Miroを認証するためのGoogle SSOの設定は4つのステップで完了します：

1. SAML ID プロバイダとしての Google の設定
2. SAMLサービスプロバイダーとしてのMiroの設定
3. ユーザー用Miroのオン
4. 認証のテスト

SAML ID プロバイダとしての Google の設定

1. Google Workspace Admin Consoleから、[**アプリ] > [ウェブアプリとモバイルアプリ]**をクリックします。
2. アプリパネルで**アプリの追加**ドロップダウンをクリックし、"アプリの検索 "を選択し、"Miro "と入力します。
3. Miro Web (SAML)」を選択し、「**選択**」をクリックします。
4. Google Identity Provider details」のOption 2で、「SSO URL」、「Entity ID」、「Certificate」がすべて入力されていることを確認し、**「Continue」をクリックします。**これらの値は後でMiroを設定するときにコピーします。
5. サービス・プロバイダーの詳細」に、以下の値を追加します：
   **ACS URL** - https://miro.com/sso/saml
   **エンティティ ID：** https://miro.com
   **開始URL** 空白
   **ログインレスポンス：** チェックなし
   名前 IDメールアドレス
6. **[続行]** をクリックします。
7. Attribute mapping "の "Google Directory attributes "で "**First Name "**を選択し、次に "**Last Name "**を選択します。
8. **完了を**クリックします。MiroアプリがGoogle Workspaceに追加されました。
   ![Google_sso_configuring_google_settings.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515989394_google_sso_configuring_google_settings.gif)*Google SAML ID プロバイダの設定*

SAMLサービスプロバイダーとしてのMiroの設定

1. ブラウザでIncognitoタブを開き、Miroダッシュボード（miro.com/app/dashboard）にログインします。
2. 右上のアバターをクリックし、「**設定**」をクリックします。
3. 会社設定から、**認証をクリックします。**Businessプランをご利用の場合、この設定は「**セキュリティー」になって**います。
4. "Turn on SSO to set up SCIM provisioning "のトグルをクリックします。
5. 会社設定の認証セクションに移動します。**SSO/SAML**トグルをクリックします。組織のSSOを有効にするには、[**オンにする]**をクリックするよう求められます。
6. **SAML サインイン URL については**、Google Workspace Admin Console に戻り、Miro アプリ内で**DOWNLOAD METADATA をクリックします。**このパネルには、必要な値をコピーするオプションがあります。
7. **SSO URL**]で[**コピー]**ボタンをクリックします。Miro に戻り、**SAML ログイン URL**に値を貼り付けます。
8. Googleの証明書を使用し、**キーx.509証明書に対して**このプロセスを繰り返します。
9. **ドメイン**情報を追加します。すでに [ドメインの設定と確認](../../canvas-25-admin-features/domain-control/01-domain-control.md)
10. **保存を**クリック*![google_sso_configuring_miro_authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515990802_google_sso_configuring_miro_authentication.png)**MiroでのSSO認証設定の構成*

ユーザー用Miroのオン

1. Googleワークスペース管理者コンソールに戻る
2. 必要に応じて、アプリメニューから**ウェブとモバイルアプリを** クリックし、**Miroを**選択します。
3. **ユーザーアクセスを**クリックします。
4. **全員ONを**クリックし、**保存を**クリック*![google_sso_turning_on_miro.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528995474_google_sso_turning_on_miro.gif)**Miroアプリを全ユーザーにオン*

特定の組織単位でMiroをオンにしたい場合は、まずOrganizational Unitsでグループをクリックし、**ONをクリックします。**さらに**OVERRIDE** または**INHERITを**クリックする必要があるかもしれません。

認証のテスト

1. Google Workspace Admin Consoleで、必要に応じてMiroアプリを起動します。
2. Miro セクションで、「**TEST SAML LOGIN**」をクリックします。
3. 新しいタブにGoogle SSOのログインオプションが表示されます。
   .GIF
4. Miroで認証をテストするには、新しいIncognitoタブを開き、Miroダッシュボードを起動します(miro.com/app/dashboard)。
5. ログインページが表示されます。**シングルサインオンでログインを**クリックし、アカウント認証情報でログインします。
   ![google_sso_testing_authentication.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528996882_google_sso_testing_authentication.gif)*Miroを使ったGoogle SSO認証のテスト*

あるいは、Miroでテストすることもできます：

1. 上記の手順を完了し、SSO 設定を構成します。
2. [**SSO 設定をテスト**] ボタンをクリックします。
3. 結果を確認してください。
   1. 問題が見つからなければ、「**SSO 設定のテストに成功しました**」という確認メッセージが表示されます。
   2. 問題が見つかった場合、「**SSO 設定のテストに失敗しました**」という確認メッセージが表示され、その後に詳細なエラーメッセージが表示されます。![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)*MiroからのSSO設定のテスト*

> **⚠️** Google Admin Consoleで設定を続ける前に、MiroでSSOを**オフに**することを強くお勧めします。ロックアウトを防ぐには、acmebreaktheglass@gmail.com のように、SSO設定に記載されているドメイン以外のドメインの電子メールを持つ「ガラスを割る」ユーザーを作成します。あるいは、サポートに連絡して組織全体の SSO を無効化することもできます。

Googleによるユーザープロビジョニングを設定したい場合は、「[Googleによる自動プロビジョニングの設定](../../security-integrations/system-for-cross-domain-identity-management-scim/04-setting-up-automated-provisioning-with-google.md)」の記事を参照してください。
