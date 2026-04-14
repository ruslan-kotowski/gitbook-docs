---
title: iOS のエンタープライズ モビリティー管理（EMM）設定
article_id: 10183062016274
translation_id: 10183062016274
locale: ja
sidebar_position: 4
created_at: '2023-02-20T18:20:46Z'
updated_at: '2025-11-25T15:36:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: desktop-mobile-tablet-app
availability:
  notes: '一般的な: 手順を説明します：VMWare Workspace ONE、Ivanti Neurons（旧MobileIron Cloud）、Intune（Microsoft
    Endpoint Manager）。異なるソリューションをご利用の場合、正しい手順については、ご利用の EMM プロバイダーのドキュメンテーションを参照することをお勧めします。'
---

EMM を利用することで、会社の管理者は、一元化かつ統一された方法で、Miro を組織内で設定し、ユーザーに配布することができます。Miro は、エンドユーザーのデバイスに以下の設定をするプロビジョニングに対応しています。

- 登録フローを無効化。
- 対応する認証プロバイダー（ソーシャル ネットワーク、メールプロバイダーなど）を制限。
- 特定の値、または許可されたメールドメインのリストにユーザー名を限定。
- 詳細な SSO 設定。

## 設定方法

### Miro を組織のアプリディレクトリーに追加する

多くの場合、EMM 設定を有効にするには、Miro を組織のアプリケーション カタログに追加する必要があります。このプロセスは、EMM プロバイダーごとに異なることもあります。それでも通常は、Apple Store から Miro を直接アプリケーション カタログに追加し、デバイスグループ、ユーザーグループなどに合わせ配布ポリシーを設定することになります。

#### 例

**VMware Workspace ONE**

全般的な VMware Workspace ONE 導入ガイドは、[こちら](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications)からご覧いただけます。

