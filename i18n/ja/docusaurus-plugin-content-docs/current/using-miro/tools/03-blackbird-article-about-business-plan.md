---
title: "SCIM \u306B\u95A2\u3059\u308B\u30D0\u30EB\u30AF\u30D0\u30FC\u30C9\u8A18\u4E8B\
  \u306E\u30C6\u30B9\u30C8"
article_id: 25902000474898
translation_id: 25902000474898
locale: ja
sidebar_position: 3
created_at: '2025-04-08T15:00:21Z'
updated_at: '2025-05-07T11:29:05Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

!!!テスト記事!!!

クロスドメインID管理システム（SCIM）を使用すると、Miro と ID プロバイダー（IdP）間でユーザー管理とプロビジョニングの自動化が可能です。

> **利用可能なプラン：**[Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) プラン
> **設定者：**会社の管理者

## 重要ポイント

- **自動プロビジョニングの設定開始前に、SAML ベースの SSO が正しく設定され、Enterprise プランで正常に機能していることが必要です。**
  SAML SSO の設定[ガイド](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)をご覧ください。
- **Miro チームとのグループの同期は任意です。**
  オプションで IdP グループを Miro のチームと同期させることができます。ただし、IdP グループが意図せずまたは一時的に削除され、それによりそのグループ内のすべてのユーザーが Miro で無効化され、ボードやスペースの再割り当てが引き起こされる問題を回避するため、IdP グループを Miro チームと同期しないでください。[Teams API](https://developers.miro.com/reference/enterprise-create-team) を使用してチームを作成および管理できます。SCIM API を使用してグループを管理する方法についての詳細は、[Miro Developers](https://developers.miro.com/docs/groups)をご覧ください。
- **SCIMでのメールアドレスの変更には以下の検証ルールが含まれます：**
  - **マネージドユーザーチェック:**ユーザーの現在のドメインが、SCIMリクエストを発行している組織によって請求されていない場合、メールの更新はブロックされ、400エラーがスローされます。
  - **ターゲットメールドメインの検証:**ターゲットのメールドメインがSCIMリクエストを開始した組織以外の組織によって要求されている場合、メールの更新がブロックされ、400エラーがスローされます。SCIM リクエストを開始した組織によってターゲットのメールドメインが所有されている場合、メールの確認なしでメールの更新が可能です。監査ログは、ユーザーがメンバーである各組織でのアップデートを記録します。
  - **ドメイン制御とSSO:**メール更新は、ドメイン制御（IDC）またはシングルサインオン（SSO）を通じたドメイン検証に基づいて許可されています。ターゲットのメールドメインが、開始された組織によってCDまたはSSOを通じて検証されている場合、更新を進めることができます。
    ![scim-diagram-2.png](images/26547093340306_scim-diagram-2.png)
    *SCIM メール変更検証ワークフローの図*

### Miro の SCIM 運用ルール

- SCIM 同期による変更は、主に新たに割り当てられたユーザーに適用されます。すでにサブスクリプションに参加しているユーザーのステータスは補足されますが、グループ/チームレベルで変更が適用されるため、上書きされない場合があります。例えば、次のように：
  a）ユーザーが Miro 側でチーム 1 のメンバーであり、IDP がそのユーザーをチーム 2 に追加する更新を送信した場合、チーム 1 のステータスは影響を受けません。
  b）IDP がユーザー 1 に対する変更を含む更新を送信した場合、他のチームメンバーには影響はありません。**対応機能** > **グループの同期とプッシュ**で説明されているように、一括してチームのステータスを上書きし、すべてのユーザーを再同期するには、新たなプッシュを試みてください。
- SCIM でプロビジョニングされたすべてのユーザーには、サブスクリプションの*デフォルトのライセンス*が割り当てられます。
  a) フレキシブル ライセンス プログラムを使用しない Enterprise サブスクリプションの場合：フルライセンス。サブスクリプションのライセンスが不足した場合、ユーザーは[制限付き無料](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)ライセンスでプロビジョニングされます。
  b）[フレキシブル ライセンス プログラム](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)が有効になっている Enterprise サブスクリプションの場合：[デフォルトのサブスクリプション ライセンス](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md)に応じて、無料または制限付き無料ライセンス。
  *- デフォルトとは異なるライセンスでプロビジョニングする必要があるユーザーがいる場合:*
  *上記のように、すべてのユーザーはデフォルトのライセンスでプロビジョニングされています。ただし、**UserType** 属性に Full 値を指定すれば、一部または全員を即座に更新することができます。この属性で更新されたユーザーは、ユーザー側でダウンタイムが生じることなく、フルライセンスにアップグレードされます。*
