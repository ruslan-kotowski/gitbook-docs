---
title: Enterprise 2 要素認証（2FA）– ユーザーガイド
article_id: 7935469290002
translation_id: 7935469290002
locale: ja
sidebar_position: 2
created_at: '2022-10-04T09:00:42Z'
updated_at: '2025-11-06T13:50:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '対象: Starter、Business、Education、Enterprise プラン'
---

## 2 要素認証 (2FA) とは

2 要素認証 (2FA) はオンラインアカウントのセキュリティーを強化します。 会社の管理者が 2 要素認証 (2FA) を有効にすると、メールアドレスとパスワードで Miro にログインするたびに、追加のセキュリティーレイヤーが適用されます。このステップにより、通常のログイン認証情報だけでは不十分で、アカウントの保護が向上します。

:::tip
あなたの組織で二要素認証（2FA）を有効にする方法を、[Enterprise プラン](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)向け、および[その他のすべてのプラン](../../../administration/security-compliance/01-two-factor-authentication-2fa.md)向けに学びます。
:::

## 二要素認証（2FA）のセットアップ方法

**新規ユーザー：** 会社のメールアドレスで[登録](https://miro.com/signup/)する際に、2FA を有効にするよう求められます。
**既存ユーザー：** 次に[ログイン](https://miro.com/login/)する際、組織が 2FA を要求しており、シングルサインオン（SSO）を使用していない場合は、2FA を設定するよう求められます。

1. モバイル端末に認証アプリをダウンロードしてください。 Google Authenticator、Microsoft Authenticator、Authy などの認証アプリは、Miro へのセキュアなサインインのために、時間ベースのワンタイム（TOTP）コードを生成します。どの認証アプリを選択するかについては、会社の管理者または IT 管理者にお尋ねください。

2. Miro の 2FA 設定画面で **認証アプリを持っています** をクリックします。

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653633554_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *認証アプリの確認*
3. 認証アプリを使用すると、次の 2 つのオプションがあります：


   QR コードをスキャン

   1. 認証アプリを開きます。
   2. アプリを使って QR コードをスキャンしてください。
   3. スキャン後、Miroで**「コードをスキャンしました」**をクリックします。

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683263122_2FA-setup-step-2-Scan-QR-code.png)*QR コードのスキャン*

   Miro コードの手動入力

   1. QR コードをスキャンできない場合は、Miro の**QR コードをスキャンできませんでしたか？**をクリックしてください。
   2. Miro は認証コードを提供します。このコードを**コピー**してください。
   3. 認証アプリを開き、コピーしたコードを貼り付けます。
   4. アプリにコードを追加したら、Miro で**コードを追加しました**をクリックします。

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653636754_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*認証アプリに貼り付けるためのMiroコードをコピー*
4. 認証アプリが 6 桁の認証コードを生成します。このコードをMiroに入力し、**コードを検証**をクリックします。

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653634706_2FA-setup-step-3-enter-6-digit-code.png)
   *6 桁のコードを検証中*
5. 6 桁のコードでアカウントの認証に成功すると、Miroはリカバリーコードを提供します。このコードを安全に保存するには、**コピー**をクリックします。2FAをリセットできるため、このコードは非常に重要です。

   コードを記録したことを確認するには、**このコードを記録しました**をクリックし、**続行**を選択してプロセスを完了してください。

   ![Save-2FA-recovery-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683265554_Save-2FA-recovery-code.png)*リカバリーコードの保存*

## 2 要素認証（2FA）によるログイン

アカウントに2要素認証（2FA）を正常に設定すると、ログインしようとするたびに、Miroは6桁の時間ベースのワンタイム（TOTP）コードの入力を促します。

このコードは認証アプリによって生成され、アカウントのセキュリティーを強化します。認証アプリを開いて現在のコードを取得し、それをログインページで入力するだけでアカウントにアクセスできます。

![2fa-user-guide.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/20847806879634_2fa-user-guide.png)
*2FAを用いたMiroへのサインイン*

ログインプロセスを再開するようプロンプトが表示される前に、3 回コードを入力することができます。

![Too-many-attempts.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683267346_Too-many-attempts.png)*2FA でのログイン試行回数超過*

### 二要素認証（2FA）デバイスの信頼

