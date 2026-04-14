---
title: "Jira \uCE74\uB4DC\uC5D0 \uB300\uD55C \uC0C1\uD638 TLS"
article_id: 4410562720658
translation_id: 33416499594002
locale: ko-kr
sidebar_position: 15
created_at: '2026-02-18T08:51:54Z'
updated_at: '2026-03-27T16:18:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  plans: Jira on-premise (Server / Data Center)
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

> **사용 가능 환경:** Enterprise 플랜
>
> **사용 가능 대상:** Jira 온프레미스 (서버/데이터 센터)

양방향 전송 계층 보안(MTLS)은 Jira 인스턴스와 Miro 간의 더욱 안전한 연결을 가능하게 합니다. 이 기능은 모든 Enterprise 플랜에 자동으로 지원되며 *Miro 측에서는 별도의 설정이 필요하지 않습니다.*

:::warning
이 문서는 자세한 지침이 아닌 *샘플 설정과 당사 인증서* (문서의 마지막 부분)에 대해 설명합니다. 네트워크 인프라에 따라 설정 단계가 다를 수 있으므로 반드시 IT 팀 및 시스템 관리자와 상의하시기 바랍니다.
:::

## 구성 방법

검증 방법에는 두 가지가 있습니다:

- 인증서를 통한 방법
- 인증서 지문을 통한 방법