1. **[追加]** をクリックし、**[パブリック アプリケーション]** をクリックします。
2. プラットフォームのドロップダウン メニューから **[Android]** を、ソースには **[アプリ ストアを検索]** を選択します。
3. **[名前テキストボックス**に**「Miro」**と入力し、[次へ] をクリックします。
4. Miro アプリを選択し、**プロンプトが表示されたら**、[承認] ボタンを押します。
5. **[保存して割当て]** をクリックしてアプリを公開します。
6. 組織の要件に応じて、割り当てと配布設定を構築します。

Ivanti Neurons

1. **[アプリ] > [アプリカタログ]** に移動し、**[追加]** をクリックします。
2. 「**iOS ストア**」を選択し、ソースとしてお住まいの国を選択します。
3. **Miro**」を検索し、「**Miro」を選択します：オンラインホワイトボード**" 利用可能なアプリケーションのリストから。
4. 組織の要件に応じて、割り当てと配布設定を構築します。

Intune（Microsoft Endpoint Manager）

[MS による Intune の全般的な導入ガイドは](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-ios-ipados)こちらからご覧いただけます。

1. **[アプリ] > [iOS/iPadOS]** に移動し、**[追加]** をクリックします。
2. **[ストアアプリ] > [iOS ストアアプリ]** を**アプリタイプ**として選択します。
3. **[App Store の検索]** クリックします。
4. 使用したいストアの国を選択します。
5. **Miro**」で検索し、「**Miro」を選択してください：オンラインホワイトボード**" 利用可能なアプリケーションのリストから。
6. 組織の要件に応じて、割り当てと配布設定を構築します。

### アプリケーションの事前設定

Miro は、顧客データの設定と保護の統一された方法として、AppConfig を採用しています。多くの EMM ソリューションは AppConfig 形式に対応しています。もしくは、互換モードで対応しています。　お客様のケースに該当する細かい制約については、ご利用の EMM プロバイダーのドキュメンテーションをご覧ください。

#### 例

**VMWare Workspace ONE**

全般的な VMware Workspace ONE 導入ガイドは、[こちら](https://techzone.vmware.com/managing-android-devices-workspace-one-operational-tutorial#deploying-android-applications)からご覧いただけます。

1. **[リソース] > [アプリ]** に移動します。
2. クリック **をクリックします。** をクリックします。 **インストール状況****を クリックします：オンラインホワイトボード** アプリ列。
3. 配布先の **[名前]、[割り当てグループ]**、**[アプリの配信方法]** を定義します。
4. **[マネージドアクセス]** と **[送信設定]** を有効化します。
5. アプリケーション設定を定義します。

Ivanti Neurons

1. 1. **[アプリ] > [アプリカタログ]** に移動します。
   2. **Miroに移動します：オンラインホワイトボード**" セッティング.
   3. **[アプリの設定] > [Apple Managed App Configuration]**（Apple マネージド設定） に移動します。
   4. **[追加]** をクリックして、新しい配布プロフィールを作成します。
   5. 構成プロファイル名を定義します。
   6. **Apple Managed App Setting**（Apple マネージドアプリ設定）を定義します。
   7. **Distribute this App Config**（このアプリの設定を配布）セクションで、配布プロフィールを選択します。

Intune（Microsoft Endpoint Manager）

[MS による Intune の全般的な導入ガイドは](https://learn.microsoft.com/mem/intune/fundamentals/deployment-guide-platform-ios-ipados)こちらからご覧いただけます。

1. 1. **[アプリ] > [アプリの構成ポリシー]** に移動します。
   2. **[追加] > [マネージャーデバイス]** をクリックして、新しいアプリケーション構成を作成します。
   3. 構成プロファイル名を定義します。
   4. **プラットフォーム**として **iOS/iPadOS** を選択します。
   5. **Miroを選択してください：オンラインホワイトボード** を**ターゲットアプリとして** **選択**します。
   6. **構成設定フォーマット**として **[構成デザイナーを使用する]** を選択します。
   7. アプリケーション構成を定義します。
   8. 構成の配布プロファイルを選択します。

## 対応している設定の全リスト

### 「… でログイン」と「登録」のオプションを制限

「登録」オプションが有効になっている場合、「… でログイン」の設定すべてが、登録のフローに作用します。

:::warning
明確に「true」に設定されていない（または存在しない）キーは、「false」に設定されているものとみなされます。そのため、その認証オプションは使用できる（デフォルトの動作）ことになります。
:::

| キー | 種類 | 使用できる値 |
| --- | --- | --- |
| **Facebook** miro.authentication.facebookRestricted | ブール値 | true/false |
| **Google** miro.authentication.googleRestricted | true/false |
| **Microsoft Office 365** miro.authentication.office365Restricted | true/false |
| **Slack**  miro.authentication.slackRestricted | true/false |
| **AppleID** miro.authentication.appleIdRestricted | true/false * Apple デバイスでのみ利用可/span> |
| 登録 miro.authentication.signUpRestricted | true/false |
| **Magic link でのログイン** miro.authentication.magicLinkRestricted | true/false |
| **Enterprise workspace** miro.authentication.enterpriseWorksSpaceDisabled | true/false |

### ユーザー名の制限

シンプルなパスワード認証を維持しつつ、セキュリティーの向上を図りたい場合は、以下のオプションをご利用できます。

| キー | 値 | 詳細情報 |
| --- | --- | --- |
| **事前に定義されたユーザー名** miro.policy.authentication.username | **値の型：**文字列 | このフィールドはロックされ、ユーザーは変更できません |
| **許可リストに追加されたドメイン** miro.policy.authentication.allowedDomains | **値の型：**配列  **値：**@miro.com、@yourdomain.com  * 一部のプロバイダーは、**配列**のデータ型に対応していません。その場合は、型の**文字** 列と JSON 配列を値として使用してください。 ["@miro.com", "@yourdomain.com"]。 | リストに記載されたドメインと一致するメールのみが許可されます。 |

### SSO 設定

組織のセキュリティーを向上させ、エンドユーザーの認証プロセスを簡素化するために、組織管理者は、以下の例のように SSO ポリシーを設定できます。

:::warning
アプリケーション構成の SSO ポリシーが、Miro の組織の SSO 設定と一致していることを確認してください。ポリシーの不一致は、ユーザーがログインできない「ロックアウト」の状態を引き起こす可能性があります。Miro は、ターゲットデバイスに設定を適用する前に、その設定の検証をすることはできません。
:::

|  |  |
| --- | --- |
| 構成キー | miro.policy.sso |
| 構成値の型 | 文字列 |
| ポリシーオブジェクト | \{ "authenticationRestricted" : false, "email": "user@domain.com", "allowedDomains": ["domain1.com", "domain2.com"], "forceSsoLogin": true \} |

| ポリシーオブジェクトの属性 | | | |
| --- | --- | --- | --- |
| パラメーター | 種類 | 詳細情報 | 注記 |
| authenticationRestricted | ブール値 | メインページで「SSO でログイン」が有効化されているか否か。 | **他の構成オプションが提供されている場合は、キーは無視されます。** |
| email | 文字列 | SSO ログイン用に事前定義されたメール。 | フィールドはロックされているので、変更できません。 |
| allowedDomains | ブール値 | SSO を、認証のための唯一の方法として維持します。 | エンドユーザーを、即座に「SSO でログイン」のページに誘導します。**email**と**allowedDomains**以外のオプションは無視されます。他の認証方法は利用できません。 |