- SCIM でプロビジョニングされたすべてのユーザーは、[ドメイン管理](../../enterprise-administration/canvas-25-admin-features/domain-control/01-domain-control.md)機能の影響も受けます。つまり、ユーザーが ID プロバイダーの 1 つのセキュリティー グループのみでメンバーだったとしても、ドメイン管理設定で 3 つのチームが指定されていた場合、このユーザーはこの 3 つのチームにも追加されることになります。
- サービス保護のため、Miro は 30 秒ごとに利用可能な API コール数を制限します。

  | リクエスト種別 | 制限レベル |
  | --- | --- |
  | GET scim/users    GET scim/users/\{userId\} | 第 1 レート制限レベル 1 |
  | POST scim/users/\{userId\}    PUT scim/users/\{userId\}    PATCH scim/users/\{userId\}    DELETE scim/users/\{userId\} | 第 3 レート制限レベル 3 |
  | GET scim/Groups    PATCH scim/Groups/\{groupId\} | 第 4 レート制限レベル 4 |
  | GET scim/Groups/\{groupId\} | 第 3 レート制限レベル 4 |

  制限レベルの詳細については、[**こちら**](https://developers.miro.com/reference#ratelimiting)をご覧ください。**リクエスト数が制限を超えた場合、Miro は、標準の **429 Too many requests**（リクエストの回数が多すぎます）のエラーメッセージを返答します。**

## 対応している機能

Miro の SCIM スキーマの詳細については[**こちら**](https://developers.miro.com/docs/scim)をご覧ください。

Miro は、以下のプロビジョニング機能をサポートしています。

- **新規ユーザーの作成**
  IdP で Miro アプリケーションに割り当てられた新しいユーザーは、Miro Enterprise サブスクリプションに Enterprise メンバーとして作成されます。同じ名称の Miro のチームに同期されたユーザーグループに追加されたユーザーは、チームメンバーとしてチームに追加されます。
- **ユーザープロファイルの更新をプッシュ**
  サポートされている属性や変更については、以下をご覧ください
- **グループの同期とプッシュ**
  IdP グループとそのメンバーを Miro Enterprise サブスクリプションのチームに同期し、ユーザーのメンバーシップを自動管理します。<span>継続的な同期により、同期された Miro のチームにはグループのユーザーに関する特定の更新情報が送信されますが、プッシュ通知はチームの状態を上書きし、グループを信頼できる情報源として扱います（Miro 側で会社の管理者が手動で変更を行った場合）。
- **グループ/チーム名の分離**
  Miro は名前によってグループとチームを同期させるので、名前は完全に一致している必要があります。ただし、最初の同期が作成された後は、いずれか一方または両方に、便利な名称を付けることができるようになります。切り離しの例については、[こちら](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)をご覧ください。
- **グループ / チームからユーザーを削除（Enterprise サブスクリプションからの削除とは別。以下参照）**
  グループからユーザーを削除すると、同期された Miro チームから（次のグループプッシュ時に）ユーザーも削除されます。
- **ユーザーを非アクティブ化する**
  ユーザーを非アクティブ化 / 削除するか、IdP でユーザーのアプリケーションへのアクセスを無効にすると、*非アクティブ化されます*。ユーザーはご利用の Miro Enterprise プランで非アクティブ化されます。</span>ユーザーを非アクティブ化すると、状況に応じて、非アクティブ化されたユーザーのコンテンツは最も古いチーム管理者に再割り当てされる場合があります。
  ー IdP 側でユーザーを非アクティブ化する一方、Miro アプリへの割り当ては維持する場合、そのユーザーの Miro 側でのチームメンバーシップは変更されず、コンテンツは再割り当てされません。ユーザーは、**アクティブ**から**非アクティブ**の状態に切り替わるだけで（ユーザーのセクションも変更）、ライセンスの消費は停止します。
  ー 同期されたチームのメンバーである IDP 内のユーザーを削除、あるいは Miro アプリから割り当てを解除して非アクティブ化する場合、ユーザーは*同期された* Miro チームからも削除され、*該当チーム内*のコンテンツは最も古いチームの管理者に再割り当てされます。
  - ユーザーが*IDP で削除*されるか、Miro アプリから*割り当てを解除*されることで非アクティブ化をトリガーした場合、ユーザーがどの*同期された*チームのメンバーでもない場合、ユーザーのチームメンバーシップは変更されず、コンテンツも再割り当てされません。
  **Enterprise サブスクリプションからのユーザーの削除**は、デフォルトでは対応していません*。*それでも、[API を使用して手動で機能を追加](https://developers.miro.com/docs/scim#section-delete-user-by-id)し、ユーザーを**非アクティブ**状態に設定するのではなく、サブスクリプションから完全に削除することができます。このシナリオでは、コンテンツは、チームメンバーに再割り当てされます。自動的に再割り当てされたコンテンツに対して所有権を取得する管理者を設定することはできません。ただし、これは[Miro の設定でユーザーを手動で非アクティブ化する場合に設定できます。](../../enterprise-administration/user-management/01-deactivated-users.md)
- **ユーザーを再度アクティブ化する**
  アプリケーションにユーザーを再度割り当てるか、IDP におけるユーザープロフィールを再アクティブ化すると、以前にプロビジョニングされ、非アクティブ化されていた場合、Miro Enterprise サブスクリプションでユーザーが再アクティブ化されます。
- **支払いグループ割り当ての自動化**
  SCIM を使用して[支払いグループ](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/01-billing-groups.md)に新規ユーザーを自動で割り当てます。ID プロバイダー（IdP）が設定されたら、コストセンターを支払いグループにリンクします。これにより、これらのコストセンターの現在および将来のユーザーが、適切な支払いカテゴリーに自動的に分類されます。

直接**Delete** API コールを送信することにより、Enterprise プランからユーザーを削除することもできます。資料は[こちら](https://developers.miro.com/docs/scim#section-delete-user-by-id)をご覧ください。ただし、ユーザーを削除できるのは*直接*コールのみです。**ID ソリューション**が起動した*削除*イベントは**非アクティブ化**のリクエストとして扱われます。

### 対応している属性

:::warning
以下にご注意ください：
- **メール** / プライマリー パラメーター / 一意の識別子 / **ユーザー名** は、Miro が要求する唯一の値であり、メール形式である必要があります。
ー メールの更新は、すでに同期されたユーザーに対してのみ可能です。つまり、IdP と Miro のメールアドレスが同じ場合、最初の同期を実行しなければなりません。そうしないと、Miro はユーザーを認識せず、新しいメールアドレスの下に重複した Miro プロフィールが作成されることになります。
ー メールの更新は、ユーザーの IdP プロフィールで行われ、割り当てリストには表示されません。
- 他の属性とは異なり、ユーザーの**メール**を更新すると、通知が送信されます。古いメールアドレスと新しいメールアドレスの両方に、Miro にログインするためには新しいメールアドレスを使用することを知らせるメッセージが送信されます。
:::

| 属性名 | SCIM 属性（クレーム） |
| --- | --- |
| メール | ユーザー名  **メール形式であることが必要** |
| *以下のリストの属性は必須ではなく、存在すれば Miro によって受け入れられます（Miro に送信された他の属性は無視されます）。* | |
| フルネーム | displayName      フォーマット済み;      givenName + " " + familyName;      userName |
| ユーザータイプ | ユーザータイプ サポート値:フル |
| アクティブ | アクティブ       サポート値: "true" または "false" |
| プロフィール写真 | **photos.^[type=='photo'].value** または     **photos.^[type==photo].value**（Okta）     **photos[type eq "photo"].value**（Entra）        画像に対しテキスト URL である必要があります。  対応しているファイル形式：jpg、jpeg、bmp、png、gif  ファイル形式を定義するには、URL に定義されたファイルの拡張子を含める必要があります（例：`https://host.com/avatar_user1.jpg`）または、URL へのリクエストでファイルコンテンツと一緒に Content-Type ヘッダーを返す必要があります（例：Content-Type = 'image/jpeg'）  ダウンロード可能な最大ファイルサイズは次の通りです:31457280 バイト |
| ユーザーの役割 | roles.^[primary==true].value（Okta）      roles[primary eq "True"].value（Entra）  サポート値： **ORGANIZATION_INTERNAL_ADMIN** **ORGANIZATION_INTERNAL_USER** |
| 従業員番号 | 社員番号 |
| コストセンター | costCenter |
| 組織 | 組織 |
| 課 | 課 |
| 部署 | 部署 |
| マネージャー名 | manager.displayName |
| マネージャー ID | manager.value  "value" フィールドは SCIM 標準では String 型ですが、managerId 内部 Miro フィールドは Long 型です。「value」属性がない場合       数値ではない場合、値は無視されます |

:::warning
パスワードは変更できません。また、当面は対応予定はありませんのでご了承ください。
⚠️ **Username**、**UserType**、および**roles.value** は[非アクティブ化されたユーザー](../../enterprise-administration/user-management/01-deactivated-users.md)に対しては更新できません。
:::

すべての属性は、エクスポートされた CSV ユーザーリストに表示され、[アクティブなユーザー](../../enterprise-administration/user-management/12-user-management-overview-on-enterprise-plan.md)セクションからダウンロードできます。

![会社設定でCSVとしてダウンロード.jpg](images/26547046267154_download%20as%20CSV%20in%20company%20settings.jpg)
*ユーザーリストをダウンロードするオプション*

![mceclip3.png](images/26547093348754_mceclip3.png)

## SCIM の設定

### ステップ 1：Miro で SCIM オプションを有効にする

Miro Enterprise プランの SCIM を有効にするには、**会社**の設定 > **Enterprise のインテグレーション** で、 SCIM プロビジョニング機能を**有効</strong>にします。<strong>そこで、IdP を構成するためのベース URL と API トークンを取得できます。**

![scim.png](images/26547046273938_scim.png)
*Miro での SCIM 設定*

### ステップ 2ID プロバイダーを設定する

この設定は、使用する ID プロバイダーによって異なります。Miro は、あらかじめ設定された Okta と Entra ID に対応していますが、SCIM の設定が可能であれば、任意の ID プロバイダーを使用することができます。

OKTA ー設定手順は[こちら](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md)をご覧ください。

Entra ID ー 設定手順は[こちら](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)をご覧ください。

## 新しいトークンを生成する

1。会社の**設定** > **Enterprise インテグレーション** に移動します。

2.<span>**SCIM プロビジョニング**のセクションで、**新しいトークンを生成する**をクリックします。

![scim.png](images/26547046273938_scim.png)
*Miro での SCIM 設定*

2.**新しい SCIM トークンを生成**画面で、**生成**をクリックします。

![generate_token.png](images/26547093353362_generate_token.png)

3新しいトークンを生成したら、IdP プロバイダーで新しいトークンを構成する必要があります。

## 起こり得る問題と解決方法

*1。許可リストエラーが原因でユーザーがプロビジョニングされない。*
![mceclip0.png](images/26547093355154_mceclip0.png)
*Okta ID プロバイダーのエラー例*

[**セキュリティー**設定](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)の許可リストに、ユーザーのドメインアドレスが追加されていることを確認してください。

*2.ある ID ソリューション（IDP1）でエンドユーザーを認証しながら、別の ID ソリューション（IDP2）を介して SCIM を有効にしたい場合、次の 2 つの条件を満たすことで可能です。*

1. IdP2 はベアラートークンを使用して API コールを行うことができます。
2. 両方の ID プロバイダーが同期している（つまり、SCIM でプロビジョニングされたユーザーは IDP1 にも存在するので、Miro で認証することができる）。

詳細については、[Miro のサポートチームまでご連絡ください](https://help.miro.com/hc/en-us/requests/new?referer=help-center-article)。
