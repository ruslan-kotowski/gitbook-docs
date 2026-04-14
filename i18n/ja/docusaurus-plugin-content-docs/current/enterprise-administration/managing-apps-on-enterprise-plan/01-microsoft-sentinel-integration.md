---
title: "Microsoft Sentinel \u3068\u306E\u30A4\u30F3\u30C6\u30B0\u30EC\u30FC\u30B7\u30E7\
  \u30F3"
article_id: 31325908249362
translation_id: 31325908249362
locale: ja
sidebar_position: 1
created_at: '2025-11-24T18:16:15Z'
updated_at: '2025-12-16T15:49:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: audit-logs
---

## 概要

[Miro](https://miro.com/) コネクターは、[Miro REST API](https://developers.miro.com/reference/overview)を使用して、監査ログおよびコンテンツ活動ログを Microsoft Sentinel に取り込みます。これにより、Microsoft Sentinel 内で Miro ワークスペース活動の監視が集中化され、セキュリティーの脅威検出、インシデント調査、コンプライアンスの報告が可能です。

## データコネクター

このソリューションには2つのデータコネクターが含まれています。

| コネクター | プランの要件 | キャプチャする内容 | 参考資料 |
| --- | --- | --- | --- |
| **Miro 監査ログ (Enterprise プラン)** | Enterprise プラン | ユーザー認証、コンテンツアクセス、チームの変更、管理操作を含む組織全体の監査イベント。 | [API ドキュメント](https://developers.miro.com/reference/enterprise-get-audit-logs) | [監査ログ概要](https://developers.miro.com/reference/audit-logs) |
| **Miro コンテンツログ (Enterprise プラン + Enterprise Guard)** | Enterprise プラン + Enterprise Guard アドオン | アイテムの作成、更新、削除に関するコンテンツ活動の追跡情報で、コンプライアンスとeDiscoveryをサポートします。 | [APIドキュメント](https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch) | [コンテンツログ概要](https://developers.miro.com/reference/board-content-logs) |

## 前提条件

### 一般的な要件

- アクティブな Microsoft Sentinel ワークスペース。
- Miro 組織の会社の管理者ロール。
- Miro OAuth アクセストークン（非期限切れ）。

### コネクタ固有の要件

#### 監査ログコネクタの場合

- Miro Enterprise プラン。
- OAuth スコープ: `auditlogs:read`。
- アクセストークン。

#### コンテンツログコネクタの場合

- Miro Enterprise プラン + Enterprise Guard アドオン。
- OAuth スコープ：`contentlogs:export`。
- アクセストークン。
- Miro 組織 ID。

## インストール

Miro コネクターを設定する方法は2通りあります。

- **オプション 1（推奨）：** エンタープライズインテグレーションを使用します。自動的にトークンを生成する最も簡単なセットアップです。
- **オプション 2（代替案）：** カスタム OAuth アプリケーションを作成します。OAuth アプリ設定をより細かくコントロールできます。

**注意:** オプション 1 を使用する場合、インテグレーションは自動的に組織内でユーザー数が最も多いチームに結びつけられます。オプション 2 を使用する場合、アプリをインストールするチームを選択できます。ただし、チームの選択は収集されるログには影響しません。どちらのオプションも組織全体のログアクセスを提供します。すべてのチームの関連するイベントがログに含まれます。

### オプション 1: Enterprise インテグレーションを使用する（推奨）

これは、多くのユーザーにとって最もシンプルなオプションです。Miro のエンタープライズインテグレーション設定を通じて、自動的に OAuth アプリケーションを作成し、アクセス トークンを生成します。

#### 監査ログ コネクターの場合

1. [Miro の会社設定](https://miro.com/app/settings/)を開く。
2. **アプリとインテグレーション**セクションを展開する。
3. **Enterprise インテグレーション**をクリックする。
4. **SIEM**トグルを有効にする。
5. **アクセス トークン**の値をコピーする。
6. トークンを安全に保管する。

#### コンテンツログコネクタ用

1. [Miroの会社設定](https://miro.com/app/settings/)を開きます。
2. **アプリとインテグレーション**セクションを展開します。
3. **Enterpriseインテグレーション**をクリックします。
4. **eDiscovery**トグルを有効にします。
5. 表示された**アクセストークン**の値をコピーします。
6. ブラウザーのURLから**組織ID**を取得します:
   - ブラウザーのURLを確認して組織IDを探します。
   - URLの形式: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`
   - URLから組織ID（数値）をコピーします。
7. トークンと組織IDを安全に保管してください。

### オプション2: カスタムOAuthアプリケーションの使用（代替）

このオプションは、OAuthアプリケーションの設定をより自由に管理できます。スコープをカスタマイズしたり、複数のインテグレーションを管理したり、手動でOAuthアプリを管理したい場合に使用してください。

#### ステップ 1：Miro OAuth アプリケーションを作成する

1. Miro アカウントにログインします。
2. [Miro のアプリ設定](https://miro.com/app/settings/user-profile/apps)に進みます。
3. **新しいアプリを作成**をクリックします。
4. アプリ作成時に**期限のないアクセストークン**オプションを選択します（[OAuth トークンについて詳しくはコチラをご覧ください](https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens)）。
5. 必要な OAuth スコープを有効にします：
   - `auditlogs:read` は監査ログコネクターのため。
   - `contentlogs:export` はコンテンツログコネクターのため（Enterprise Guard が必要です）。
6. **アプリをインストールして OAuth トークンを取得する** をクリックします。
7. **アクセストークン** をコピーし、安全に保管します。

OAuth の詳しいセットアップ方法については、[OAuth のはじめ方](https://developers.miro.com/docs/getting-started-with-oauth)をご覧ください。

#### ステップ 2：コンテンツログ専用オーガニゼーションIDの取得

1. [Miro の会社設定](https://miro.com/app/settings/)に移動します。
2. ブラウザのURLを確認し、組織IDを見つけます:
   - URLの形式は次の通りです: `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`。
   - URLから組織ID（数値）をコピーします。

### Microsoft Sentinelでソリューションを展開する

1. Microsoft Sentinel で、**コンテンツ ハブ**に移動します。
2. **「Miro」**を検索し、ソリューションをクリックします。
3. **インストール**をクリックし、展開ウィザードに従います。
4. Log Analytics ワークスペースを選択します。
5. インストールを完了します。

### データ コネクタの設定

#### Miro 監査ログ コネクタ

1. Microsoft Sentinel で**データ コネクタ**に移動します。
2. **Miro 監査ログ (Enterprise プラン)**を見つけて**コネクタページを開く**をクリックします。
3. **接続**をクリックします。
4. **アクセストークン**を入力します。
5. コネクタを有効にするために**接続**をクリックします。

#### Miro コンテンツ ログ コネクタ

1. Microsoft Sentinel で、**データコネクター** に移動します。
2. **Miro Content Logs (Enterprise Plan + Enterprise Guard)** を見つけ、**コネクターページを開く** をクリックします。
3. **接続** をクリックします。
4. **組織ID** を入力します。
5. **アクセス トークン** を入力します。
6. **接続** をクリックしてコネクターを有効化します。

データの取り込みはコネクターの有効化後、5～10分以内に開始します。

## データテーブル

### MiroAuditLogs_CL

組織レベルの監査イベントには以下が含まれます：

- ユーザー認証とアクセス。
- コンテンツオペレーション。
- チームと組織の変更。
- ユーザープロフィールの変更。
- 管理操作。

**主要列**

| カラム | 説明 |
| --- | --- |
| `TimeGenerated` | イベントのタイムスタンプ。 |
| `event` | 特定のアクションや活動を識別するイベント名。 |
| `logType` | ログエントリのタイプ。 |
| `category` | 関連するイベントをグループ化するイベントカテゴリ。 |
| `createdBy_email` | イベントを引き起こしたユーザー。 |
| `context_ip` | イベントのIPアドレス。 |
| `details` | イベント固有の追加情報（JSON）。 |

### MiroContentLogs_CL

コンテンツレベルの活動ログには以下が含まれます：

- ユーザーの関連情報やタイムスタンプを含むアイテムレベルの操作。
- 状態の遷移と変更。
- コンプライアンスおよびeDiscoveryのための活動追跡。

**主要なカラム**

| カラム | 説明 |
| --- | --- |
| `TimeGenerated` | イベントのタイムスタンプ。 |
| `actionType` | コンテンツに対して実行されたアクションの種類。 |
| `actor_email` | アクションを実行したユーザー。 |
| `itemType` | 対象コンテンツアイテムの種類。 |
| `contentId` | コンテンツの一意の識別子。 |
| `state` | アイテムの状態情報（JSON）。 |

## サンプルクエリ

### 最近の監査イベントを閲覧

```
MiroAuditLogs_CL
| sort by TimeGenerated desc
| project TimeGenerated, event, category, createdBy_email, context_ip
| take 20
```

### ユーザーとイベントタイプによるアクティビティ

```
MiroAuditLogs_CL
| summarize EventCount = count() by createdBy_email, event, category
| order by EventCount desc
```

### ユーザーによるコンテンツの変更

```
MiroContentLogs_CL
| where TimeGenerated > ago(7d)
| summarize Changes = count() by actor_email, actionType
| order by Changes desc
```

### 時間におけるイベントの傾向

```
MiroAuditLogs_CL
| summarize count() by event, bin(TimeGenerated, 1h)
| render timechart
```

### 最もアクティブなユーザー（コンテンツ変更）

```
MiroContentLogs_CL
| where TimeGenerated > ago(30d)
| summarize TotalActions = count() by actor_email
| top 10 by TotalActions desc
```

## トラブルシューティング

### データが表示されない

- アクセストークンが有効で、正しいスコープを持っていることを確認してください。
- コンテンツログの場合、組織にEnterprise Guardアドオンがあることを確認してください。
- 組織IDが正しいことを確認してください（コンテンツログの場合）。
- 初回のデータ取り込みには5～10分かかることがあります。
- **データコネクタ** ページでコネクタのステータスを確認してください。

### 認証エラー

#### オプション 1 を使用している場合（Enterprise インテグレーションのトグル）

- [Miro の会社設定](https://miro.com/app/settings/)に移動し、**アプリとインテグレーション**を展開し、**Enterprise インテグレーション**をクリックします。
- トグル（監査ログのための SIEM、コンテンツログのための eDiscovery）がまだ有効化されていることを確認します。
- 他の管理者がトグルを無効化した場合、そのトークンは無効になります。
- 新しいトークンを生成し、コネクタ設定を更新するためにトグルを再度有効化します。
- Miro で会社の管理者の役割を持っていることを確認します。

#### オプション 2 (カスタム OAuth アプリ) を使用する場合

- [Miro アプリ設定](https://miro.com/app/settings/user-profile/apps)でトークンが無効になっていないことを確認します。
- OAuth アプリケーションに必要なスコープが有効であることを確認します。
- 必要に応じてトークンを再生成し、コネクタ設定に更新します。
- あなたが Miro の会社の管理者の役割を持っていることを確認します。

### コンテンツログが動作していない

- Miro プランに **Enterprise Guard** アドオンが含まれていることを確認してください（ベースとなる Enterprise プランには含まれていません）。
- OAuth スコープ `contentlogs:export` が有効になっていることを確認してください。
- 組織 ID が正しいことを再確認してください。
- Enterprise Guard へのアップグレードが必要な場合は、Miro アカウントマネージャーにお問い合わせください。

## リソース

### Miro ヘルプセンターのリソース

- **Miro 監査ログ:** `../security-integrations/security-management/01-audit-logs.md
- **Miro コンテンツログ:** `../canvas-25-admin-features/ediscovery/06-content-logs-overview.md
- **Miro Sentinel インテグレーションガイド:** `01-microsoft-sentinel-integration.md`。

### Miro 開発者ドキュメント

- **Enterprise API 入門:** `https://developers.miro.com/docs/getting-started-with-enterprise-api`.
- **OAuth 入門:** `https://developers.miro.com/docs/getting-started-with-oauth`.
- **OAuth トークン認証:** `https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens`.
- **監査ログ API:** `https://developers.miro.com/reference/enterprise-get-audit-logs`.
- **コンテンツログ API:** `https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch`.
- **API リファレンス:** `https://developers.miro.com/reference`.

### Microsoft Sentinel

- **Microsoft Sentinel のドキュメント:** `https://docs.microsoft.com/azure/sentinel/`.
