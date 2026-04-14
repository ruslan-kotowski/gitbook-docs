---
title: Uwierzytelnianie dwuskładnikowe (2FA)
article_id: 27356474050834
translation_id: 27356474050834
locale: pl-pl
sidebar_position: 1
created_at: '2025-06-12T12:01:03Z'
updated_at: '2025-06-24T08:19:34Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: 'Kto może to zrobić: Administratorzy zespołu, administratorzy firmy Jakie
    wersje: Starter, Business, Education, Enterprise Na których platformach: Przeglądarka,
    Aplikacja komputerowa, Urządzenia mobilne'
---

Uwierzytelnianie dwuskładnikowe (2FA) dodaje dodatkową warstwę bezpieczeństwa do kont online, wymagając od użytkowników podania dwóch unikalnych metod weryfikacji przed uzyskaniem dostępu do ich kont.

Administratorzy Miro mogą włączyć 2FA dla swoich zespołów i zresetować 2FA dla członków zespołu. Użytkownicy mają możliwość zaufania urządzeniu na 30 dni.

:::note
Ten artykuł wyjaśnia 2FA dla abonamentów Starter, Business i Education. Aby dowiedzieć się więcej o 2FA dla Enterprise, zobacz [Uwierzytelnianie dwuskładnikowe (2FA) (przewodnik dla administratora).](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md)
:::

## Włącz uwierzytelnianie dwuskładnikowe (2FA)

W wersjach Starter i Education upewnij się, że masz rolę administratora zespołu.

W przypadku abonamentu Business upewnij się, że masz rolę administratora firmy.

Wykonaj następujące kroki:

1. Na pulpicie nawigacyjnym Miro kliknij swój awatar w prawym górnym rogu i wybierz **Konsolę administratora**.
2. (Starter) Przejdź do **Bezpieczeństwo** > **Uprawnienia**.
   (Education) Przejdź do **Uprawnienia**.
   Przejdź do **Bezpieczeństwo** > **Uwierzytelnianie**.
3. W sekcji **Uwierzytelnianie dwuskładnikowe (2FA)**, przełącz **Wymagaj uwierzytelniania dwuskładnikowego podczas logowania** na pozycję włączoną.

## Konfigurowanie uwierzytelniania dwuskładnikowego (2FA) dla użytkowników

Dla zespołów, które mają włączone uwierzytelnianie dwuskładnikowe (2FA), użytkownicy muszą się uwierzytelnić za pomocą aplikacji uwierzytelniającej, oprócz użycia adresu e-mail i hasła.

Aby dowiedzieć się, jak skonfigurować 2FA jako użytkownik, zobacz [Uwierzytelnianie dwuskładnikowe (2FA) – przewodnik użytkownika](02-two-factor-authentication-2fa-–-user-guide.md).

## Zaufane urządzenia

Użytkownik logujący się do Miro za pomocą 2FA może zdecydować się na zaufanie swojemu urządzeniu.

Podczas logowania za pomocą zaufanego urządzenia użytkownik zostanie poproszony jedynie o uwierzytelnienie pierwszym czynnikiem, pomijając drugi, ponieważ urządzenie jest zaufane.

![](../../../../../../docs/administration/security-compliance/images/27358547112978_image.png)

*Zaufane urządzenie dla 2FA jest domyślnie włączone.*

Przy logowaniu opcja **Ufaj temu urządzeniu przez 30 dni** jest domyślnie zaznaczona, ale użytkownik może ją opcjonalnie odznaczyć.

:::note
Okres urządzenia zaufanego można modyfikować tylko w ramach wersji Enterprise. Aby uzyskać więcej informacji, zobacz [Uwierzytelnianie dwuskładnikowe (2FA) (przewodnik dla administratora)](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).
:::

Aby przestać ufać urządzeniu, któremu przypadkowo udzielono zaufania, użytkownik może się wszędzie wylogować. Przejdź do **profilu**, w sekcji **Ustawienia profilu** kliknij **Wyloguj się ze wszystkich urządzeń**.

## Zresetuj uwierzytelnianie dwuskładnikowe (2FA)

Jeśli użytkownik straci dostęp do swojego drugiego składnika, może poprosić administratora o zresetowanie jego 2FA.

Aby zresetować 2FA dla użytkowników w wersjach Starter i Education, upewnij się, że masz rolę administratora zespołu.

Aby zresetować 2FA dla użytkowników w wersji Business, upewnij się, że masz rolę administratora firmy.

Wykonaj następujące kroki:

1. Z pulpitu Miro kliknij swój awatar w prawym górnym rogu i wybierz **Konsola administratora**.
2. Przejdź do **Użytkownicy**>**Wszyscy użytkownicy**.
3. Zlokalizuj użytkownika, a następnie wybierz menu z 3 kropkami (**...**) na końcu wiersza.
4. Kliknij **Zresetuj uwierzytelnianie dwuskładnikowe**.
   Użytkownik otrzymuje instrukcje dotyczące resetowania na e-mail.