管理者が設定している場合、セキュリティー保護されたデバイスを使用して 2FA でアカウントにログインする際に、「**このデバイスを信頼する**」チェックボックスを選択できます（共有または一般アクセス可能なコンピューターからログインする場合は、「**このデバイスを信頼する**」を使用しないでください）。この操作をすると、指定された時間が経過するまで、二番目の要素を入力せずにログインできるようになります。この期間は管理者によって 7 日から 90 日の間で設定されます。

![2FA-signin.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/19612606396818_2FA-signin.png)

*二要素認証でサインインする際、チェックボックスの横にデバイスを信頼する期間が表示されます*

「このデバイスを信頼する」というオプションが表示されない場合は、管理者が組織でこのオプションを有効にしていません。

新しいデバイスでサインインした場合、または信頼済みデバイスのクッキーを消去した場合は、2 要素認証が再度要求されます。

## 二要素認証（2FA）のリセット方法

認証アプリに問題がある場合、デバイスを紛失した場合、またはその他の理由で 2 要素認証をリセットする必要がある場合は、以下の手順を実施してください：

### リカバリーコードを持っている場合

1. 「**二要素認証をリセット**」をクリックします。
2. 初回の 2FA 設定時に保存したリカバリーコードを使用します。再度設定プロセスを進め、認証アプリを再設定してください。

![Reset-two-factor-authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683268114_Reset-two-factor-authentication.png)*二要素認証をリセットするオプション*

### リカバリーコードがない場合

リカバリーコードを紛失したり、自己リカバリーフローを利用できない場合は、管理者に 2FA のリセットを依頼する必要があります。

もしあなたのメールドメインが組織の認証済みドメインの一部でない場合、管理者がリセットを開始することはできません。あなた自身で2要素認証（2FA）のリセットを依頼する必要があります。その後、管理者が承認することが可能になります。

管理者は、管理者がリセットを開始した場合に限り、組織でメールドメインが認証されているユーザーの2要素認証をリセットできます。ユーザーがリセットを依頼した場合、組織内のいずれかの管理者が承認することができます。

以下の手順に従ってください：

1. **管理者にリセットを依頼** をクリックします。
   ![2fa-user-reset.png](https://help.miro.com/hc/article_attachments/24650834680466)
   *リカバリーコードがない場合は管理者に 2FA のリセットを依頼*
2. 2FA を使用している複数の組織に所属している場合は、どの組織の管理者にリクエストを行うかを選択してください。
3. 認証コードが記載されたメールが届きます。
4. 認証コードを入力してください。
5. 選択した管理者にリクエストが送信されたことの確認が表示されます。
6. 管理者が 2FA をリセットした場合、次回ログイン時に 2FA の設定を行う必要があります。

## よくある質問

なぜ 2FA を設定する必要があるのですか？

2 要素認証は組織のセキュリティーを強化します。
会社の管理者によりこの要件が強制されている場合、すべての非 SSO ユーザーはログインに 2 要素認証を使用する必要があります。

ログインするたびに 2FA を使用しなければなりませんか？

はい。初期設定完了後、アカウントのセキュリティーのため、ログインのたびに認証アプリを使用する必要があります。

2FA を設定しようとしましたが、コードは正しいにもかかわらず「無効なコード」というエラーが表示されました。どうすればいいですか？

デバイスのタイムゾーン、日付、時刻が正しく設定されていることを確認してください。問題が解決しない場合は、別のデバイスで 2FA を設定してみてください。

共有デバイスを誤って信頼してしまったら？

共有デバイスを誤って信頼してしまった場合、そのデバイスで Miro のクッキーをクリアしてください。やり方は簡単です：

1. ブラウザーのアドレスバーの左側にある、スライダーのアイコンをクリックしてください。
2. メニューの「Cookie とサイトデータ」をクリックしてください。
3. 次に、「デバイス上のサイトデータを管理」をクリックします。
4. クッキーとサイトデータをクリアするには、リストされている各 URL の横にあるゴミ箱アイコンをクリックしてください。

デバイスからサイトデータをクリアすると、2 要素認証を使って再度ログインが必要です。

信頼できるデバイスへのアクセスを失った場合はどうなりますか？

信頼期間が切れる前に信頼済みデバイスへのアクセスを失った場合、「**すべての場所からログアウト**」オプションを使用して、使用しているデバイスを除くすべてのサインイン済みデバイスからアクセスを削除できます。この操作により、他のすべてのデバイスからログアウトし、信頼できるデバイスから2FAを失効させます。ユーザープロフィールの設定で「**すべての場所からログアウト**」リンクを見つけることができます。その後、利用可能なデバイスで再度2FAサインインプロセスを行う必要があります。
