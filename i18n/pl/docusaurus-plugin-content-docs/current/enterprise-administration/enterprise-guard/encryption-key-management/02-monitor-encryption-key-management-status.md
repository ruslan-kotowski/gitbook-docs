---
title: "Monitorowanie statusu zarz\u0105dzania kluczami szyfrowania"
article_id: 31325531757970
translation_id: 31325531757970
locale: pl-pl
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

Administratorzy mogą monitorować i śledzić status konfiguracji zarządzania kluczami szyfrowania (EKM) w konsoli administracyjnej Miro. To zapewnia większą przejrzystość procesu wdrażania kluczy i postępu szyfrowania, pomagając Ci być na bieżąco bez potrzeby dodatkowej pomocy.

## Sprawdź status EKM

1. W konsoli administracyjnej Miro przejdź do **Enterprise Guard**.
2. Wybierz **Zarządzanie kluczami szyfrowania**.
3. W sekcji **Status** sprawdź aktualny stan oraz komunikat.

## Zrozum status EKM

Sekcja **Status** pokazuje, na jakim etapie znajdujesz się w procesie konfiguracji i szyfrowania EKM.

| Stan | Co to oznacza |
| --- | --- |
| **Dodano klucze niestandardowe** | Miro konfiguruje szyfrowanie z użyciem Twoich kluczy niestandardowych. Po ich przygotowaniu klucze automatycznie rozpoczną szyfrowanie treści. |
| **Aktywacja klucza w toku** | Nowe treści są szyfrowane za pomocą Twoich kluczy niestandardowych. Proces ponownego szyfrowania istniejących treści trwa. |
| **Klucze niestandardowe są aktywne** | Wszystkie treści są szyfrowane za pomocą Twoich kluczy niestandardowych. |
| **Przełączanie z powrotem na klucze domyślne** | Miro zmienia szyfrowanie na domyślne klucze. Twoje klucze niestandardowe zostaną usunięte. |

## Przejrzyj skonfigurowane klucze

W sekcji Klucze możesz wyświetlić identyfikatory kluczy obecnie skonfigurowanych dla zarządzania kluczami szyfrowania (EKM). Jeśli Miro zarządza Twoimi niestandardowymi kluczami, możesz zobaczyć powiadomienie zamiast ARN klucza.

- **Klucz główny**

  Szyfruje tablice, komentarze i inne treści Twojej organizacji.
- **Klucz kopii zapasowej**

  Szyfruje zarchiwizowane wersje i kopie zapasowe.
- **Klucz ARN**

  Identyfikator klucza w [AWS KMS](https://aws.amazon.com/kms/). Jeśli Miro zarządza Twoimi niestandardowymi kluczami, możesz zobaczyć powiadomienie zamiast ARN klucza.

(Opcjonalnie) Aby wprowadzić zmiany w kluczach (na przykład, jeśli widzisz niepoprawny klucz lub chcesz wrócić do domyślnego szyfrowania), skontaktuj się ze swoim managerem ds. sukcesu klienta lub napisz na adres [support@miro.com](mailto:support@miro.com).
