---
title: "\u30B7\u30F3\u30B0\u30EB\u30B5\u30A4\u30F3\u30AA\u30F3\uFF08SSO\uFF09"
article_id: 360017571414
translation_id: 360017571414
locale: ja
sidebar_position: 9
created_at: '2019-02-11T10:08:59Z'
updated_at: '2026-01-07T13:25:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

SAML ベースのシングルサインオン（SSO）により、ユーザーは選択した ID プロバイダー（IdP）を介して Miro にアクセスできます。

> **利用可能なプラン：**Business、Enterprise
> **設定者：** 会社の管理者

## SAML SSO の仕組み

1. Miro のユーザーが SSO を使用して Miro にログインしようとすると、Miro は、SAML（Security Assertion Markup Language）リクエストを ID プロバイダー（IdP）に送信します
2. ID プロバイダーは、ユーザーの認証情報を検証し、Miro に返信して、メンバーの ID を確認します
3. Miro が、応答を認識し、アクセスを許可して、メンバーが Miro アカウントにログインできるようになります

## SSO を有効にした後はどうなりますか？

**初めて SSO を有効にする**

初めて SSO を設定しても、既存のユーザーは中断されることなく Miro で作業を続けることができます。ただし、ログアウトしたときや、セッションの有効期限が切れたとき、または新しいデバイスからログインしようとするときは、SSO でログインする必要があります。

標準のログイン + パスワード、Google、Facebook、Slack、AppleID、O365 などの他のログインオプションは無効になります。

**アイドル セッション タイムアウト**

[アイドルセッション タイムアウト](../../security-integrations/security-management/02-idle-session-timeout.md)を有効にしている場合、ユーザーは自動的に Miro プロフィールからログアウトされ、SSO で認証する必要があります。

**複数のチームと組織**

ユーザーが複数の Miro チームや組織を使用している場合、同じ ID プロバイダー（IdP）を認証に使用するように設定することができます。

**SSO によるログインが必要なユーザー**

SSO でのログインが必要なのは、Enterprise サブスクリプションの一員で、*かつ* SSO 設定にドメインが記載されているユーザーのみです。

- SSO 設定に追加されていないドメインから Miro にアクセスするユーザーは、SSO でログインする必要はありません。代わりに、標準のログイン方法を使用してログインする必要があります。
- Miro Enterprise サブスクリプションに属していない検証済みドメインのユーザーは、[ジャストインタイム（JIT）プロビジョニング](../../user-management/13-user-provisioning-on-enterprise-plan.md)が有効になっている場合にのみ、シングルサインオン（SSO）を介してサインインする必要があります。これらのユーザーは、事前に設定されたチームに自動的に追加され、ログインに SSO を使用する必要があります。
- [管理対象ユーザー](../../user-management/06-managed-users-on-enterprise-plan.md)Enterpriseサブスクリプション外のチームのメンバーでもある管理対象ユーザーを含む、検証済みドメイン内のすべてのユーザーです。特定のチームへのアクセスを制限するには、[ドメイン制御](../../canvas-25-admin-features/domain-control/01-domain-control.md)の設定を更新してください。
  > ✏️ Enterpriseサブスクリプションでは、組織は検証済みドメインと未検証ドメインを持つことができます。認証済みドメインの場合、ユーザーはSSOで認証する必要がある管理ユーザーとなります。同じ組織に所属する未認証のドメインユーザーの場合、認証には電子メールとパスワードが必要です。

**ユーザーの詳細情報を管理する**

ログインに成功すると、ID プロバイダーによって、Miro 内のユーザーデータの紐づけが自動的に行われます。名前やパスワードなどの一部のパラメーターは変更できません。部門やプロフィールの写真などの他のパラメーターは任意です。/span>

