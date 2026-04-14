---
title: サードパーティー製アプリに埋め込まれたボードのアクセス権限
article_id: 4411883577618
translation_id: 4411883577618
locale: ja
sidebar_position: 1
created_at: '2021-12-08T10:13:42Z'
updated_at: '2025-11-25T16:07:55Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: confluence
availability:
  notes: 'ユーザー: ボード所有者、ボード共同所有者 プラン: すべてのプラン プラットフォーム: ブラウザー、デスクトップアプリ'
---

Miro は、[Microsoft Teams](../microsoft)、[Confluence](../atlassian/01-miro-for-confluence.md)、Notion、Google Meet などのサードパーティー環境においてボードで簡単にコラボレーションできるインテグレーションを提供しています。[Miro マーケットプレイス](https://miro.com/marketplace/category/embed-miro/)で他の対応アプリを確認できます。ボードを埋め込む際に、ユーザーアクセスの異なるレベルを設定でき、Miro 内からこれらの権限を管理できます。

## 埋め込みアクセスを理解する

外部アプリでボードを共有する際、Miro のアクセス権に関わらず、アプリ内のユーザーに、一度限りの閲覧、コメント、または編集権限を付与してコラボレーションを行うことができます。こうしたユーザーは、Miro プロフィールがなくてもアプリ内のボードにアクセスすることができます。つまり、ボードを公開共有しなくても、Miro に未登録のユーザーに対して、外部アプリに埋め込んだボードのアクセス権を設定することができます。

高いセキュリティーを確保するため、1回限りのコラボレーション（ワークショップなど）以外でこの方法を使用することはお勧めしません。組織内で Miro のアクセスを、必要なユーザーに適切に割り当てることをお勧めします。

![embed_Miro_in_Zoom.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020254296722_embed%20Miro%20in%20Zoom.gif) *埋め込みボードのアクセス権設定*

ボードは埋め込んだアプリ内でのみアクセス可能です。埋め込みボードに設定したアクセスレベルは、そのアプリ内でのみ機能し、アプリ外の共有設定には影響しません。例えば、[非公開ボード](../../using-miro/sharing-boards/15-make-a-miro-board-private.md)が、「誰でも閲覧可能」の設定で Microsoft Teams のチャンネルに埋め込まれている場合、その Microsoft Teams チャンネルのユーザーは、Miro にログインせずにボードを閲覧することができます。同じユーザーが、Microsoft Teams チャンネルの外でボードのリンクをたどってボードにアクセスしようとしても、アクセスすることはできません。

ただし、Miro 側のボード共有設定は、外部アプリで設定したアクセスレベルよりも優先されます。例えば、ボードが[Miro 側で公開されている](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)場合、埋め込みボードを非公開としていても、Microsoft Teams では誰でもボードにアクセスできるようになります。

## 埋め込みアクセスの管理と取り消し

対応する外部アプリに埋め込まれたボードへのアクセス権限は、簡単に追跡、管理、取り消すことができます。

埋め込みボードへのアクセス権限を管理し、取り消す方法：

1. **共有** ボタンをクリックして、Miro ボードの共有設定を開きます。
2. **共有設定** を選択します。
3. **埋め込み** タブを開きます。
4. ボードが埋め込まれた外部アプリケーションが表示され、そのインテグレーション名、いつ誰によって埋め込まれたか、そしてアプリ内でのボードのアクセス設定が確認できます。
5. アプリ内のボードへのアクセスを取り消すには、アプリの横にある**アクセスを取り消す**をクリックします。このアクションを取り消すことはできませんのでご注意ください。

ol

![remove_an_access_link.gif](../../../../../../docs/integrations-apps/integrate-miro-with-other-apps/images/21020265344914_remove%20an%20access%20link.gif)
*アクセスリンクの削除*

埋め込みボードへのアクセス権限が取り消されると、アプリ内でのボードへのアクセスが制限されます。Miro 側でボードが共有されていると、権限の取り消し後もアプリ内でボードに継続してアクセスできる可能性があることに注意してください。例えば、

- ボードが、アプリ内で誰でも**編集**でき、Miro 側で[公開共有](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)されて**閲覧**可能な場合、誰もが引き続きアプリ内でそのボードを**閲覧**できます。
- ボードが非公開で、[他のユーザーとメールでのみ共有](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)されている場合、アプリ内で埋め込まれたボードにアクセスするには**ログイン**が必要です。

## 埋め込みのルールと制限

ボードを埋め込む際には、以下のルールと制限にご注意ください。

- [非アクティブ](../../using-miro/tools/troubleshooting/15-the-board-is-locked.md)なボードや、閲覧権限しかないボードは埋め込むことができません。
- [Free チーム](../../plans-billing/miro-plans/09-free-plan.md)に保存されているボードは、コメント権限を付与して埋め込むことはできません。
- [Enterprise プラン](../../plans-billing/miro-plans/04-enterprise-plan.md)のユーザーの場合、アクセス設定は組織全体のアクセス制御に従うため、いくつかの共有オプションが制限される可能性があります。詳細はこちらをご覧ください。[インテグレーションの埋め込みに関する Enterprise 共有ポリシーの管理](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)。
- 一部の古いリンクでは、アクセスレベルとアプリケーションのみが表示され、ボードを作成した者や埋め込まれた日時は表示されません。
- Enterprise 組織で外部アプリ内の Miro ボードの埋め込みを制限したい場合は、[インテグレーションの埋め込みに関する Enterprise 共有ポリシーの管理](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)をご覧ください。
- 埋め込まれたボードへのアクセスリンクの管理は、モバイルおよびタブレット端末ではまだサポートされていません。

[制限付き無料ライセンスユーザー向けの埋め込みボードアクセスの詳細](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)をご覧ください。
