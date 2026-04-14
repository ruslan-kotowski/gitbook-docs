---
title: "SSO \u7D4C\u7531\u3067\u30ED\u30B0\u30A4\u30F3\u3067\u304D\u306A\u3044"
article_id: 360019271654
translation_id: 360019271654
locale: ja
sidebar_position: 10
created_at: '2019-03-07T15:50:03Z'
updated_at: '2025-11-25T16:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

シングルサインオン（SSO）に関連した問題について、ユーザーと IT 管理者に向けたトラブルシューティングのアドバイスをご覧ください。

> **️✏️** [️Miro SSO](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) と [Miro SCIM](https://developers.miro.com/docs/scim) の設定の詳細をご覧ください。

## Miro の SSO エラー

これらの SSO エラーメッセージが表示された場合、以下の解決策を検討してください。IT 部門または会社の管理者の助けが必要な場合があります。

メールアドレスが SSO アカウントと関連付けられていません

Miro に入力したメールアドレスが、SSO で認証されるべきユーザーとして認識されない場合に発生します。

考えられる原因：

- **SSO をログイン要件として設定したサブスクリプションのメンバーでない**。標準的なオプション（メールアドレスとパスワード）でログインするか、管理者と連絡を取って、会社のサブスクリプションに招待してもらいます。
- **SSO でログインするはずが、メールアドレスに関して混乱が起きている**。複数のメールアドレス（またはエイリアス）を持っているため、SSO で設定されたプランへの招待が他のアドレスに送信されたのかもしれません。別のメールアドレスでログインしてください。

メールアドレスが SSO アカウントと関連付けられていません。会社の管理者にアクセスをリクエストしてください

これは通常、2 つのシナリオで起こります：

- **ID プロバイダーシステムのユーザープロフィールに、Miro にログインする権限が与えられていない（役割が割り当てられていない）場合**。この場合おそらく、プロバイダーの MyApps ダッシュボード上で Miro をタイルとして見つけることができないでしょう。プロバイダーの管理者に連絡して、必要なアクセス権を取得してください。
- **最近、メールアドレスを変更**（例えば、結婚のために）した結果、変更がすべてのシステムで正しく適用されておらず、競合が生じている場合。管理者に連絡して状況を明確にしてください。管理者は必要であれば Miro に連絡して、必要な変更を承認します。

SSO で Miro にログインできない場合、[Miro の SSO ログインページ](https://miro.com/sso/login/)で該当するボタンをクリックして、会社の管理者にアクセスをリクエストできます。

![sso-new-sign-in.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/20463017477778_sso-new-sign-in.png)*会社の管理者にアクセスを要求するオプション*

メールアドレス宛てに送信される確認コードを入力する必要があります。コードを入力すると、会社のサブスクリプションの管理者に通知が送信され、サポートが必要であることを知らせます。

接続エラーが発生しました：応答に対する署名の検証に失敗しました

これは、ユーザー側の Miro の SSO 設定、または ID プロバイダー側の設定が間違っているということです。他の同僚もログインできていない可能性があります。IT 部門または ID プロバイダーの管理者に連絡して、以下の点を確認してください。

- SAML の応答は、署名された*アサーション*を含んでいることが必要です。これは、Miro の要件です。
- ID プロバイダーは、特定の方法で署名された応答を扱っている可能性があります。例えば、Google SSO がアサーションを*解除*するのは、応答が*署名された*時です。これに該当する場合、応答の署名を解除してください。
- SAML の応答に必要な署名されたアサーションが含まれていても、本来検証に使われる X.509 の証明書の値が存在しないことがあります（VPN / ファイアウォールが[データ転送の一部を切り離した場合](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)にも起こり得ます）。X.509 の証明書の値が、Miro に SAML トラフィックで渡されたことを確認してください。
- SAML の応答に*[Miro の設定](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)*で追加された X.509 の証明書の値とは違う値が含まれているため、ミスマッチが発生し検証に失敗することがあります。IDP 側と Miro 側で、証明書の値が一致していることを確認してください。

接続エラーが発生しました：SAML レスポンスでユーザーの情報が提供されませんでした。

これは、ID プロバイダー側で、一般的な設定または特定のユーザープロフィールについての設定が誤っているということです。IT 部門または ID プロバイダーの管理者に連絡して、以下の点を確認してください。

- SSO 設定のユーザー名（NameID、一意のユーザー ID）の形式が、未指定またはメール以外の属性に設定されているため、Miro に送信されたユーザーの値が認識できない。ID プロバイダー側の **EmailAddress**（またはメール形式の他の属性）にユーザー名を指定します。
- SAML の応答にユーザーのメールの値が含まれていないため、ユーザーを認識できない（VPN / ファイアウォールが[データ転送の一部を切り離した](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)場合にも起こり得ます）。メールが Miro に SAML トラフィックで渡されたことを確認してください。
- SAML の応答が暗号化されている。Miro がサポートしていないため、暗号化を使用しないでください。

接続エラーが発生しました：SAML レスポンスが正しくありません

これは通常、ID プロバイダー側でプロフィールに問題が発生した場合に起こります。
考えられる原因：

- **ID プロバイダーシステムのユーザープロフィールが正しく設定されていない**。例えば、Miro にログインする権限が与えられていない（役割が割り当てられていない）場合。この場合おそらく、プロバイダーの MyApps ダッシュボード上で Miro をタイルとして見つけることができないでしょう。プロバイダーの管理者に連絡して、必要なアクセス権を取得してください。
- **ID プロバイダーシステムのユーザープロフィールは正しく設定されていても、制限が設けられている**。例えば、IP の制限があると特定の場所からしかログインできません。ID プロバイダーの管理者に連絡し、アクセス権についてお問合せください。

SSO で認証するには、会社側が提供した URL リンクを使用してください

つまり、このページから Miro にアクセスすることが本来できないか、Miro Enterprise プランの SSO 設定が完了していないということです。この場合、MyApps ダッシュボードからログインできる可能性があります。
考えられる原因：

- IDP が **IdP 起動のログイン**[のみに設定されていて](https://blogs.oracle.com/dcarru/sp-vs-idp-initiated-sso)、**Miro のログインページからログインできない。**提供されたリンクを使って MyApps ダッシュボードからログインするか、会社の管理者に連絡して、手順を確認してください。
- **SSO は Miro Enterprise プランで有効になっていても、設定が完了していない**。IT 部門または ID プロバイダーの管理者に連絡を取り、[これらの手順](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)に従って設定を完了してもらいます。

## Entra または ADFS エラー

シングルサインオン設定は、Enterprise アプリケーション エクスペリエンスのこのアプリケーションでは利用できません

メッセージの全文：*シングルサインオン設定は、Enterprise アプリケーション エクスペリエンスのこのアプリケーションでは利用できませんMiro（旧 RealtimeBoard）はマルチテナントのアプリケーションで、アプリケーションは別のテナントが所有しています。**返信 URL や識別子などのプロパティーを変更するには、アプリケーションの所有者に連絡してください。*IT 部門と連絡を取り、SSO 設定を確認してもらうよう依頼してください。ほとんどの場合、Azure AD にすでに設定された Miro アプリがあり、そこで Miro の識別子（[https://miro.com/](https://miro.com/))）が使用され、従って取得されています。Entra は、この ID プロバイダーが一意の識別子（Entity ID）を要求するという点で、一意であるといえます。
この状況を解決するには、Entra インスタンスの Enterprise アプリケーションを確認し、Miro の設定に既に構成されているものを使用することをお勧めします。
Enterprise アプリに他の Miro アプリがないことを確認している場合は、Entra ギャラリーから Miro アプリの新しいコピーを取得してみてください。

エラーが発生しました。詳細については、管理者に連絡してください

このコミュニティーの投稿を IT 部門と共有いただけます：[「エラーが発生しました。詳細は管理者にお問い合わせください。](https://blog.kloud.com.au/2015/07/22/adfs-sign-in-error-an-error-occurred-contact-your-administrator-for-more-information/)

アクセス権が付与されていません：エラー AADSTS50105

![mceclip3.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044185746_mceclip3.png)
このコミュニティーの記事を IT 部門と共有いただけます：[「役割が割り当てられていません」のエラー](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50105-user-not-assigned-role)

アプリケーションの構成ミス：エラー AADSTS650056

![mceclip2.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016044184722_mceclip2.png)
マイクロソフトの [AADSTS650056エラーに関するドキュメント](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)（および[コミュニティーからの提案](https://blogs.aaddevsup.xyz/2019/11/aadsts650056-misconfigured-application/)）を確認したところ、このエラーはアプリのアクセス許可に追加した変更が原因である可能性があるようです。エンドユーザーが Miro で認証できるよう、Entra 管理者による Miro アプリへの同意が必要である場合があります。この場合、[Microsoft のチュートリアル](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow)をご参照ください。

[他に起こり得る SSO エラーについては、support.microsoft.com の記事](https://support.office.com/article/how-to-troubleshoot-issues-that-you-encounter-when-you-sign-in-to-office-apps-for-mac-ipad-iphone-or-ipod-touch-when-using-active-directory-federation-services-e44357b4-c9c4-4580-a946-ef5dabdb98cd?ui=en-US&rs=en-US&ad=US)をご覧ください。

## Google SAML エラー

[Google ドキュメントのこのセクション](https://support.google.com/a/answer/6301076?hl=en)を参照してください。考えられるエラーと状況を解決するための手順がリストアップされています。

## デスクトップアプリ、タブレット、またはモバイル上で、SSO 経由で Miro アプリにログインする問題

デスクトップ / タブレット / モバイルデバイスでは、SSO 経由で Miro アプリにログインできないが、[ブラウザーバージョン](https://miro.com/app/)にはログインできる場合、以下を行います。

1. デバイスからアプリを削除し、再インストールします。デスクトップアプリの場合、すべてのアプリフォルダーを削除するために、[こちらの手順](../../../getting-started/apps-for-devices/05-desktop-app.md)を行います。この問題の最も一般的な原因は不良キャッシュなので、すべてを完全に削除して新しくインストールし直すと解決するはずです。
2. 試しにデバイスでデフォルトで使っているブラウザーを変え、別のブラウザーでプロセスを完了できるかどうかを確認してみてください。お使いのブラウザーが[サードパーティーのクッキー](https://akohubteam.medium.com/how-to-enable-third-party-cookies-on-your-browsers-f9a8143b8cc5)を許可していることを確認してください。
3. ID プロバイダーが*リレーステート* パラメーターを管理**していない**か確認します。これは、Miro が生成し、ユーザーがブラウザーのページにとどまるのではなく、アプリに戻されることになっていることを認識するために使用する独自のトークンです。**RelayState** を管理する IdP 設定のフィールドが*空*になっていることを確認してください（フィールド名は、Okta では **Default RelayState**、Google SSO では **Start URL** など、異なる場合があります）。
4. 問題が解決しない場合は、この特定のデバイスが会社の SSO 環境にアクセスできない可能性があります。SSO の使用が許可されている特定のデバイスに関する制限があるかどうか、IT 部門に確認してください。例えば、MDM ソリューションでは、Miro が適切に[許可リスト](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md)に追加されていない場合に問題が発生する可能性があります。
5. 特に Miro デスクトップアプリについては、当社のアプリのスキーマが正常に動作し、壊れていないことを確認してください。そのためには、ご利用ブラウザーのアドレス行に **miroapp://** と入力し、クリックして*ウェブサイト*として開きます（単にエンターキーを押すと、検索が開始されますのでご注意ください）。
   ![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)
   この時、Miro アプリを開くように促すポップアップが表示されるはずです。そうならない場合は、スキーマが壊れている可能性があります。スキーマが正しくインストールされているかどうかを確認するには、Windows または Mac の指示に従います（これは Miro アプリの MS Store バージョンには適用されません）。

   Windows の場合Mac の場合

   1. [レジストリー エディターアプリ](https://support.microsoft.com/windows/how-to-open-registry-editor-in-windows-10-deab38e6-91d6-e0aa-4b7c-8878d9e07b11)に移動します。
   2. Ctrl + F キーを押し、**miroapp** を見つけます。レジストリは次のようになっているはずです： *![registry_editor_map.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21016057554322_registry%20editor%20map.png)*

   1. ターミナルアプリで、以下のコマンドを実行します。

      **sudo /System/Library/Frameworks/CoreServices.framework/Versions/A/Frameworks/LaunchServices.framework/Versions/A/Support/lsregister -dump URLSchemeBinding | grep miroapp**

      結果は、次のようになります。

      ![](/attachments/token/I53o1MUemZ9TqkRlz9dQ7ndsr/?name=image.png)

状況が異なる場合（スキーマレコードがレジストリーに表示されない、または別のパスで表示されるなど）は、[Miro のウェブサイトから](https://miro.com/apps/)アプリを再インストールしてみてください。

それでも解決しない場合は、IT チームに問い合わせて、状況、特に以下の点について確認するよう依頼してください。

- カスタム URI プロトコルが許可されているか。これがブロックされている場合、アプリのインストールプロセス中にスキーマがインストールされない可能性があります。
- レジストリーが、標準的なインストールを妨げるまたは変更する可能性があるその他の制限やポリシーの対象になっているか。

## メールアドレスを変更したら、SSO でプロフィールにログインできません

組織が SSO を使用している場合、Miro 側と ID プロバイダー側でメールアドレスの変更を行った後で、エンドユーザーが新しい認証情報を使用して Miro にログインすることが必要です。次のログイン前に変更が行われていない場合、メールアドレスは新しいユーザーとして認識され、Miro にログインする際に問題が発生する可能性があります。

管理者に連絡して、状況を把握することをおすすめします。ユーザーと管理者は、[Miro サポート](../../tools/troubleshooting/06-contacting-miro-support.md)に連絡して新しい空のプロフィールを削除し、既存のプロフィールのメールアドレスを変更することが必要な場合があります。その場合、以下の情報を提供してください：

- 新しいメールアドレスと古いメールアドレス
- 会社の Miro の管理者を CC に入れ、Miro による変更を承認する確認メールを送信してほしい旨を依頼します（セキュリティー上の理由で必要です）

> ️️✏️ 上記で解決しない問題があれば、[Miro サポートにご連絡ください](https://miro.com/contact/recover/)。
