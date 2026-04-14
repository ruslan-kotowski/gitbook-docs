---
title: "\u5BFE\u5FDC\u30A2\u30D7\u30EA\u3078\u306E Miro \u30DC\u30FC\u30C9\u306E\u57CB\
  \u3081\u8FBC\u307F\u3092\u8A31\u53EF\u307E\u305F\u306F\u5236\u9650\u3059\u308B\u65B9\
  \u6CD5"
article_id: 4405088016274
translation_id: 4405088016274
locale: ja
sidebar_position: 5
created_at: '2021-08-13T05:51:25Z'
updated_at: '2025-11-25T16:06:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: live-embed
---

Miro には、Zoom[、](../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md)Microsoft Teams[、](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md)Jira[、](../../integrations-apps/atlassian/02-miro-for-jira-cloud.md)Confluence [などの](../../integrations-apps/atlassian/01-miro-for-confluence.md)外部アプリで、ユーザーがボードを簡単に共有できるインテグレーションがあります。 Enterprise 管理者は、対応するアプリ内へのボードの埋め込みを許可または制限することができます。

> **対象プラン：**[Enterprise プラン](../../plans-billing/miro-plans/04-enterprise-plan.md)

### 対応アプリへの Miro ボードの埋め込み

対応アプリに Miro ボードを埋め込むと、そのアプリのユーザーが Miro のプロフィールを持っていない場合でも、ボードにアクセスできるようになります。

対応アプリ内でボードを共有しても、Miro 側の共有設定には影響しません。対応アプリに埋め込まれたボードへのアクセス権限の詳細はこちらをご覧ください/span>[。](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

![allow_restrict_embed_customize_embed.gif](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/21019705471122_allow_restrict_embed_customize_embed.gif)*アクセス制限付きMiroボードの埋め込み*

### 対応アプリにボードの埋め込みを制限または許可する方法

> **実行可能なユーザー**：会社の管理者

Enterprise プランをご利用の会社の管理者は、対応アプリに Miro ボードを埋め込む権限を設定できます**。**この設定をオンにすると、組織やチームで公開共有が制限されている/strong>場合でも、ユーザーは Miro ボードを埋め込むことができます。

対応アプリ内での未登録ユーザーとの共有を許可または制限するには：

1. **組織の** **設定に**移動します。
2. **セキュリティー**」で「**共有**」をクリックします。
3. コンテンツ]セクションまでスクロールダウンし、[**埋め込みによる共有を許可]**のオン/オフを切り替えます。

:::note
[制限付き無料ライセンスユーザーの埋め込みボードアクセス権の詳細](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)をご覧ください。
:::

![allow-embedding.pngEnterprise](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803639826_allow-embedding.png)
*プランで埋め込みによる共有を。*

この設定をオフにすると、以前に埋め込まれたボードは使用できなくなります。新しいボードを埋め込むこともできますが、ビジターにはアクセス権が必要になります。

ユーザーは、特定のボードが埋め込まれたアプリの一覧をすべて閲覧し、ボードへのアクセスをいつでも取り消すことができます。全てはボードの共有設定から行うことが可能です。埋め込みボードへのアクセス権の管理と取り消しの方法については、こちらをご覧ください/span>[。](../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

### 対応アプリに埋め込まれたボードを、パスワード保護することはできますか？

会社の設定では、管理者は公開リンクで共有されているMiroボードにパスワードを要求するオプションがあります。

Miro 側でパスワードを設定した公開リンクでボードを共有すると、これらの設定は対応アプリに埋め込まれたボードには反映されません。Microsoft Teams や Zoom などのアプリ/span>[にボードを埋め込む際に、パスワード保護は行なわれません](../../integrations-apps/microsoft/microsoft-teams/05-embed-miro-boards-in-microsoft-teams.md)。

その代わり、ボードが Miro 側で共有[されていない限り、埋め込みボードには対応アプリ内でのみアクセス可能で、アプリ外（ウェブブラウザーなど）では利用できません](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)。
