---
title: Jira on-premise z autoryzacją stron trzecich za pomocą odniesienia do OAuth
  2.0
article_id: 26726425696530
translation_id: 26751139657746
locale: pl-pl
sidebar_position: 11
created_at: '2025-05-16T09:09:04Z'
updated_at: '2025-11-25T15:51:19Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Kto może to zrobić: Administratorzy firmy Które abonamenty: Enterprise'
---

Ten artykuł zawiera szczegółowe informacje techniczne dotyczące używania zewnętrznego serwera autoryzacji z OAuth 2.0 do integracji Jira z Miro.

Aby dowiedzieć się, jak skonfigurować połączenie, zobacz [Łączenie z Jira on-premise z użyciem serwerów autoryzacji innych firm za pomocą OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Jak działa integracja Jiry z Miro z wykorzystaniem autoryzacji on-premise i OAuth 2.0

Poniższy wykres pokazuje przepływ komunikacji między Miro a lokalnym serwerem autoryzacji Jira.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Integracja Miro i Jira przy użyciu lokalnego serwera autoryzacji przez bramę API*

## Parametry konfiguracji

Aby skonfigurować przepływ autoryzacji pomiędzy Miro a Jira za pomocą zewnętrznego serwera autoryzacji z OAuth 2.0, musisz określić następujące parametry:

- **Serwer autoryzacji**
  - Prośba o URL autoryzacji
  - URL żądania tokenu
  - Zakres
- **Konfiguracja aplikacji autoryzacyjnej**
  - ID klienta
  - Sekret klienta
- **Instancja Jira**
  - Publiczny URL Jira
  - Podstawowy adres URL Jira; wewnętrzny adres URL

> Miro dostarcza adres URL przekierowania, który serwer autoryzacji sprawdza w odniesieniu do zarejestrowanej aplikacji.

**Więcej informacji:** Zobacz [Połączenie z Jira on-premise przy użyciu serwerów autoryzacji zewnętrznego dostawcy z OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Prośby autoryzacji użytkownika między Miro a lokalnym serwerem autoryzacji

W przypadku integracji między Miro i Jira za pomocą zewnętrznego serwera autoryzacji, poniższy wykres przedstawia przepływ prośby użytkownika o autoryzację.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Prośba o autoryzację użytkownika*

### Prośba o autoryzację

```
https://{authorization_URL}?
    response_type=code&
    client_id={CLIENT_ID}&
    redirect_uri={Adres przekierowania Miro}&
    scope={scope}&
    state={{state}}
```

Użytkownik może dodać parametry do prośby autoryzacyjnej jako pary klucz-wartość w konfiguracji.

### Prośba o token

```
curl --polecenie POST \
    --url '{token request URL}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=authorization_code \
    --data 'client_id={CLIENT_ID}' \
    --data 'client_secret={CLIENT_SECRET}' \
    --data 'code={Otrzymany kod autoryzacji}' \
    --data 'przekieruj_uri={Miro Redirect URI}' \
```

Po otrzymaniu kodu autoryzacji, Miro zapewnia stan i prosi o parę tokenów.

### Odśwież wymianę tokenów

```
curl --request POST \
    --url '{token prośby URL}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=refresh_token \
    --data 'client_id={CLIENT_ID}' \
    --data 'refresh_token={obecny ważny token odświeżania}' \
```

Upewnij się, że operacja tokenu odświeżania jest włączona; włącz dostęp offline do API.

### Żądania API Jira

```
curl --request GET \
    --url {Jira Public URL}/rest/api/{apiversion}/... \backslash
    --header 'autoryzacja: Okaziciel {accessToken}' \
    --header 'content-type: application/json'
```

Każda prośba używa podanego publicznego adresu URL Jira jako podstawowego adresu URL oraz tokenu dostępu użytkownika jako tokenu okaziciela.
