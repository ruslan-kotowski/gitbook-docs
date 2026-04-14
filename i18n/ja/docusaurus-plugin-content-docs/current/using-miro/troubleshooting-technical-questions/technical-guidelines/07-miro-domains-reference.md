---
title: "Miro \u30C9\u30E1\u30A4\u30F3 \u30EA\u30D5\u30A1\u30EC\u30F3\u30B9"
article_id: 20857452690706
translation_id: 20857452690706
locale: ja
sidebar_position: 8
created_at: '2024-08-20T08:12:36Z'
updated_at: '2026-03-06T13:37:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

このリファレンス記事には、Miro がその SaaS アプリケーションで使用する各ドメインが一覧表示されています。

:::note
Miro のために開発されたサードパーティー製アプリケーションや Miroverse アプリケーションの中には、Miro が制御していない外部のドメインやサービスに依存しているものがあります。
:::

## グローバル プロダクション ドメイン

保護されたネットワークを使用する組織は、以下のグローバル プロダクション ドメインを許可する必要があります：

```
*.miro.com
注意: 次のような派生ドメインも含みます: *.api.miro.com | *.svc.miro.com
```

```
*.miro-apps.com
```

```
mirostatic.com
```

```
*.mirostatic.com
```

```
onlinewhiteboard.com
```

```
realtimeboard.com
```

```
*.realtimeboard.com
```

```
webwhiteboard.com
```

## プロダクションツール ドメイン

保護されたネットワークを使用する組織は、以下のプロダクションツール ドメインを許可する必要があります：

```
api.stigg.io
注意: Miro AI 機能のために必要です。
```

```
*api.stigg.io
注意: Miro AI 機能のために必要です。
```

```
braze.eu
```

```
*.braze.eu
```

```
browser.sentry-cdn.io
```

```
cdn.cookielaw.org
```

```
fonts.googleapis.com
```

```
fonts.gstatic.com
```

```
miroapp.github.io
```

```
realtimeboardhelp.zendesk.com
```

```
*.sentry.io
```

```
split.io
```

```
*.split.io
```

## 地域別プロダクション ドメイン

保護されたネットワークを使用する組織は、以下の地域別プロダクション ドメインを許可する必要があります。

:::note
グローバル プロダクション ドメイン、およびプロダクション ツーリング ドメインに加えて、オーストラリアやアメリカ合衆国における[データレジデンシー](../../../enterprise-administration/canvas-25-admin-features/data-residency/02-data-residency-at-miro.md)に対応するために地域別プロダクション ドメインも許可する必要があります。
:::

### オーストラリア

```
*.au.miro.com
注: 次のような派生ドメインも含みます：*.api.au.miro.com | *.svc.au.miro.com
```

```
*.au01.miro.com
```

### アメリカ合衆国

```
*.us.miro.com
注: 次のような派生ドメインも含みます：*.api.us.miro.com | *.svc.us.miro.com
```

```
*.us01.miro.com
```