- Miro のユーザー名は、ユーザー認証が成功するたびに更新されます。Miro のユーザー名の設定について詳しくは、高度な SSO 設定をご覧ください。ユーザーのメールアドレスを変更する必要がある場合は、[SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) でのみ変更できます。SCIM をご利用でない場合は、[サポートチームまでご連絡](https://help.miro.com/hc/requests/new?referer=help-center-article)ください。

![sso-settings-2.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21027132582290_sso-settings-2.png)
*SSO 設定におけるドメインの選択*

> **💡** ロックアウトを防ぐには、SSO 設定にリストされているドメイン外のドメインを持つメールアドレス（例：acmebreaktheglass@gmail.com）で、「break the glass」ユーザーを作成します。あるいは、サポートに連絡して組織全体の SSO を無効化することもできます。

## SSO の設定

### ID プロバイダー（IdP）

ご希望の ID プロバイダーを使用してください。最もよく使われている ID プロバイダーのプラットフォームには、以下のようなものがあります。

- [OKTA](../../security-integrations/single-sign-on-sso/07-how-to-configure-okta-sso.md)
- マイクロソフトの[Entra ID](../../security-integrations/single-sign-on-sso/05-how-to-configure-entra-id-sso.md)
- [OneLogin](../../security-integrations/single-sign-on-sso/08-how-to-configure-onelogin-sso.md)
- [ADFS](../../security-integrations/single-sign-on-sso/02-how-to-configure-adfs-sso.md)（Microsoft）
- [Auth0](../../security-integrations/single-sign-on-sso/03-how-to-сonfigure-auth0-sso.md)
- [Google SSO](../../security-integrations/single-sign-on-sso/06-how-to-configure-google-sso.md)
- [Jumpcloud SSO](https://support.jumpcloud.com/support/s/article/single-sign-on-sso-with-miro)

### IdP の設定方法

> **💡** [Enterprise 組織で複数の ID プロバイダ](../../security-integrations/single-sign-on-sso/01-adding-multiple-identity-providers.md)（IdP）を追加したい場合は、[プライベートベータ](https://coda.io/form/Miro-Multi-IdP-Private-Beta-Sign-Up_dkoTJMza_jV)に登録してください。

1. ID プロバイダーの設定パネルに移動し、プロバイダーの指示に従って、シングルサインオンを設定します。

2. 以下のメタデータを追加します。オプションのフィールドは飛ばし、デフォルト値はそのままにしておくことをお勧めします。

#### 設定仕様（メタデータ）

|  |  |
| --- | --- |
| **プロトコル** | SAML 2.0 |
| **バインディング** | SP から IdP への HTTP リダイレクト IdP から SP への HTTP ポスト |
| **サービス URL**（SP-initiated URL）  起動 URL、返信 URL、リライングパーティー SSO サービス URL、ターゲット URL、SSO ログイン URL、ID プロバイダー エンドポイントなどとも呼ばれます。 | https://miro.com/sso/saml |
| **Assertion Consumer Service URL**    許可されたコールバック URL、カスタム ACS URL、返信 URL としても知られています | https://miro.com/sso/saml |
| **エンティティー ID**    識別子、証明書利用者信頼識別子としても知られています | https://miro.com/ |
| **デフォルトのリレー状態** | 設定で空のままにする必要があります |
| [**署名要件**](https://developers.onelogin.com/saml/examples/response) | 署名付きアサーションを含む未署名の SAML 応答  署名付きアサーションを含む署名付き SAML 応答 |
| **SubjectConfirmation Method** | "urn:oasis:names:tc:SAML:2.0:cm:bearer" |
| ID プロバイダーの SAML 応答には、ID プロバイダーが発行した公開鍵の x509 証明書が含まれている必要があります。  SAML の詳細な例をご覧ください。[Miro SP メタデータファイル](https://drive.google.com/file/d/1BN58fiwC062F5MC-PsO3QN7JlCbKNCSJ/view)（XML）をダウンロードします。 | |

:::warning
暗号化やシングルログアウトには対応してません。
:::

#### ユーザーの資格情報

以下のフィールドは必須ではありません。オプションのフィールドは飛ばし、デフォルト値はそのままにしておくことをお勧めします。

|  |  |
| --- | --- |
| 必要なユーザーの資格情報の属性 | |
| **NameID**（ユーザーのメールアドレスと同じ）  SAML_Subject、主キー、ログオン名、アプリケーション ユーザー名形式などとしても知られています。 | &lt;NameID Format="urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress"&gt; |
| **アサーション付きで送信するオプションの属性**  （SSO 経由で新しい認証ごとに更新され、存在する場合に使用されます） | - "DisplayName" または "http://schemas.microsoft.com/identity/claims/displayname"（優先名として使用）  [mceclip0.png](http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname)  - “FirstName”, "GivenName" または "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname" - “LastName”, "Surname" または "http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname" - "ProfilePicture" ー エンコードされた画像の URL |

### Miro の設定で SSO を有効にする方法

Business プラン Enterprise プラン

1. **[会社]** の設定 > **[セキュリティー]** > **[シングルサインオン]** に移動します
2. SSO/SAML のトグルをオンにします

*![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20889990489874_security-sso.png)
*security-sso.png**

1. **[会社]** の設定 > **[セキュリティーとコンプライアンス]** > **[認証]** > **[シングルサインオン]** に移動します
2. SSO/SAML のトグルをオンにします

*![](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366644626_sso-enterprise.png)
*sso-enterprise.png**

:::note
設定で SSO を有効化しても、すぐにユーザーの SSO が有効になるわけではありません。SSOログインは、[ドメインが認証された](../../canvas-25-admin-features/domain-control/01-domain-control.md)後に利用可能になります。その後、次のセクションでSSOを設定する際に、検証済みのドメインを追加してください。
:::

### Miro の設定で SSO を設定する方法

シングルサインオン設定で SSO/SAML 機能をオンにした後、以下のフィールドに入力します。

1. **SAML ログイン URL**（多くの場合、エンドユーザーが資格情報を入力する ID プロバイダーのページが開きます）
2. **公開鍵の x.509 証明書**（ID プロバイダーが発行したもの）
3. SAML サーバー経由で認証できる、または認証する必要があるすべてのドメインおよびサブドメイン（ACME.com または ACME.dev.com）
4. 検証済みのドメインを追加します。**これらのドメインのユーザーはSSOを使用してログインします**]をクリックします。 ***ドメインを選択***をクリックし、リストに追加するドメインを選択します。

![sso-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366648082_sso-settings.png)
*Miro の SSO 設定*

### SSO / SAML 証明書の更新

公開鍵の x.509 証明書の有効期限が切れている場合でも、SSO は引き続き機能しますが、Miro を安全に使い続けるためには、更新することを強くお勧めします。公開鍵の x.509 証明書は、ID プロバイダーと Miro の間で共有される情報のセキュリティー、プライバシー、信頼性、完全性を保証します。

こうした証明書は、ID プロバイダーで指定（および確認）できる期間のみ有効です。有効期限を確認するには、ID プロバイダーにご確認ください。

このプロセスには 2 つの手順があります。

1. ID プロバイダーで証明書を更新します。これを行う方法については、プロバイダーの指示をご確認ください。
2. 更新された証明書を Miro SSO 設定に追加します。

#### 更新された証明書を Miro に追加

:::warning
ログイン時の混乱を避けるため、x.509 証明書の交換は、組織内であまり忙しくない期間（週末や営業時間後など）に行うことをお勧めします。
:::

1. **[会社の設定]** > **[認証]** > **[シングルサインオン]** に移動します
2. **鍵の x.509 証明書**フィールド内のコンテンツを削除します
3. このフィールドに新しいキーを貼り付けます
4. スクロールダウンして、**[保存]** をクリックします。
   ![sso-gif-2.gif](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21027132584850_sso-gif-2.gif)
*Miro で x.509証明書を更新*

## SSO 設定のテスト

SSO の設定を有効にする前にテストして、ログインで発生する可能性のある問題を確認できます。

1. 上記の手順を完了し、SSO 設定を構成します。
2. [**SSO 設定をテスト**] ボタンをクリックします。
3. 結果を確認してください。

- 問題が見つからなければ、「**SSO 設定のテストに成功しました**」という確認メッセージが表示されます。
- 問題が見つかった場合、「**SSO 設定のテストに失敗しました**」という確認メッセージが表示され、その後に詳細なエラーメッセージが表示されます。

![sso-test.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/20937366649618_sso-test.png)
*SSO 設定のテスト*

## オプションの高度な SSO 設定

オプション設定は SSO 設定に精通している上級ユーザー向けのセクションです。

### 新規ユーザー向けのジャストインタイム プロビジョニング

エンドユーザーが、招待を待ち、全オンボーディング プロセスに参加しなくても、Miro にすぐ参加できるようにします。また、管理するサブスクリプション以外の無料チームの作成を防ぐこともできます（ドメイン管理が必要です）。新規ユーザーのジャストインタイム（JIT）プロビジョニングを有効にするには、SSO が必要です。JIT でプロビジョニングされたすべてのユーザーには、以下のサブスクリプションのデフォルトライセンスが割り当てられます。

|  |  |  |
| --- | --- | --- |
| **サブスクリプション タイプ** | **ライセンスタイプ** | **ライセンスがすべて使われている場合の動作** |
| Business プラン | フルライセンス | ユーザーは自動的に追加されず、JIT 機能は動作しなくなります。 |
| Enterprise プラン（[フレキシブル ライセンス プログラム](../../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)がない場合） | フルライセンス | [制限付き無料](../../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)ライセンスでプロビジョニングされたユーザー |
| Enterprise プラン（フレキシブル ライセンス プログラムが有効な場合） | 無料または制限付き無料ライセンス | [デフォルトのライセンス](../../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md)設定によって異なります |

### ジャストインタイム プロビジョニングを有効にする方法

ジャストインタイム プロビジョニングを有効にすると、Miro に登録しているすべての新規ユーザーに自動的に適用されます。ただし、既存の Miro ユーザーがプランに参加するには招待が必要です。

1. [SSO 設定] に移動します
2. **リストにあるドメインの新規登録ユーザーを全員 Enterprise アカウントに自動的に追加する**にチェックを入れます。
3. ドロップダウンから、**新規登録ユーザーのデフォルトチームを選択**します
4. **[保存]** をクリックします

シングルサインオン（SSO）設定に特定のドメインをリストすると、そのドメインに登録したユーザーは、自動的に Enterprise サブスクリプションに追加されます。ジャストインタイム（JIT）設定で選択したチームに割り当てられます。

![Copy of user_provisioning_jit_provisioning.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528391698_Copy%20of%20user_provisioning_jit_provisioning.png)*Enterprise インテグレーションページでJust in Time プロビジョニング機能を有効化*

設定で記載したドメインの**新規登録ユーザー**はすべて、Miro 登録時に、ご利用の Enterprise 傘下でこの特定のチームに自動的に追加されます。

:::warning
Enterprise プランでは、チームの公開設定を有効にすると、このチームは公開されたチームのリストにも表示されます。
:::

### デフォルトのユーザー名として DisplayName を設定

デフォルトで Miro は **FirstName** + **LastName** の属性を使用します。あるいは、**DisplayName** の使用をリクエストすることもできます。この場合、ユーザーの SAML 応答に **DisplayName** *があると*、Miro はこれを使用します。

**DisplayName** がなくても、**FirstName** + **LastName** がある場合、Miro は **FirstName + LastName** を使用します。**DisplayName** を希望の SSO ユーザー名にするには、Miro サポートにご連絡ください。

SAML 通信にこの 3 つの属性がいずれも存在しない場合、Miro は、ユーザーのメールアドレスをユーザー名として表示します。

|  |  |
| --- | --- |
| **設定** | **デフォルトのユーザー名** |
| Miro のユーザー名 | FirstName + LastName |
| 代替設定 | DisplayName（ユーザーの SAML リクエストに存在する場合） |
| フォールバック | FirstName + LastName（DisplayName が存在しない場合） |
| 希望の SSO ユーザー名 | DisplayName（[Miro サポートにお問い合わせください](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)） |
| 属性が存在しません | ユーザー名として表示されるメールアドレス |

予期したものと異なるものが表示された場合は、SSO で認証する必要があるかもしれません。あるいは、SAML 応答に更新に必要な値が含まれていない可能性があります。

### IdP からユーザープロフィール写真を同期

:::warning
SCIM を有効化していない場合、または IdP が**ProfilePicture** 属性をサポートしていない場合（例えば、ProfilePicture ではサポートされていない場合など）にこのオプションを有効にすることをお勧めします。その他の場合は、SCIM 経由で ProfilePicture を転送し、すぐに更新することをお勧めします。
:::

この設定がオンになっている場合：

- IdP 側で設定したプロフィール写真は、ユーザーの Miro のプロフィール写真として設定されます。
- ユーザーは、自分でプロフィール写真を更新または削除することはできません。

ユーザー名と同じように、Miro でデータを変更するオプションは即時になくなりますが、データの*同期*は即時には行われません。ユーザーの*次*の SSO 認証の際に、IdP 側は更新情報を Miro に送信します（ただし、その時点で「IdP からユーザープロフィール写真を同期する」の設定がまだ有効である場合に限ります）。

IdP でプロフィール写真が設定され、SAML 通信でその属性を移したい場合、Miro は以下のスキーマを求めます。

```
<saml2:Attribute Name="ProfilePicture" NameFormat="urn:oasis:names:tc:SAML:2.0:attrname-format:uri">
<saml2:AttributeValue
xmlns:xs="http://www.w3.org/2001/XMLSchema"
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">https://images.app.goo.gl/cfdeBqKfDKsap1icxecsaHF
</saml2:AttributeValue>
</saml2:Attribute>
```

## SSOとデータレジデンシー

Miroの[データレジデンシーサポートを](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md)使用し、専用のURL（workspacedomain.miro.com）を持っている場合は、IDプロバイダの設定を調整する必要があります。

:::note
オーストラリアと米国にデータレジデンシーを持つ組織の場合、ソーシャルログインはご利用いただけません。データレジデンシーの詳細については、[Miroのデータレジデンシーを](../../canvas-25-admin-features/data-residency/02-data-residency-at-miro.md)ご覧ください。
:::

これを行うには、[ORGANIZATION_ID] を URL に追加する必要があります。

ORGANIZATION_ID は、Miro のダッシュボードから、右上の **[プロフィール]** > **[設定]** をクリックすると、アドレスバーの URL に表示されています。

|  | 基準値 | データレジデンシーによる値 |
| --- | --- | --- |
| **アサーション コンシューマー サービス URL**（別名：許可されたコールバック URL、カスタム ACS URL、返信 URL）： | https://miro.com/sso/saml | https://workspace-domain.miro.com/ sso/saml/ORGANIZATION_ID |
| **エンティティー ID**（識別子、証明書利用者信頼識別子）：https://miro.com/ | https://miro.com/ | https://workspace-domain.miro.com/ 組織 ID |

## SSO 外のユーザーに対する多要素認証（2FA）の設定

2 要素認証（2FA）は、セキュリティレイヤーを追加します。2FA では、ユーザーがログイン中に追加のステップを完了して、識別情報を検証することが求められます。この追加措置により、許可された個人のみがご利用のサブスクリプションにアクセスできるようになります。
詳しくは[二要素認証管理者ガイド](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)をご覧ください。

## よくある質問と考えられる問題の解決法

「DomainName is busy」というメッセージが表示され、SSO 設定で、ドメインアドレスが承認されません。

セキュリティー上の理由から、対応できるのは、組織のドメインにつき*会社（Enterprise サブスクリプション） 1 つのみです*。Business プランまたは [Enterprise プラン](../../../plans-billing/miro-plans/04-enterprise-plan.md)の別のアカウントで、ドメインがすでに設定されているため、希望するドメインで SSO を有効にできない可能性があります。あらかじめ同僚の方に確認してみてください。

利用可能なドメインのドロップダウンに利用中のドメインが表示されません。

まず、[マネージドドメイン設定](../../canvas-25-admin-features/domain-control/01-domain-control.md)でドメインを登録し、検証する必要があります。

エンドユーザーのメールアドレスを変更しなければなりません / ユーザーのメールアドレスを変更したため、ユーザーがボードにアクセスできなくなりました。

会社がドメイン名を変更し、エンドユーザーのメールアドレスの SSO 認証情報の変更が必要な場合は、[サポートチームにご連絡](https://help.miro.com/hc/requests/new?referer=help-center-article)ください。

SSO の手順に、個別のゲートウェイ（例えば、Duo DAG などの MFA）を使用したいと考えています。

もちろんご利用いただけます。SAML 2.0 で動作する限り、Miro はご希望のソリューションに対応します。

SSO を有効にしましたが、Miro のユーザープロフィール データ（IdP でサポートされている場合は、名前、プロフィール写真）が、IdP のデータと同期されません。

SAMLResponse に空でない新しい値が含まれている場合、ユーザー認証がすべて成功した後、Miro のユーザー名やプロフィール写真は更新されます。Miro のユーザー名の設定について詳しくは、 高度な SSO 設定をご覧ください。

SSOプロバイダーを変更するには、どのような手続きが必要ですか？

SSOプロバイダを変更する場合は、初回セットアップ時と同様に、新しいIDPを一から設定する必要があります。

Miro にログインしようとしたときに、ユーザーの一人または全員にエラーが発生した場合は、よくあるエラーリストと解決方法をご確認ください。
