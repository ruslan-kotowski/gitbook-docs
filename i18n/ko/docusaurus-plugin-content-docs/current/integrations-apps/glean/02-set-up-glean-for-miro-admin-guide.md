---
title: 미로용 글린 설정 (관리자 가이드)
article_id: 27581463837330
translation_id: 27581463837330
locale: ko-kr
sidebar_position: 2
created_at: '2025-06-23T10:52:57Z'
updated_at: '2026-01-02T09:57:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: '대상: 회사 관리자 플랜: Business, Enterprise 플랫폼: 데스크톱, 브라우저'
---

회사 관리자로서 조직에 Glean 통합을 설치하고 구성할 수 있습니다. 이를 통해 Glean의 AI 기반 검색 기능을 Miro에 직접 연결하여 팀이 100개 이상의 소스 시스템에서 정보를 찾아 생산성을 향상시킬 수 있습니다.

## 전제 조건

1. 당신은 **Miro 조직 관리자**이며 **Glean 관리자**입니다.
2. Glean에서 **OAuth 클라이언트 ID를 등록**합니다. 자세한 내용은 [Glean 문서](https://developers.glean.com/api-info/client/authentication/oauth)를 참조하세요.
3. 사용자 레벨 개인 정보 설정에서 **채팅 기록을 최대 30일 동안 저장 허용**을 활성화합니다.

## Glean 앱 설치

시작하려면 Miro 마켓플레이스에서 조직의 관련 팀에 Glean 앱을 설치합니다.

1. 회사 **설정**으로 이동하여 **앱 및 통합**을 클릭합니다.
2. **앱** 탭에서 **앱 추가**를 클릭하여 마켓플레이스를 엽니다.
3. "Glean"을 검색합니다. 검색창에 클라이언트 ID인 `1202342442818548396`을 붙여넣어 찾을 수도 있습니다.
4. 앱 프로필에서 앱을 추가할 곳을 선택합니다: **모든 팀** 또는 **특정 팀 선택...**.
5. 권한 페이지를 확인합니다. Glean 앱은 Miro에서 개발 및 유지 관리되며, 특정 권한이 필요하지 않습니다.
6. **추가**를 선택하여 설치를 완료합니다.

## SSO(통합로그인) 설정 (Okta)

귀사의 조직이 SSO(통합로그인) 제공자로 Okta를 사용하는 경우, 다음 단계로 진행하기 전에 Okta OpenID Connect (OIDC) 웹 애플리케이션을 생성해야 합니다.

1. 여기에 나와 있는 설명서를 참조하여 새로운 Okta 앱을 생성하세요 [여기](https://help.okta.com/en-us/content/topics/apps/apps_app_integration_wizard_oidc.htm)를 클릭하세요.
   1. **OIDC - OpenID Connect**를 로그인 방법으로 선택합니다.
   2. **웹 애플리케이션**을 애플리케이션 유형으로 선택합니다.
   3. **Grant type** > **Core grants** 설정에서 **리프레시 토큰**이 활성화되어 있는지 확인합니다.
   4. `https://integrations.miro.com/api/external-auth/oauth2/callback`을(를) **로그인 리디렉트 URI**로 추가합니다.
   5. **저장**을 선택합니다.
2. **ClientId**와 **Client Secret**을 클라이언트 자격 증명 섹션에서 복사하세요. 이는 통합 설정을 완료하는 다음 섹션에서 필요합니다.

## SSO(통합로그인) 구성

앱을 구성하려면 다음 단계를 따르세요:

1. **앱 및 통합** 페이지에서 **앱 관리하기**로 이동합니다.
2. 설치된 앱 목록에서 "Glean"을 찾아 **설정**을 클릭합니다. 앱이 보이지 않으면 클라이언트 ID (`1202342442818548396`)로 검색한 후 먼저 승인을 요청하세요.
Azure3. **저장**을 클릭해 구성을 적용합니다.

:::note
Azure를 사용하는 경우, Microsoft Entra 관리자 센터에서 Glean 앱에 대해 "조직을 대신하여 동의"를 선택해 사용자가 올바르게 인증할 수 있도록 하십시오.
:::

## Glean 관리자 콘솔 구성

Miro에서 Glean을 사용하기 전에 Glean 관리자 콘솔에서 OAuth 토큰 기반 접근을 구성해야 합니다.

1. **Glean 관리자 콘솔**을 열고 **설정** > **서드파티 액세스 (OAuth)**로 이동합니다.
2. **IDP 설정 OAuth** 섹션에서 **API 액세스를 위한 IDP OAuth 활성화**를 사용하도록 설정합니다.
3. **설정 관리**를 클릭하고, **SSO 공급자**를 선택합니다.
4. SSO 제공자에 따라 제공자 세부 정보를 입력하세요.
   - **Okta**
     - 인증 서버 URL: `https://<subdomain>.okta.com`
     - 허용된 클라이언트 ID(s): 앞 단락에서 생성한 Okta 앱의 클라이언트 ID입니다.
     - 나머지 양식 필드는 비워 둘 수 있습니다.
   - **Azure**
     - 발급자 하위 도메인: `https://login.microsoftonline.com/<tenant-id>/v2.0`
     - 허용된 클라이언트 ID: `a49fdb25-3b5f-4d3b-bedf-6da7be2b4bf4`
   - **GSuite**
     - 허용된 클라이언트 ID: `1062019541050-pf2ndc9f3o4lrmkupj3cj0fep5hkecns.apps.googleusercontent.com`
5. **저장**을 선택하여 설정을 적용하세요.

> ⏰ **참고:** 변경 사항이 Glean 관리자 콘솔에 반영되기까지 최대 30분이 소요될 수 있습니다.

## Glean 앱 사용하기

앱을 설치하고 구성하면, 지정된 팀의 사용자들이 사용을 시작할 수 있습니다. 사용자가 Miro에서 Glean 앱을 처음 열 때, 인증을 프롬프트 받게 됩니다.

1. Miro 보드를 열고 툴바에서 Glean 아이콘을 클릭해 측면 패널을 엽니다.
2. **Glean 연결**을 클릭해 인증을 시작합니다.
3. SSO(통합로그인) 인증 대화 상자가 나타납니다.
4. 인증이 성공하면, Glean 유저 인터페이스가 나타나 사용 준비가 완료됩니다.

## 보안

데이터 및 보안에 대한 자세한 내용은 이 [보안 문서](https://docs.google.com/document/d/1lGLF7eASQb2uMRmMEAaH-GzFhyz4UKfwMeqSQOSYPdM/edit?tab=t.0#heading=h.gu9ng058yy7y)를 참조하세요.
