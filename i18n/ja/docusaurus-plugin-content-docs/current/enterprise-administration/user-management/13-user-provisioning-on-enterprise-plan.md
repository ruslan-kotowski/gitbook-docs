---
title: "Enterprise \u30D7\u30E9\u30F3\u306E\u30E6\u30FC\u30B6\u30FC \u30D7\u30ED\u30D3\
  \u30B8\u30E7\u30CB\u30F3\u30B0"
article_id: 4403139914130
translation_id: 4403139914130
locale: ja
sidebar_position: 13
created_at: '2021-07-01T07:59:23Z'
updated_at: '2025-11-25T16:05:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: scim
---

自動プロビジョニングを利用すると、会社のドメイン内のすべての新しいユーザーが Enterprise サブスクリプションにルーティングされ、会社のアセットにアクセスできるようになります。

Miro Enterprise はいくつかのプロビジョニングオプションを提供しています： 招待、ジャストインタイムプロビジョニング（JIT）、クロスドメイン ID 管理システム (SCIM)、およびドメイン制御。

> **対象プラン：**Enterprise プラン

## 招待

ダッシュボードの **[メンバーを招待する]** ボタンを使うとサブスクリプションにユーザーを招待できます。招待はすぐに送信され、それ以上の設定は必要ありません。

作業を共有し、Miroでのコラボレーションの詳細については、[Enterprise プランでの招待の管理](05-manage-user-invitations-on-enterprise-plan.md)と[ボードの共有とコラボレーターの招待](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)をご覧ください。

![invite_members_button.jpg](../../../../../../docs/enterprise-administration/user-management/images/21017653284754_invite%20members%20button.jpg)*Miro ダッシュボード上のメンバー招待オプション*

## ジャストインタイム プロビジョニング（JIT）

JIT プロビジョニングは、[シングルサインオン (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) と統合されており、企業の SSO ドメインに登録されたすべての新しいユーザーを特定のチームに自動的に追加します。
JIT プロビジョニングは、Miro の SSO 設定で簡単に有効にできます。[SSO の設定方法を学ぶ](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)。

![user_provisioning_jit_provisioning.png](../../../../../../docs/enterprise-administration/user-management/images/21017682931730_user_provisioning_jit_provisioning.png)*SSO 設定での Just-in-Time (JIT) プロビジョニングの有効化*

## クロスドメイン アイデンティティ管理システム (SCIM)

SCIM は、[シングルサインオン（SSO）](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md)と統合されており、選択したアイデンティティプロバイダー（IdP）を通じて、Enterprise プランのユーザーを自動的にプロビジョニングし、管理することができます。

SCIM を有効にすると、特定のチームにユーザーを追加したり、詳細やメールアドレスを更新したり、選択した IdP 内でのアクティベーションステータスを管理することができます。この機能は、Miro アカウントと IdP との間のユーザー情報の交換を自動化します。

SCIM は、Miro と IdP の間でユーザー情報の交換を自動化し、IdP から Enterprise プランへの従業員のアクセスを一元的に管理できるようにします。

[SCIM 機能](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md)について詳しく学び、[Entra ID](../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)、[OKTA](../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md)、または[OneLogin](../security-integrations/system-for-cross-domain-identity-management-scim/06-setting-up-automated-provisioning-with-onelogin.md)の設定手順を確認してください。

## ドメイン制御

[ドメイン制御](../canvas-25-admin-features/domain-control/01-domain-control.md) により、Enterprise サブスクリプションに新しいユーザーを自動的に追加し、企業ユーザーが別の Miro サブスクリプションを作成する機能を制限し、ドメイン内のユーザーアクティビティーを監視することができます。

ドメイン制御を利用すると、会社ユーザーに対してプロビジョニングのルールを設定できます：

- ドメインの新規登録ユーザーは、サブスクリプションへのアクセスをリクエストすることができます。
- ドメインの新規登録ユーザーは、自動的にサブスクリプションに参加できます。
- ドメインの新規登録ユーザーは、自動的にサブスクリプションに参加できますが、ドメインのユーザーが新たに Miro のチームを作成することはできません。

![Add-a-domain-Image1.png](../../../../../../docs/enterprise-administration/user-management/images/21017653288082_Add-a-domain-Image1.png)*Miro セキュリティ設定内のドメイン制御*

## ライセンスの仕組み

会社の管理者は、新規ユーザーを招待する際、サブスクリプションの設定に応じて、招待するユーザーのライセンスを選択することができます。

管理者以外が招待したユーザーや、JIT、SCIM、ドメイン制御でサブスクリプションに自動的にプロビジョニングされたユーザーには、*デフォルトのライセンス*が割り当てられます。

- **非フレキシブル ライセンス（非 FLP）のプランの場合:** デフォルトのライセンスはフルライセンスです（組織のフルライセンスが不足している場合、実質上照合されたユーザーには[制限付き無料ライセンス](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)が付与されます）。
- **フレキシブル ライセンス プログラム（FLP）のプランの場合:** デフォルトのライセンスはFreeまたは[制限付き無料ライセンス](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)です。

:::note
私たちの[Enterpriseライセンスモデルについて](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md)、[フレキシブル ライセンス プログラムのライセンス管理](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md)、[リクエスト管理を使用したライセンスの割り当てとアップグレード管理](09-request-management-on-enterprise-plan.md)について学びましょう、[ソフトウェア資産管理](../security-integrations/software-asset-management/01-software-asset-management-miro-enterprise.md)でライセンス使用状況を追跡する方法。
:::

## よくある質問

ドメイン制御を設定して新しいユーザーをキャプチャする場合、特定のドメインを持つユーザーを Enterprise サブスクリプション内のデフォルトチームに自動的に割り当てるという点で、JIT と同様に機能しますか？

はい。ただし、ドメイン制御では、Enterprise プラン用に SSO を設定する必要はありません。SSO なしでも機能します。

自動プロビジョニングされたユーザーがボードでの作業を開始するまで、フルライセンスを受け取るのを防ぐことができますか？

はい、[フレキシブル ライセンス プログラム](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md)でこれが可能です。

Enterprise サブスクリプションに複数のプロビジョニング オプションを設定できますか？

はい、複数のプロビジョニングのオプションを同時に使用できます。
