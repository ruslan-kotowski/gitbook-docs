---
title: 複数 ID プロバイダーの追加
article_id: 16287287497234
translation_id: 16287287497234
locale: ja
sidebar_position: 1
created_at: '2024-01-10T10:51:24Z'
updated_at: '2026-02-18T08:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '利用可能対象: Enterprise 設定者: 会社の管理者'
---

:::note
複数の ID プロバイダーの追加は、Enterprise のお客様にのみ提供される専用機能です。この機能にアクセスし有効化するには、Miro のアカウント チーム マネージャーまたはお客様担当者にご連絡ください。Miro サポートではこの機能を有効にできません。
:::

シングルサインオン（SSO）で複数の ID プロバイダー（IdP）を使用できます。これは、複数の支店や子会社を持つ大きな組織で、それぞれ独自の IdP を持ちつつも、同じ Miro サブスクリプションを利用する場合に特に便利です。

## 複数の ID プロバイダーを追加する準備

複数の IdP アプリケーションを追加した後も[シングルサインオン（SSO）](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)を確実に動作させるためには、既存の IdP アプリケーションの構成を更新する必要があります。

Entra ID などの IdP は、組織が複数のアイデンティティプロバイダー (multi-IdP) のプライベート機能を有効にするまで、新しい構成形式をサポートしません。ログインの中断を避けるために、お客様担当者とコールを設定し、一緒にこのプライベート機能を有効にするための手順を案内してもらうことをお勧めします。

### Enterprise 設定の構成方法

1. SCIM をオフにする。
2. SSO の設定を更新する。
3. SSO 機能を確認する。

#### SCIM を無効にする

現在、複数の IdP との[SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)はサポートしていません。Enterprise プランの SCIM を無効にするには、**企業** 設定 > **アカウント** > **Enterprise インテグレーション** に進み、**SCIM プロビジョニング**をオフにしてください。

#### SSO 設定の更新

**旧設定**

Miro SSO が IdP に最初に設定されたとき、以下の設定値が使用されたと考えられます。

- **コールバック URL/ACS：** https://miro.com/sso/saml
- **エンティティ ID：** https://miro.com

**新しい構成**

IdP が Miro 内のどの構成に関連するかを認識するために、以下の値を更新する必要があります。**設定** > **セキュリティ** > **認証** に進んでください。

これらの値は、組織がマルチIdPプライベート機能を有効にすると、SSO設定で利用可能になり、以下の形式になります。

- **コールバック URL/ACS:** https://miro.com/sso/saml/&lt;org_id&gt;/&lt;saml_settings_id&gt;
- **エンティティ ID:** https://miro.com/&lt;org_id&gt;/&lt;saml_settings_id&gt;

![Callback URL and Entity ID in the Enterprise admin console](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/23763575205778_image.png)

*管理者コンソール内のコールバックURLとエンティティID*

#### SSO 機能を検証します

IdP 設定の更新が完了したら、ログアウトして再度ログインし、SSO が正しく動作することをテストします。

## 新しい ID プロバイダー（IdP）の追加

新しい IdP を追加するプロセスは、既存の[SSO 構成](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)に似ていますが、いくつかの重要な変更が含まれています:

- **新規フィールド：**「IdP name」と「IdP description」（オプション）。これらのフィールドは、特に複数の IdP が使用されている場合、ログイン時にユーザーと管理者が正しい IdP を識別するのに役立ちます。

  これらのフィールドは管理者設定に表示され、ユーザーが SSO 経由でログインしたときに表示される可能性があるため、名前は意図的に設定することをお勧めします（例えば、ビジネスユニットや IdP 名）。

  ![idP-name-and-IdP description.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016020733970_idP-name-and-IdP%20description.png)
*IdP 名と IdP 説明を追加するオプション*
- **読み取り専用フィールド:** 「Callback URL」（許可された Callback URL、カスタム Assertion Consumer Service URL、Reply URL）と「Entity ID」（識別子、証明書利用者信頼識別子）は、組織がマルチ IdP プライベート機能を有効にした後、自動的に Miro IdP 設定で生成されます。

  以前は、これらの値はすべての IdP 構成で同じであったため、静的でした。生成後は、これらの値をコピーして、IdP プロバイダー設定の対応するフィールドへの貼り付けが必要です。

  ![Callback-ID-and-Entity-ID-fields.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034166290_Callback-ID-and-Entity-ID-fields.png)
*Callback URL および Entity ID フィールド*

## 複数の ID プロバイダー（IdP）の管理

> **💡** 一度に最大 20 件の ID プロバイダーを追加し、有効にできます。

IdP を追加した後、必要に応じて各構成をオンまたはオフにできます。IdP をオフにするには、**企業** 設定 > **アカウント** > **認証** に移動し、IdP をオフにしてください。

![Toggle-on-or-off-IdPs.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034165010_Toggle-on-or-off-IdPs.png)
*IdP をオンまたはオフにするオプション*

## 複数の IdP を持つメールドメインのログイン表示

ユーザーのメールドメインが複数の IdP 設定にリンクされている場合、ログイン時に 1 つを選択できます。これらの構成に固有のドメインがある場合、ユーザーは該当する IdP に自動ルーティングされます。

![sso-screenshot.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/22437449166610_sso-screenshot.png)
*ログイン時に複数の IdP が表示される様子*
