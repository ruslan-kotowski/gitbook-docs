---
title: "\uC554\uD638\uD654 \uD0A4 \uAD00\uB9AC \uC0C1\uD0DC \uBAA8\uB2C8\uD130\uB9C1"
article_id: 31325531757970
translation_id: 31325531757970
locale: ko-kr
sidebar_position: 1
created_at: '2025-11-24T17:59:06Z'
updated_at: '2026-02-04T20:46:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

관리자들은 Miro 관리자 콘솔에서 암호화 키 관리(EKM) 설정 상태를 모니터링하고 추적할 수 있습니다. 이를 통해 키 온보딩 및 암호화 진행 상황에 대한 투명성이 높아져 추가 지원이 필요 없이 정보를 지속적으로 파악할 수 있습니다.

## EKM 상태 확인

1. Miro 관리자 콘솔에서 **Enterprise Guard**로 이동합니다.
2. **암호화 키 관리**를 선택합니다.
3. **상태** 섹션에서 현재 상태 및 메시지를 검토합니다.

## EKM 상태 이해

**상태** 섹션에는 EKM 설정 및 암호화 프로세스 진행 상황이 표시됩니다.

| 상태 | 의미 |
| --- | --- |
| **사용자 지정 키 추가됨** | Miro는 귀하의 사용자 지정 키로 암호화를 설정하고 있습니다. 준비가 완료되면 키가 자동으로 콘텐츠를 암호화하기 시작합니다. |
| **키 활성화 진행 중** | 새로운 콘텐츠는 귀하의 사용자 지정 키로 암호화됩니다. 기존 콘텐츠의 재암호화가 진행 중입니다. |
| **사용자 지정 키 활성** | 모든 콘텐츠가 귀하의 사용자 지정 키로 암호화되었습니다. |
| **기본 키로 전환 중** | Miro는 암호화를 기본 키로 전환하고 있습니다. 귀하의 사용자 지정 키는 제거될 것입니다. |

## 구성된 키 검토

키 섹션에서 EKM에 현재 구성된 키의 식별자를 볼 수 있습니다. Miro가 사용자 지정 키를 관리하는 경우, 키 ARN 대신 알림을 볼 수 있습니다.

- **주 키**

  귀하의 조직 보드, 댓글 및 기타 콘텐츠를 암호화합니다.
- **백업 저장 키**

  보관된 버전과 백업을 암호화합니다.
- **키 ARN**

  키 식별자는 [AWS KMS](https://aws.amazon.com/kms/)에 있습니다. Miro가 사용자 지정 키를 관리하는 경우, 키 ARN 대신 알림을 볼 수 있습니다.

(선택 사항) 키를 변경하려면 (예: 잘못된 키가 표시되거나 기본 암호화로 돌아가고 싶을 경우), 고객 성공 매니저나 [support@miro.com](mailto:support@miro.com)으로 문의하세요.
