---
title: AWS コスト計算アプリ
article_id: 15223376381074
translation_id: 15223376381074
locale: ja
sidebar_position: 1
created_at: '2023-11-21T10:05:53Z'
updated_at: '2026-02-18T12:27:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: aws-cost-calculator
availability:
  notes: '対象: Business, Enterprise（アドバンスト ライセンス）'
---

AWS コスト計算アプリは、Miro ボード上で直接 AWS サービスのコストを簡単に見積もるためのシンプルな方法を提供します。これは、プロジェクト マネージャーや IT 担当者に特に有用であり、効率的なプランニングのためにコスト見積もりを合理化します。

:::note
(Enterprise) AWS コスト計算アプリは、アドバンスト ライセンスでのみ利用可能です。詳細については、[Enterprise ライセンスについて](../../plans-billing/miro-plans/05-understanding-enterprise-licenses.md)をご覧ください。
:::

AWS コスト計算アプリは、以下の AWS サービスからのアイコンをサポートしています:

1. ALB
2. APIGateway
3. AS2
4. Athena
5. CertificateAuthority
6. クラシックロードバランサー
7. CloudFront
8. CloudWatch
9. CodePipeline
10. データファイヤーハウス
11. DynamoDB
12. EBS
13. EC2
14. ECR
15. EFS
16. EKS
17. Elb
18. EventBridge
19. Fargate
20. FileCache
21. FTP
22. FTPS
23. GLB
24. Glueクローラー
25. Glueデータブリューインタラクティブセッション
26. Glueデータカタログストレージ要求
27. GlueETLForRayJobsとインタラクティブセッション
28. GlueETLジョブとインタラクティブセッション
29. IAM
30. Kafka
31. Kinesisデータストリーム
32. Lambda
33. NATゲートウェイ
34. NLB
35. RDS
36. Redshift
37. Route53
38. S3
39. SageMaker
40. SecretManager
41. Ses
42. SFTP
43. SNS
44. SQS
45. StepFunctions
46. StepFunctionsExpressWorkFlow
47. TransitGateway
48. VpcCloudWan
49. VpcNetworkAccessAnalyzer
50. VpcPrivateLink
51. VpcReachabilityAnalyzer
52. VpcTrafficMirroring
53. VPNConnection
54. Waf

## AWS コスト計算アプリの設定と使用方法

1. [Miro マーケットプレイス](https://miro.com/marketplace/aws-cost-calculator/)から AWS コスト計算アプリをインストールします。
2. AWS コストを計算したい Miro ボードを開きます。
3. [作成](../../getting-started/start-here/your-first-board/05-toolbars.md)ツールバーの**ツール、メディア、インテグレーション** (**+**) をクリックし、「AWS コスト計算アプリ」を検索します。
4. **AWS コスト計算アプリ**を選択します。ボードの左側に AWS コスト計算アプリ パネルが開きます。
5. クリックしてドラッグすると、ダイアグラム内のすべての AWS アイコンが選択されます。コスト計算機能は、ダイアグラム内のすべての AWS アイコンを自動的に入力します。
6. 各 AWS アイコンについて、**編集** をクリックして、リージョンやストレージの種類などの詳細を指定し、その後 **サービスの選択を保存** をクリックします。
7. すべてのアイコンを編集した後、**計算** をクリックすると、AWS コストの合計が表示されます。
8. コストをより詳細に把握するには、上部のタブとドロップダウンメニューを使用して、期間 (**時間**、**月**、**年**) および **リージョン** でコストを絞り込みます。

![aws-cost-calculator.gif](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/21862013565970_aws-cost-calculator.gif)
*AWS サービスコストの計算*

## 正確な計算のためのヒント

- **具体的に**: 詳細な情報があればあるほど、見積もりはより正確になります。
- **定期的な見直し**: AWS の価格は変更される可能性があります。定期的に見積もりをチェックし、更新してください。また、実際のコストは常に AWS に直接確認してください。

## AWS コスト計算アプリ に関するフィードバック

AWS コスト計算アプリ を改善し、よりお役に立つサービスとするため、皆様からのフィードバックをお待ちしています。

1. Miro ボードで**AWS コスト計算アプリ**パネルを開きます。
2. パネルの右下にあるフィードバック アイコンをクリックして、ご利用体験を評価してください。
3. 開いたテキストフィールドに、今後のアップデートで対応してほしい AWS アイコンなどのフィードバックを記載してください。

![Leave-AWS-Cost-Calculator-feedback.png](../../../../../../docs/integrations-apps/amazon-web-services-aws/images/21020254524946_Leave-AWS-Cost-Calculator-feedback.png)
*AWS コスト計算アプリのフィードバックを残す*
