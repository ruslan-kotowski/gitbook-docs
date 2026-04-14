---
title: TLS Mutuel pour les cartes Jira
article_id: 4410562720658
translation_id: 8643012207122
locale: fr
sidebar_position: 15
created_at: '2022-11-18T15:32:08Z'
updated_at: '2026-03-27T16:18:35Z'
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

> **Disponible sur :** Forfait Enterprise
>
> **Disponible pour :** Jira on-premise (Serveur / Centre de données)

La sécurité de transport mutuel permet d’établir une connexion encore plus sécurisée entre votre instance Jira et Miro. La fonctionnalité est automatiquement prise en charge pour tous les forfaits Enterprise et ne *nécessite aucune configuration du côté de Miro.*

:::warning
Notez que cet article ne propose pas d’instructions détaillées, il fournit simplement *un exemple de configuration et notre certificat* (à la fin de l’article). Veuillez consulter votre équipe informatique et vos administrateurs système, car les étapes de configuration peuvent différer en fonction de votre infrastructure réseau.
:::

## Différentes façons de configurer

Vous pouvez choisir parmi deux options en ce qui concerne la vérification de la validation :

- Via le certificat
- Via l’empreinte du certificat

Choisissez la méthode que vous préférez et ajustez la configuration NGINX que vous avez à l’aide de l’un des snippets suivants. Assurez-vous de remplacer [127.0.0.1](http://127.0.0.1/jira/plugins/servlet/oauth/authorize) par l’adresse IP ou Web de votre instance Jira et de saisir notre certificat à la place de ENTER_MIRO_CERTIFICATE_HERE.

### Validation via le certificat

Voici l’exemple de la configuration NGINX ci-dessous :

```
ssl_verify_client optional; ssl_verify_depth 3; set $cert_old "ENTREZ_ANCIEN_CERTIFICAT_MIRO_ICI"; set $cert_new "ENTREZ_NOUVEAU_CERTIFICAT_MIRO_ICI"; set $valid_cert_flag 0; location /jira/plugins/servlet/oauth/authorize { proxy_pass http://127.0.0.1/jira/plugins/servlet/oauth/authorize; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; } location /jira/login.jsp { proxy_pass http://127.0.0.1/jira/login.jsp; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; } location /jira { if ($ssl_client_raw_cert ~ $cert_old) { set $valid_cert_flag 1; } if ($ssl_client_raw_cert ~ $cert_new) { set $valid_cert_flag 1; } if ($valid_cert_flag != 1) { return 403 "Certificat invalide\n"; } proxy_pass http://127.0.0.1/jira; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; }
```

### Validation via l’empreinte du certificat

Voici l’exemple de la configuration NGINX ci-dessous :

```
ssl_verify_client optional; ssl_verify_depth 3; set $fingerprint_old "ENTRER_L’ANCIENNE_EMPREINTE_DU_CERTIFICAT_DE_MIRO_ICI"; set $fingerprint_new "ENTRER_LA_NOUVELLE_EMPREINTE_DU_CERTIFICAT_DE_MIRO_ICI"; set $valid_fingerprint_flag 0; location /jira/plugins/servlet/oauth/authorize { proxy_pass http://127.0.0.1/jira/plugins/servlet/oauth/authorize; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; } location /jira/login.jsp { proxy_pass http://127.0.0.1/jira/login.jsp; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; } location /jira { if ($ssl_client_fingerprint = $fingerprint_old) { set $valid_fingerprint_flag 1; } if ($ssl_client_fingerprint = $fingerprint_new) { set $valid_fingerprint_flag 1; } if ($valid_fingerprint_flag != 1) { return 403; } proxy_pass http://127.0.0.1/jira; proxy_set_header X-Forwarded-Host $host; proxy_set_header X-Forwarded-Server $host; proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for; client_max_body_size 10M; proxy_redirect off; }
```

## Certificats Miro

Nouveau certificat Ancien certificat

Le nouveau certificat est valable du 14 avril 2026 jusqu’au 9 octobre 2026.

```
-----BEGIN CERTIFICATE----- MIIFyDCCBLCgAwIBAgIQAVWS1YUeVBEU1ZV4SCfiajANBgkqhkiG9w0BAQsFADA8 MQswCQYDVQQGEwJVUzEPMA0GA1UEChMGQW1hem9uMRwwGgYDVQQDExNBbWF6b24g UlNBIDIwNDggTTAxMB4XDTI2MDMyNjAwMDAwMFoXDTI2MTAwOTIzNTk1OVowHjEc MBoGA1UEAxMTamlyYS1jYXJkcy5taXJvLmNvbTCCASIwDQYJKoZIhvcNAQEBBQAD ggEPADCCAQoCggEBANI4Mg+7ub8Zr+M0pQSCKPuWemQuFpQWsstj9GIHxliMWqVH NISKliSGbFnIXhGJaJBE/EZSPh2x2jRpbYLnr6eT1zam4Na1G+wNeg++LneZ3KVQ 95BLI6FX/xvduiMCB+3JgtHTk1LujHBggmgoMrrWpcHRv8wZ2m9kk0a5y2HTJU0z MsQTTY7TgH95SM/cMlFtBA3mxWI1DTVETWarHqBnVgxniDwjLqQRVxwTDp8jDuKn M9hdagKlibZFQNN69JUeS7gNs8KW6SfhJiZDJ98lcA/XWLxeouOxcp2n+D2rWPvb o6cB9AtQ25yNsI3dREQp0pzCvuL2yK5qF6VH8SMCAwEAAaOCAuIwggLeMB8GA1Ud IwQYMBaAFIG4DmOKiRIY5fo7O1CVn+blkBOFMB0GA1UdDgQWBBSW/cWH4YEVg69F sUlhePZY92aN0zAeBgNVHREEFzAVghNqaXJhLWNhcmRzLm1pcm8uY29tMBMGA1Ud IAQMMAowCAYGZ4EMAQIBMA4GA1UdDwEB/wQEAwIFoDATBgNVHSUEDDAKBggrBgEF BQcDATA7BgNVHR8ENDAyMDCgLqAshipodHRwOi8vY3JsLnIybTAxLmFtYXpvbnRy dXN0LmNvbS9yMm0wMS5jcmwwdQYIKwYBBQUHAQEEaTBnMC0GCCsGAQUFBzABhiFo dHRwOi8vb2NzcC5yMm0wMS5hbWF6b250cnVzdC5jb20wNgYIKwYBBQUHMAKGKmh0 dHA6Ly9jcnQucjJtMDEuYW1hem9udHJ1c3QuY29tL3IybTAxLmNlcjAMBgNVHRMB Af8EAjAAMIIBfgYKKwYBBAHWeQIEAgSCAW4EggFqAWgAdgDCMX5XRRmjRe5/ON6y kEHrx8IhWiK/f9W1rXaa2Q5SzQAAAZ0p22YpAAAEAwBHMEUCIQDEHNj7+jk+UsK1 5+MSFCiQKG5FuePcorz8C6mXaoa/MQIgR+aYj6T43Y7ORuiHk7yvJoUSDgbiVL8F 9gCbdDVoT1IAdwDYCVU7lE96/8gWGW+UT4WrsPj8XodVJg8V0S5yu0VLFAAAAZ0p 22Y6AAAEAwBIMEYCIQD2TmtQQc+zE6ROJYDLba6TXtHS8mmsv935pNywhJSEOgIh AKZitGkeJaUnoPcy8pByeSqYAg1GryIWdY1ar2Q78dW+AHUAlE5Dh/rswe+B8xkk JqgYZQHH0184AgE/cmd9VTcuGdgAAAGdKdtmOQAABAMARjBEAiAhpDAs0Aq0CRnq abEcTkmtGHDsdWgKl3Y9aP7bE0/zqQIgMncdRSYdeGV40gxKvQY3OV3aSIP/Sqgp qJ1COJiJTzEwDQYJKoZIhvcNAQELBQADggEBAAcm+m2MKdFEip9T1kH4amSOA6Mj blgHWTbEvYcOdhYmssvmiIU5+hdOyUyeYF8OXh2jahUKef+1n/hhzXLr0A4ySDN3 FZE0GbeYwaTIEc1Dnyj8UF9IKcsp8OyujYNK8aA77m7pQe4uWRbfNTisaCd/2kfD d6a6l5J7JvCH4EkMfEDrKHvZatvLDzuiITDQLFhPss4ou9h6F1fMwn/xv/OV39hc d3QP8jClh4h1ghCx0otQgbnCMapcL3qK8dhIMdja7tJzZfh9qE0ZsyF/CepuZCRE a51L8sJNFYZ8esDLH2ZZCM1yx87ls2rpxgT/HxWPtNDUuyxOj2NSQ30Pjj0= -----END CERTIFICATE-----
```

L’ancien certificat est valable jusqu’au 14 avril 2026.

```
-----BEGIN CERTIFICATE----- MIIFBTCCAu2gAwIBAgIUeB+3gSF1xoR9xrCrGoTRXZLYV+EwDQYJKoZIhvcNAQEL BQAwEjEQMA4GA1UEAwwHY2FfbWlybzAeFw0yNjAyMTcxNzA2MTRaFw0yNjEyMTQx NzA2MTRaMBIxEDAOBgNVBAMMB2NhX21pcm8wggIiMA0GCSqGSIb3DQEBAQUAA4IC DwAwggIKAoICAQCtRlgo6yypDcTFSE/ODVmHU5lzluceyfj1ByKfxQmkfHtYugN9 PQRrDhV66drU5CKAHCI0pVo0PwTYisaMGmkyKK7WqFPdgx/4hQA/Ch97VjMrKY+u VsK7rvuHERFJvX63wGM7F9vJT8t819GTa9rPlBpWO7NPuO4jgIwHXlA/Emfjwu4Z wucLslP7bU9EJNLVnzC7rWCwM0kPXsN9Jwoj4O4PDrOSgRu+LJI8gV4mVrMnE3Qq yd4ZLliI82XsRfpjSMmy/0LqfZ86aXxuBk52wSGtHrK83hyscN5l8PHqs1Ka7CvU /22fGsvlfWbfNxLLgbeNZvH4PaTs5vkzlsmO3/5W28gklGwv9XgXhm1C7dSYCTIf jxzAphlvvoo9m7UAHl3AxHCchJXKqax64e1Hanx+vh2V7k/+E/ULgATUVB+ezUDI oCM7AzJoaTg1wTwwtdfifYdgWxfEzion3QcHqhv3WeyzHCtOx+2xbaL21+6Ubtdv TTKbAD1ZkCtPyJ08dr0r32AEY0xpboTOB8r6rRacwSEYm26iidNyZA1ztDUhAMdu xT4i4ZKvUlJDOHbrjonHejJGtL1t52FCUDUCC46lyfoFt33N3hBR3hcwP7EPXEhb i5WI3QWF1oqP/yPWbC+l/ynm+pRDsbExx9x9Cd992my+LbxB2AQfacmSJQIDAQAB o1MwUTAdBgNVHQ4EFgQU+T1NQVQ4sEkQgucvwAAyv9LzNSswHwYDVR0jBBgwFoAU +T1NQVQ4sEkQgucvwAAyv9LzNSswDwYDVR0TAQH/BAUwAwEB/zANBgkqhkiG9w0B AQsFAAOCAgEADuuVEF51RXb9NVs+19op20Uz/043JbZdoLWFaJJ4jL0XLJwdwsj9 G7eTffSRfRdbA0vfqlfss3lreMS9hFxFBCcA58QjwwLARvFZZoyY6iOh3KtSeMns RzTG3y6hBPeHEZEfRdEdQLR8heAPLqBCpfyfZ2qHPZpDQPiOMg63SSDWynY39zyX IcRXRKS4WAoiujVeSXc7ruTCVdonzrdPJrq9BSqKgv4bu2Wt6XBuXsCKh7fYhQSi WTciyadNoFkDJQsQuQKSLDlD7G3Tv3l+Ihu1GL1oiyhTcVHTCFymB81EGQ0MhHGJ qejQ0Kc1AmPn6Cc5XqVW0i0dUCGy3HDujCYlTusT9jijMXlZ25EaceFL7W+Ks5sa 2jVRnSzg5mJuNYo9x2SleemuyHsCviDgaL4DDBAELkxThDDi3XP+gY4XkJ+9yNuz oCsiZvhLEttQdA2DG3Iaw8kTtQbdLpUlGPPMUZ/pJv2pSlno8D5LvI4sCFPuz7mP QXQKjbOUd6OFQRk0GLgoPQVgl4Tyjkukf8oGa/WmheIcu1oeJBYcoQbSvjeTwfzu rHivIxpDK0GTQ5THbfGhTi64/+TFXSe0URKrHKt2H6gSdwtdV195PVSzKD4EZtAY 4m6L2k8AfTULlNVUADD09H36OszfS+Y3oW0cefDsRQdNRfcgD0vGzso= -----END CERTIFICATE-----
```
