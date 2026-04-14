---
title: "Google Meet \u3068 Miro \u306E\u30B3\u30E9\u30DC\u30EC\u30FC\u30B7\u30E7\u30F3"
article_id: 6251039904530
translation_id: 6251039904530
locale: ja
sidebar_position: 10
created_at: '2022-06-24T07:22:19Z'
updated_at: '2025-11-25T16:08:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: google-meet
---

Google Meet と Miro のコラボレーションで、より魅力的でインタラクティブな会議を実現しましょう。Google Meet を使いながら、Miro ボードを表示させたり、ボードを作成することができます。また、Miro のプロフィールなしで、誰とでもコラボレーションできます。作業内容を保存しておけば、いつでもアクセスできます。

Google Meet インテグレーションは、Google Workspace アドオンの一部になりました。既に Miro アドオンをインストールしているユーザーは、引き続き Google Meet にアクセスできます。Miro アドオンをインストールしていないユーザーが、Google Meet のアドオンにアクセスするには Miro アドオンが必要です。

Google Workspace アドオンを Miro にインストールする方法については、[こちら](07-miro-for-google-workspace.md)をご覧ください。

## 重要事項

- Google Meet で Miro ボードを開くには、会議の主催者である必要はありません。会議の参加者であれば誰でも Google Meet で Miro ボードを開くことができます
- Miro プロフィールを持たないユーザーやログインしていないユーザーは、適切な権限がボードに設定されている限り、プロフィールを作成しなくても、[ゲスト](../../using-miro/sharing-boards/07-collaboration-with-guests.md)として Miro ボードを表示することや、ボードに参加することができます。
- プロフィールなしで Miro ボードを作成した場合、まず Miro にメールアドレスを提供するよう求められ、その後、24 時間以内に作業を保存して Miro プロフィールを作成するために必要な情報がメールされます
- 管理者には、組織内の特定のチームやユーザーが Google Meet で Miro を使用することを制限するオプションがあります。詳細については、[こちら](https://support.google.com/a/answer/6089179?hl=en)をご覧ください。

:::warning
Google Meet の Miro は、Chrome シークレットモードまたはコンパニオンモードに対応しておらず、Chrome と Edge ブラウザーにのみ対応しています。
:::

## Google Meet で Miro を設定する方法

1. Google Meet を開始します。
2. **[アクティビティー]** タブをクリックして、Miro を開始します。

   activities.jpg
   *Google Meet のアクティビティー*
3. アプリの一覧から Miro を選択します。

   ![Miro_platform_in_Google_Meet.jpg](../../../../../../docs/integrations-apps/google/images/21016033814290_Miro%20platform%20in%20Google%20Meet.jpg)*Google MeetにおけるMiroアドオン*
4. ここでは、Miro プロフィールにサインインして Miro ボードを開始するか、プロフィールなしで Miro ボードを開始するかを選択します。
   プロフィールなしで Miro ボードを作成すると、24 時間以内に作業を保存して Miro プロフィールを作成するために必要な情報がメールされます。

   /span>Miro プロフィールに新しく登録するには、ログインを選択し、ログインウィンドウの右上にある [登録] をクリックします。

   sign_in_or_create_a_board.jpg
   新規 Miro ユーザー向けのログインオプション
5. Miro にログインすると、自分のボードがすべて表示されます。今回の会議で使用するボードを選択します。編集が許可されているボードのみ選択できます。![google_meet_board_picker.png](../../../../../../docs/integrations-apps/google/images/21016020380562_google_meet_board_picker.png)
   Google Meet で使用する Miro のボードピッカー/span>
6. 会議の参加者全員にボードへの適切なアクセスレベルを選択し、**[Embed board]（ボードの埋め込み）** をクリックします。アクセスレベルは、4 つのオプションから選択できます。閲覧 / コメント / 編集の権限を与えるか、ボードを非公開にし、Miro にログインしてボードにアクセスできるユーザーの権限を Miro 側で設定します。
   > ⚠️ **無料チームのボードを埋め込む場合は、[全員がコメント可](../../plans-billing/miro-plans/09-free-plan.md)のオプションはサポートされません**。

   > ✏️ この手順で非公開を選択しても、 [Miro 側でボードが公開設定されていれば、](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md)Google Meet 内でもデフォルトで公開されることになります。ただし、Google Meet 側で埋め込まれたボードに設定したアクセスレベルは、Miro 側で設定されたボード共有設定には影響を与えません。 [詳しくはこちら](../integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md)

   > [️✏️ Enterprise プランの Miro ユーザーの場合、アクセス設定は組織全体のアクセス管理に準ずるので、](../../enterprise-administration/user-management/05-manage-user-invitations-on-enterprise-plan.md)共有オプションの一部は制限されている可能性があります。さらに詳しい情報： インテグレーションの埋め込みに関する Enterprise 共有ポリシーの管理

   ![google_meet_board_access_settings.png](../../../../../../docs/integrations-apps/google/images/21016020382098_google_meet_board_access_settings.png)*Google Meet 内のボードアクセス設定*
7. **[Start activity]（アクティビティーを開始）**をクリックして、会議の参加者全員と Miro ボードを共有します。会議は、センターステージで開きます。ボード上で作業するよう招待されたすべてのユーザーに確認メッセージが表示されます。

   ![google_meet_starting_collaboration.png](../../../../../../docs/integrations-apps/google/images/21016020384018_google_meet_starting_collaboration.png)*Google Meet の Miro ボードでアクティビティを開始します。

   会議の参加者に、ボードに参加してコラボレーションするように求めるポップアップ通知が表示されます。*/em>/span>/span>

   Google_Meet_Miro_collaboration.jpg

Google Meet と Miro のコラボレーションで、プレゼンターと参加者の画面は次のとおりです。

![google_meet_presenter_view.png](../../../../../../docs/integrations-apps/google/images/21016033821458_google_meet_presenter_view.png)*Miro for Google Meetの発表者ビュー。*

![Google_meet_attendee_view.png](../../../../../../docs/integrations-apps/google/images/21016033817746_google_meet_attendee_view.png)*Miro for Google Meetの参加者ビュー。*

## Google Meet のアクティビティーの終了

Miro ボードでの作業が終了したら、アクティビティーを終了しますが、その後も Google Meet で通話を続けることができます。

1. [End activity]（アクティビティーを終了） **をクリックします**
2. 確認を求める新しいポップアップが表示されます。**[続行]** をクリックしてアクティビティーを終了し、通話に戻ります。これで Miro のコラボレーションは終了しますが、いつでも新しいコラボレーションを開始することや、Meet の右下にある [アクティビティー] アイコンをクリックして、別のボードを選択することができます。

   ![google_meet_end_activity.gif](../../../../../../docs/integrations-apps/google/images/21016033824146_google_meet_end_activity.gif)*Google MeetのMiroボード上でのコラボレーションの終了*

[Google Meet と Miro のコラボレーション](https://support.google.com/meet/answer/12312774)の詳細はこちらをご覧ください。
