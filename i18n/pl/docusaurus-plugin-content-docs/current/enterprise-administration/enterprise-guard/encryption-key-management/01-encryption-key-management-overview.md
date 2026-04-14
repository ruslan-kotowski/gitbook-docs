---
title: "Przegl\u0105d zarz\u0105dzania kluczami szyfrowania"
article_id: 14634334255250
translation_id: 14634334255250
locale: pl-pl
sidebar_position: 0
created_at: '2023-10-24T14:24:53Z'
updated_at: '2026-02-05T15:17:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

Dodatek Enterprise Guard zawiera opcję zarządzania kluczami szyfrowania (EKM). Zarządzanie kluczami szyfrowania zapewnia scentralizowaną kontrolę nad kluczami szyfrowania, aby pomóc w ochronie Twoich danych. To rozwiązanie oparte na chmurze umożliwia monitorowanie dzienników aktywności związanych z kluczami szyfrowania i pozwala na cofnięcie dostępu do kluczy do Twoich danych.

Dla dodatkowej kontroli i wglądu w sposób, w jaki klucze szyfrowania są używane w Miro, możesz również skorzystać z opcji Bring Your Own Key (BYOK). Dzięki BYOK, zarządzasz szyfrowaniem danych swojej organizacji na platformie Miro.

## Poznaj zalety zarządzania kluczami szyfrowania

- **Bezproblemowa implementacja:** Bez wysiłku zintegruj zarządzanie kluczami szyfrowania z Twoim systemem bez potrzeby instalacji czy konserwacji sprzętu, dzięki w 100% chmurowemu rozwiązaniu.

- **Całkowita kontrola dostępu do kluczy:** Ciesz się pełnym zarządzaniem swoimi kluczami szyfrowania. Masz możliwość wycofania klucza, czyniąc wszystkie zaszyfrowane dane niedostępnymi zarówno dla Miro, jak i użytkowników końcowych.

- **Lepsza widoczność dostępu:** Zyskaj wgląd w akcje związane z kluczami dzięki widoczności dostępu. Monitoruj i śledź logi przez AWS CloudTrail, aby w pełni zrozumieć sposób użycia klucza szyfrowania.

![Enterprise Key Management Diagram](images/33084060145042_EKM.png)

## Jak zarządzanie kluczami szyfrowania chroni dane klientów

Miro zapewnia zarządzanie kluczami szyfrowania (EKM), oferując szyfrowanie danych produkcyjnych i kopii zapasowych w stanie spoczynku za pomocą niestandardowego klucza szyfrowania, przy czym klient udziela Miro dostępu do tego klucza. Miro wspiera zarządzanie kluczami szyfrowania z kluczem umieszczonym w Twoim własnym koncie AWS za pośrednictwem AWS KMS. Dzięki zarządzaniu kluczami szyfrowania zyskujesz lepszą widoczność audytów i zwiększoną kontrolę dostępu do danych (treści generowanych przez użytkowników), takich jak kształty, widgety i przesłane pliki.

## Szyfrowanie danych w Miro

Zapewnienie najwyższego poziomu bezpieczeństwa Twoich danych jest priorytetem w Miro. Domyślnie stosujemy środki szyfrowania danych klientów zarówno w trakcie przesyłu, jak i w stanie spoczynku, niezależnie od ich abonamentu. Podczas korzystania z Miro przez internet, Twoje dane są chronione przez szyfrowanie TLS 1.3 i certyfikaty PKI wystawione przez Amazon Web Services (AWS). Po dotarciu do naszych serwerów, Twoje dane są dodatkowo zabezpieczane szyfrowaniem AES-256 w stanie spoczynku, przy użyciu kluczy zarządzanych przez Miro za pośrednictwem AWS Key Management Service (KMS). [Dowiedz się więcej o bezpieczeństwie w Miro.](https://miro.com/trust/security/)

> Uwaga: Jesteś wyłącznie odpowiedzialny za bezpieczeństwo i ochronę wszelkich Danych Kopii Zapasowej pobranych lub przeniesionych przez Ciebie do Twoich systemów lub systemów stron trzecich. Jesteś wyłącznie odpowiedzialny za Twój Niestandardowy Klucz Szyfrowania. Jeśli utracisz swój Niestandardowy Klucz Szyfrowania, Miro nie może Ci pomóc w odzyskaniu dostępu do danych. Gdy Twoje Dane Produkcyjne lub Dane Kopii Zapasowej znajdują się w tranzycie lub poza kontrolą Miro, Miro nie może zagwarantować ich ochrony.

## Jak włączyć Zarządzanie Kluczami Szyfrowania

Konfigurowanie i wdrażanie Zarządzania Kluczami Szyfrowania wymaga pomocy zespołów wewnętrznych Miro. Jeśli potrzebujesz pomocy, skontaktuj się z przedstawicielem Miro lub [poproś o pomoc poprzez zespół pomocy Miro tutaj](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).

## Glosariusz

- **Kopia zapasowa danych:** Zrzut treści utworzony w lub przesłany do usługi Miro, przechowywany przez Miro do celów odzyskiwania i innych.

- **Niestandardowy klucz szyfrowania:**  Unikalny klucz zabezpieczający dostosowany i wdrożony przez Ciebie, który jest wymagany do uzyskania dostępu do Danych roboczych i Kopii zapasowych danych.

- **Dane robocze:** Wszystkie dane, które Ty i Twoi użytkownicy uzyskujecie podczas korzystania i codziennego działania usług Miro.
