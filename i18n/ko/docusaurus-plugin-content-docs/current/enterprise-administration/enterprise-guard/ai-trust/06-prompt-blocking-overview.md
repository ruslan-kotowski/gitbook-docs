---
title: "\uD504\uB86C\uD504\uD2B8 \uCC28\uB2E8 \uAC1C\uC694 (\uBCA0\uD0C0)"
article_id: 29332642230546
translation_id: 29332642230546
locale: ko-kr
sidebar_position: 4
created_at: '2025-09-09T07:58:00Z'
updated_at: '2026-01-12T11:23:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

프롬프트 차단 기능은 민감한 콘텐츠 관리자가 사용자들이 민감 정보를 포함한 AI 프롬프트를 제출하는 것을 방지하여, 조직 전체에서 Miro AI에 민감 데이터가 포함되지 않도록 돕습니다. Miro는 사용자가 프롬프트 필드에 입력한 텍스트와 보드에서 추가한 텍스트 기반 콘텐츠를 스캔합니다. 그 콘텐츠가 프롬프트 차단 구성을 통해 선택된 민감도 레이블이나 소스 코드 패턴과 일치하면, Miro는 프롬프트 제출을 차단합니다.

:::note
베타 버전에서는 텍스트 기반 콘텐츠만 지원됩니다.
:::

## 작동 방식

- 조직 레벨에서 차단할 레이블 카테고리를 선택합니다. 변경 사항은 조직 내 모든 사람에게 즉시 적용됩니다.
- 프롬프트에서 민감한 데이터가 감지되면, Miro AI는 사용자의 입력지점에 정책 메시지를 표시하고 프롬프트가 차단되어 Miro AI에 제출될 수 없습니다.
- 프롬프트 차단과 보드 스캔은 다릅니다. 보드 스캔은 보드에서 민감한 콘텐츠를 찾고 보드를 자동으로 분류할 수 있습니다. 프롬프트 차단은 사용자가 Miro AI에 전송하려는 내용을 검토합니다.

## 차단되는 항목

- 개인정보 보호 레이블: SPII, HIPAA, 신원 정보, 금융 번호 등 내장된 모든 개인정보 보호 레이블을 선택할 수 있습니다. 내장된 개인정보 보호 레이블에 대한 자세한 내용은 [민감도 레이블 및 정보 유형 참조](../../canvas-25-admin-features/data-discovery/06-sensitivity-labels-and-infotypes-reference.md)를 참조하세요.
- 코드 스캔: 활성화되면 Miro는 인식된 소스 코드를 포함하는 프롬프트를 차단합니다. 자세한 내용은 [코드 스캔](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md)을 참조하세요.

## 사용자가 보게 되는 일반적인 결과

사용자가 설정된 민감 정보를 포함하는 프롬프트를 입력하면:

- 사용자에게는 귀하의 조직의 정책을 위반할 수 있어 이 콘텐츠를 생성할 수 없다는 메시지가 표시됩니다.
- 프롬프트가 Miro AI에 전송되지 않습니다. 사용자는 프롬프트를 편집한 후 다시 시도할 수 있습니다.

## 코드 스캔

코드 스캔은 인식 가능한 소스 코드가 포함된 AI 프롬프트를 차단합니다. 차단을 유발하려면 최소한 5줄의 코드가 필요합니다.

예:

```
function connect() {

  const token = "example-token";

  fetch("https://api.example.com/health");

  return true;

}
```

## 지원되는 언어

- C
- C#
- C++
- Go
- HTML
- Java
- JavaScript
- JSON
- PHP
- PowerShell
- Python
- Rust
- Shell script
- SQL
- TypeScript