원하는 방법을 선택하고 아래 제공된 스니펫을 사용하여 가지고 있는 NGINX 구성을 조정하세요. [127.0.0.1](http://127.0.0.1/jira/plugins/servlet/oauth/authorize)을 자신의 Jira 인스턴스 IP 또는 웹 주소로 변경하고, ENTER_MIRO_CERTIFICATE_HERE 대신 우리의 인증서 값을 입력하세요.

### 인증서로 검증하기

아래는 NGINX 구성 예입니다:

```
ssl_verify_client optional; ssl_verify_depth 3; set $cert_old "ENTER_OLD_MIRO_CERTIFICATE_HERE"; set $cert_new "ENTER_NEW_MIRO_CERTIFICATE_HERE"; set $valid_cert_flag 0; location /jira/plugins/servlet/oauth/authorize { proxy_pass http://127.0.0.1/jira/plugins/servlet/oauth/authorize; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; } location /jira/login.jsp { proxy_pass http://127.0.0.1/jira/login.jsp; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; } location /jira { if ($ssl_client_raw_cert ~ $cert_old) { set $valid_cert_flag 1; } if ($ssl_client_raw_cert ~ $cert_new) { set $valid_cert_flag 1; } if ($valid_cert_flag != 1) { return 403 "Invalid certificate\n"; } proxy_pass http://127.0.0.1/jira; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; }
```

### 인증서의 지문을 통해 검증하기

아래에서 NGINX 구성 샘플을 확인하세요:

```
ssl_verify_client optional; ssl_verify_depth 3; set $fingerprint_old "여기에 Miro 인증서의 기존 지문 입력"; set $fingerprint_new "여기에 Miro 인증서의 새로운 지문 입력"; set $valid_fingerprint_flag 0; location /jira/plugins/servlet/oauth/authorize { proxy_pass http://127.0.0.1/jira/plugins/servlet/oauth/authorize; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; } location /jira/login.jsp { proxy_pass http://127.0.0.1/jira/login.jsp; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; } location /jira { if ($ssl_client_fingerprint = $fingerprint_old) { set $valid_fingerprint_flag 1; } if ($ssl_client_fingerprint = $fingerprint_new) { set $valid_fingerprint_flag 1; } if ($valid_fingerprint_flag != 1) { return 403; } proxy_pass http://127.0.0.1/jira; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; }
```

## Miro 인증서

새 인증서 이전 인증서

새 인증서는 2026년 4월 14일부터 2026년 10월 9일까지 유효합니다.

```
-----BEGIN CERTIFICATE----- MIIFyDCCBLCgAwIBAgIQAVWS1YUeVBEU1ZV4SCfiajANBgkqhkiG9w0BAQsFADA8 MQswCQYDVQQGEwJVUzEPMA0GA1UEChMGQW1hem9uMRwwGgYDVQQDExNBbWF6b24g UlNBIDIwNDggTTAxMB4XDTI2MDMyNjAwMDAwMFoXDTI2MTAwOTIzNTk1OVowHjEc MBoGA1UEAxMTamlyYS1jYXJkcy5taXJvLmNvbTCCASIwDQYJKoZIhvcNAQEBBQAD ggEPADCCAQoCggEBANI4Mg+7ub8Zr+M0pQSCKPuWemQuFpQWsstj9GIHxliMWqVH NISKliSGbFnIXhGJaJBE/EZSPh2x2jRpbYLnr6eT1zam4Na1G+wNeg++LneZ3KVQ 95BLI6FX/xvduiMCB+3JgtHTk1LujHBggmgoMrrWpcHRv8wZ2m9kk0a5y2HTJU0z MsQTTY7TgH95SM/cMlFtBA3mxWI1DTVETWarHqBnVgxniDwjLqQRVxwTDp8jDuKn M9hdagKlibZFQNN69JUeS7gNs8KW6SfhJiZDJ98lcA/XWLxeouOxcp2n+D2rWPvb o6cB9AtQ25yNsI3dREQp0pzCvuL2yK5qF6VH8SMCAwEAAaOCAuIwggLeMB8GA1Ud IwQYMBaAFIG4DmOKiRIY5fo7O1CVn+blkBOFMB0GA1UdDgQWBBSW/cWH4YEVg69F sUlhePZY92aN0zAeBgNVHREEFzAVghNqaXJhLWNhcmRzLm1pcm8uY29tMBMGA1Ud IAQMMAowCAYGZ4EMAQIBMA4GA1UdDwEB/wQEAwIFoDATBgNVHSUEDDAKBggrBgEF BQcDATA7BgNVHR8ENDAyMDCgLqAshipodHRwOi8vY3JsLnIybTAxLmFtYXpvbnRy dXN0LmNvbS9yMm0wMS5jcmwwdQYIKwYBBQUHAQEEaTBnMC0GCCsGAQUFBzABhiFo dHRwOi8vb2NzcC5yMm0wMS5hbWF6b250cnVzdC5jb20wNgYIKwYBBQUHMAKGKmh0 dHA6Ly9jcnQucjJtMDEuYW1hem9udHJ1c3QuY29tL3IybTAxLmNlcjAMBgNVHRMB Af8EAjAAMIIBfgYKKwYBBAHWeQIEAgSCAW4EggFqAWgAdgDCMX5XRRmjRe5/ON6y kEHrx8IhWiK/f9W1rXaa2Q5SzQAAAZ0p22YpAAAEAwBHMEUCIQDEHNj7+jk+UsK1 5+MSFCiQKG5FuePcorz8C6mXaoa/MQIgR+aYj6T43Y7ORuiHk7yvJoUSDgbiVL8F 9gCbdDVoT1IAdwDYCVU7lE96/8gWGW+UT4WrsPj8XodVJg8V0S5yu0VLFAAAAZ0p 22Y6AAAEAwBIMEYCIQD2TmtQQc+zE6ROJYDLba6TXtHS8mmsv935pNywhJSEOgIh AKZitGkeJaUnoPcy8pByeSqYAg1GryIWdY1ar2Q78dW+AHUAlE5Dh/rswe+B8xkk JqgYZQHH0184AgE/cmd9VTcuGdgAAAGdKdtmOQAABAMARjBEAiAhpDAs0Aq0CRnq abEcTkmtGHDsdWgKl3Y9aP7bE0/zqQIgMncdRSYdeGV40gxKvQY3OV3aSIP/Sqgp qJ1COJiJTzEwDQYJKoZIhvcNAQELBQADggEBAAcm+m2MKdFEip9T1kH4amSOA6Mj blgHWTbEvYcOdhYmssvmiIU5+hdOyUyeYF8OXh2jahUKef+1n/hhzXLr0A4ySDN3 FZE0GbeYwaTIEc1Dnyj8UF9IKcsp8OyujYNK8aA77m7pQe4uWRbfNTisaCd/2kfD d6a6l5J7JvCH4EkMfEDrKHvZatvLDzuiITDQLFhPss4ou9h6F1fMwn/xv/OV39hc d3QP8jClh4h1ghCx0otQgbnCMapcL3qK8dhIMdja7tJzZfh9qE0ZsyF/CepuZCRE a51L8sJNFYZ8esDLH2ZZCM1yx87ls2rpxgT/HxWPtNDUuyxOj2NSQ30Pjj0= -----END CERTIFICATE-----
```

이전 인증서는 2026년 4월 14일까지 유효합니다.

```
-----BEGIN CERTIFICATE----- MIIFBTCCAu2gAwIBAgIUeB+3gSF1xoR9xrCrGoTRXZLYV+EwDQYJKoZIhvcNAQELBQAwEjEQMA4GA1UEAwwHY2FfbWlybzAeFw0yNjAyMTcxNzA2MTRaFw0yNjEyMTQxNzA2MTRaMBIxEDAOBgNVBAMMB2NhX21pcm8wggIiMA0GCSqGSIb3DQEBAQUAA4ICDwAwggIKAoICAQCtRlgo6yypDcTFSE/ODVmHU5lzluceyfj1ByKfxQmkfHtYugN9PQRrDhV66drU5CKAHCI0pVo0PwTYisaMGmkyKK7WqFPdgx/4hQA/Ch97VjMrKY+uVsK7rvuHERFJvX63wGM7F9vJT8t819GTa9rPlBpWO7NPuO4jgIwHXlA/Emfjwu4ZwucLslP7bU9EJNLVnzC7rWCwM0kPXsN9Jwoj4O4PDrOSgRu+LJI8gV4mVrMnE3Qqyd4ZLliI82XsRfpjSMmy/0LqfZ86aXxuBk52wSGtHrK83hyscN5l8PHqs1Ka7CvU/22fGsvlfWbfNxLLgbeNZvH4PaTs5vkzlsmO3/5W28gklGwv9XgXhm1C7dSYCTIfjxzAphlvvoo9m7UAHl3AxHCchJXKqax64e1Hanx+vh2V7k/+E/ULgATUVB+ezUDIoCM7AzJoaTg1wTwwtdfifYdgWxfEzion3QcHqhv3WeyzHCtOx+2xbaL21+6UbtdvTTKbAD1ZkCtPyJ08dr0r32AEY0xpboTOB8r6rRacwSEYm26iidNyZA1ztDUhAMduxT4i4ZKvUlJDOHbrjonHejJGtL1t52FCUDUCC46lyfoFt33N3hBR3hcwP7EPXEhbi5WI3QWF1oqP/yPWbC+l/ynm+pRDsbExx9x9Cd992my+LbxB2AQfacmSJQIDAQABo1MwUTAdBgNVHQ4EFgQU+T1NQVQ4sEkQgucvwAAyv9LzNSswHwYDVR0jBBgwFoAU+T1NQVQ4sEkQgucvwAAyv9LzNSswDwYDVR0TAQH/BAUwAwEB/zANBgkqhkiG9w0BAQsFAAOCAgEADuuVEF51RXb9NVs+19op20Uz/043JbZdoLWFaJJ4jL0XLJwdwsj9G7eTffSRfRdbA0vfqlfss3lreMS9hFxFBCcA58QjwwLARvFZZoyY6iOh3KtSeMnsRzTG3y6hBPeHEZEfRdEdQLR8heAPLqBCpfyfZ2qHPZpDQPiOMg63SSDWynY39zyXIcRXRKS4WAoiujVeSXc7ruTCVdonzrdPJrq9BSqKgv4bu2Wt6XBuXsCKh7fYhQSiWTciyadNoFkDJQsQuQKSLDlD7G3Tv3l+Ihu1GL1oiyhTcVHTCFymB81EGQ0MhHGJqejQ0Kc1AmPn6Cc5XqVW0i0dUCGy3HDujCYlTusT9jijMXlZ25EaceFL7W+Ks5sa2jVRnSzg5mJuNYo9x2SleemuyHsCviDgaL4DDBAELkxThDDi3XP+gY4XkJ+9yNuzoCsiZvhLEttQdA2DG3Iaw8kTtQbdLpUlGPPMUZ/pJv2pSlno8D5LvI4sCFPuz7mPQXQKjbOUd6OFQRk0GLgoPQVgl4Tyjkukf8oGa/WmheIcu1oeJBYcoQbSvjeTwfzurHivIxpDK0GTQ5THbfGhTi64/+TFXSe0URKrHKt2H6gSdwtdV195PVSzKD4EZtAY4m6L2k8AfTULlNVUADD09H36OszfS+Y3oW0cefDsRQdNRfcgD0vGzso= -----END CERTIFICATE-----
```
