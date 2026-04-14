---
title: ADFS SSO の設定方法
article_id: 360022411353
translation_id: 360022411353
locale: ja
sidebar_position: 2
created_at: '2019-04-29T20:13:47Z'
updated_at: '2025-11-25T16:04:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '利用可能なプラン：: [エンタープライズ](../../../plans-billing/miro-plans/04-enterprise-plan.md),[ビジネス](../../../plans-billing/miro-plans/06-business-plan.md)プラン
    設定者：: 会社の管理者'
---

Miro は、SAML 2.0 によるシングルサインオン（SSO）ログインに対応しています。

SAML 2.0 ID プロバイダー（IDP）は多くの形式を取ることができますが、そのうちの 1 つに、セルフホストされた Active Directory フェデレーション サービス（ADFS）サーバーがあります。ADFS は、Microsoft が Windows Server の標準的な機能として提供しているサービスで、既存の Active Directory の資格情報を使用した Web ログインを提供します。

このガイドでは、**Server 2012R2** のスクリーンショットを使用していますが、他のバージョンでもこの手順は利用することができます。

まず、サーバーに ADFS をインストールします。ADFS の設定とインストールは、このガイドの説明範囲外ですが、Microsoft の[こちらの記事](http://msdn.microsoft.com/library/gg188612.aspx)で詳しく説明しています。

テストをする際は、作業ステーションとテストの認証で使用するメールアドレスが同じであることを確認してください。同じでなければ、ADFS の設定とプロフィールが正しくてもログインすることができません。

> *お使いのブラウザーのシークレットモードのウィンドウを新たに開けて、SSO を設定することを強くお勧めします。*そうすることで、セッションを標準ウィンドウに保ち、誤った設定があった場合に、SSO 認証をオフにすることができます。

実際に SSO を有効にする前にテストインスタンスを設定したい場合は、アカウント担当者または営業担当者にご連絡ください。SSO 設定者のみがこのテストインスタンスに追加されます。

> **⚠️ ルール、サポートされている機能、Miro 側でのオプション設定については、SSO に関する主要記事を**[**こちら**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)**でご覧ください。**

## ステップ 1 ー 証明書利用者信頼の追加

1) ADFS サーバーにログインし、**ADFS 管理コンソール**を起動します。

2) **AD FS 管理コンソール**から **証明書利用者信頼**のフォルダーを選択し、**アクション** サイドバーから新しい **標準証明書利用者信頼** を追加します。上記の設定が完了すると、新しい信頼証明書設定ウィザードが開始されます。

add_a_party_trust.jpg
利用者信頼を追加

3) **データソースの選択**画面の一番下にある **[Enter Data About the Party Manually]（利用者のデータを手動で入力する）**にチェックを入れます。

step_3.jpg
**Enter Data About the Party Manually（利用者のデータを手動で入力する）を選択する**

4) 後からでも分かるように、**表示名**とメモを入力しておきます。

display_name.jpg
Display name（表示名）を追加

5) **[ADFS FS (ADFS 2.0) profile]（ADFS FS（ADFS 2.0）プロフィール）**ボタンを選択します。

step_5.jpg

next.jpg
請求の暗号化と復号化に必要な証明書を参照するよう求められます。この設定はオプションなので、**[次へ]** を押してスキップすることも可能です。

6)**[Enable Support for SAML 2.0 WebSSO protocol (SAML 2.0 WebSSO プロトコルのサポートを有効にする**)] というラベルの付いたボックスをオンにします。
サービスURLはhttps://miro.com/sso/saml。

URL の末尾にはスラッシュがないことに**ご注意**ください。

step_6.jpg
SAML 2.0 WebSSO プロトコルサポートの有効化

7) **証明書利用者信頼識別子**に `https://miro.com/` を追加します。

step_7.jpg
**証明書利用者信頼識別子の追加**

*次の画面では、多要素認証を設定することができますが、これはこのガイドの説明範囲外です。*

rejecting_on_step_7.jpg
*多要素認証の設定を拒否するオプション*

8) **[Permit all users to access this relying party]（すべてのユーザーにこの証明書利用者へのアクセスを許可する）**ボタンを選択します。

step_8.jpg
すべてのユーザーに証明書利用者へのアクセスを許可するオプション

次に表示される 2 つの画面のウィザードには、設定の概要が表示されます。

最後に表示される画面で、**[閉じる]** ボタンをクリックして、コンソールを終了し、**[Claim Rules]（要求規則）**エディターを開きます。

final_step.jpg
証明書利用者信頼の追加の終了

また、設定に**署名済みのアサーション**が含まれていることを確認してください。

## ステップ 2 ー 要求規則の作成

依拠当事者信託が作成されたら、請求ルールを作成することができます。
デフォルトでは、トラストを作成するとクレーム・ルール・エディターが開きます。

1) 新しい規則を作成するには、**[Add Rule]（規則を追加）**をクリックします。

adding_a_rule.jpg
新しい規則の追加

2) テンプレートに **[LDAP 属性を要求として送信する]（]end LDAP Attributes as Claims）**を選択して、新しい規則を作成します。

claim_rule_template.jpg
新しい規則の作成

3) 次の画面で規則に名前をつけて、**Active Directory** を属性ストアとして、以下のようにマッピングします。

| LDAP 属性 | 送信要求タイプ |
| --- | --- |
| E-Mail-Addresses（メールアドレス） | E-Mail Address（メールアドレス） |
| Given-Name（名） | FirstName（姓） |
| Surname（姓） | LastName（名） |

map_LDAP_attributes.jpg
LDAP 属性のマッピング

**[OK]** をクリックして、新しい規則を保存します。

4) **[ルールを追加]** をクリックして別の新しいルールを作成します。ここではテンプレートに **[Transform an Incoming Claim]（受信した規則を変換する）**を選択します。

add_another_rule.jpg
**テンプレートにTransform an Incoming Claim（受信した規則を変換する）を選択**

5) 次に、規則に名前をつけて、以下のパラメータを設定します。

|  |  |
| --- | --- |
| **受信要求タイプ** | E-mail Address（メールアドレス） |
| **送信要求タイプ** | 名前 ID |
| **送信名 ID フォーマット** | メールアドレス |

set_rule_parameters.jpg
規則のパラメータ設定

最後に、**[OK]** をクリックして要求規則を作成し、その後、再度 **[OK]** をクリックして規則の作成を終了します。

これでADFSの設定は完了です。以降は、[Miro プランの SSO 機能を有効にする](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)だけで、エンドユーザによる SAML を使用した Miro の認証が可能になります。

## MiroでのSSO設定のテスト

1. 上記の手順を完了し、SSO 設定を構成します。
2. [**SSO 設定をテスト**] ボタンをクリックします。
3. 結果を確認してください。

1. 問題が見つからなければ、「**SSO 設定のテストに成功しました**」という確認メッセージが表示されます。
2. 問題が見つかった場合、「**SSO 設定のテストに失敗しました**」という確認メッセージが表示され、その後に詳細なエラーメッセージが表示されます。

![test-sso.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/19662118715282_test-sso.png)

*MiroでのSSO設定のテスト*
