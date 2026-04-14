---
title: Przewodnik dla administratorów po uwierzytelnianiu dwuskładnikowym (2FA) w
  Enterprise
article_id: 7935391125394
translation_id: 7935391125394
locale: pl-pl
sidebar_position: 1
created_at: '2022-10-04T08:57:18Z'
updated_at: '2026-01-13T13:35:36Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Dotyczy: Enterprise Plan Ustawienia przez: administratorów firmy'
---

## Uwierzytelnianie dwuskładnikowe (2FA) dla organizacji

2FA dodaje dodatkową warstwę zabezpieczeń do profili online, wykraczając poza sam login i hasło. Administratorzy firmy Enterprise mogą wymagać dodatkowego potwierdzenia tożsamości, gdy użytkownicy uzyskują dostęp do subskrypcji Miro swojej organizacji. Ten wymóg dotyczy wszystkich logowań z użyciem e-mail i hasła.

Dla firm używających pojedynczego logowania (SSO) 2FA obejmuje tylko zewnętrznych współpracowników niekorzystających z SSO. Dla firm niekorzystających z SSO, 2FA dotyczy wszystkich użytkowników.

:::note
Ten artykuł wyjaśnia uwierzytelnianie dwuskładnikowe (2FA) dla abonamentu Enterprise. Dla wszystkich innych abonamentów, zobacz [Uwierzytelnianie dwuskładnikowe (2FA)](../../../administration/security-compliance/01-two-factor-authentication-2fa.md) w administracji.
:::

## Jak skonfigurować egzekwowane 2FA dla swojej organizacji

:::note
Przed włączeniem uwierzytelniania dwuskładnikowego (2FA) ważne jest, aby poinformować wszystkich tych użytkowników, których może to dotyczyć, w tym zarówno członków Twojej organizacji, jak i zewnętrznych współpracowników. Aby zapewnić płynne przejście, sugerujemy udostępnienie naszego [przewodnika użytkownika 2FA](../../security-integrations/two-factor-authentication-2fa/02-enterprise-two-factor-authentication-2fa-–-user-guide.md), aby pomóc im w tym procesie.
:::

## Jak włączyć 2FA dla Twoich użytkowników

1. Przejdź do konsoli administracyjnej > **Bezpieczeństwo** > **Uwierzytelnianie**.
2. Włącz **Wymuszaj 2FA u użytkowników, którzy nie logują się przez SSO**.

![2FA-enable.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277317394_2FA-enable.png)*Wymuszanie uwierzytelniania dwuskładnikowego dla użytkowników niekorzystających z SSO*

### Zaufanie do urządzeń używających 2FA

Po włączeniu użytkownikom 2FA będzie pokazywane pole wyboru, które pozwala im na pomijanie uwierzytelniania dwuskładnikowego przy każdym logowaniu na tym urządzeniu przez następne X dni, gdzie „X” to ramka czasowa ustalona przez administratora. Możesz zezwolić na oznaczanie urządzeń jako zaufane na 7 do 90 dni. Domyślnie zaufanie do urządzeń 2FA jest włączone, choć tę funkcję można wyłączyć w konsoli administracyjnej.

![2FA-trusted-devices.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24790277323410_2FA-trusted-devices.png)

:::warning
Jeśli zaufanie do urządzeń 2FA jest wyłączone, użytkownicy będą musieli wprowadzać kod uwierzytelniania dwuskładnikowego przy każdym logowaniu. To spowolni proces logowania.
:::

Uwierzytelnianie dwuskładnikowe będzie wymagane ponownie po upływie okresu zaufania.

Uwierzytelnianie dwuskładnikowe nie będzie pomijane, jeśli użytkownicy logują się na nowym urządzeniu lub przeglądarce, lub jeśli wyczyszczą pliki cookie przeglądarki.

## Resetowanie 2FA dla użytkowników

Jeśli użytkownik straci dostęp do swojej metody uwierzytelniania dwuskładnikowego, administratorzy mogą jej resetować. Po zgłoszeniu przez użytkownika prośby o resetowanie tej metody, odpowiedni administrator otrzyma powiadomienie e-mail.

:::note
Administratorzy mogą resetować uwierzytelnianie dwuskładnikowe tylko dla użytkowników, których domeny e-mail są zweryfikowane w ich organizacji, jeśli administrator inicjuje reset. Jeśli użytkownik prosi o reset, każdy administrator w organizacji może go zatwierdzić.
:::

Aby zresetować metodę uwierzytelniania dwuskładnikowego dla użytkownika:

1. Przejdź do **Konsola administracyjna** > **Użytkownicy** > karta **Aktywni użytkownicy**.
2. Znajdź użytkownika, któremu trzeba zresetować metodę 2FA.
3. Kliknij ikonę **menu z 3 kropkami** (**...**) w wierszu użytkownika.
   ![reset-2fa.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/24650686629138_reset-2fa.png)
   *Resetowanie uwierzytelniania dwuskładnikowego w konsoli administracyjnej*
4. Kliknij **Resetuj uwierzytelnianie dwuskładnikowe**.
   Pojawi się okno dialogowe z prośbą o potwierdzenie.
5. Kliknij przycisk **Resetuj 2FA** w oknie dialogowym.
6. Na górze ekranu pojawi się wiadomość potwierdzająca, że instrukcje dotyczące resetu zostały wysłane użytkownikowi.

## Wpływ na doświadczenie użytkownika

- Użytkownicy niekorzystający z SSO będą poproszeni o skonfigurowanie drugiego czynnika podczas następnego logowania. Ten proces nie wylogowuje ich z bieżących sesji.
- Użytkownicy muszą skonfigurować uwierzytelnianie dwuskładnikowe przy użyciu urządzenia mobilnego oraz aplikacji generującej jednorazowe hasła czasowe (TOTP), takich jak Microsoft Authenticator, Google Authenticator lub Authy.
- Dla użytkowników korzystających z 2FA istnieje limit 3 prób wprowadzenia poprawnego kodu TOTP. Jeśli ten limit zostanie przekroczony, będą musieli rozpocząć proces uwierzytelniania od początku.
- Logowanie z użyciem 2FA jest dostępne w aplikacjach mobilnych i na tabletach, ale proces początkowej rejestracji jest wspierany wyłącznie w przeglądarkach i aplikacjach stacjonarnych.

## Ważne informacje

Egzekwowanie 2FA dotyczy tylko *użytkowników uwierzytelniających się za pomocą swojego e-maila i hasła lub za pomocą magicznych linków (wysyłanych e-mailem)*.

- 2FA nie jest włączane dla zewnętrznych współpracowników uwierzytelniających się za pomocą SSO.
- Jeśli współpracownik Twojej organizacji Enterprise już uwierzytelnia się za pomocą SSO z organizacji macierzystej, nadal będzie mieć dostęp do wszystkich zespołów i tablic w Miro, używając SSO.
- Gdy użytkownik uwierzytelnia się przez integrację logowania zewnętrznego (np. Google, Microsoft, Slack), będzie utrzymywał dostęp do wszystkich zespołów i tablic Miro poprzez tę metodę logowania. Administratorzy mają możliwość zachęcania tych użytkowników do ustawienia drugiego czynnika w ramach ich odpowiedniej integracji logowania. Jednakże, proces uwierzytelniania Miro nie poprosi tych użytkowników o ustawienie drugiego czynnika.

## Dzienniki audytu

Administratorzy mogą śledzić użytkowników, którzy skonfigurowali uwierzytelnianie dwuskładnikowe, wraz z sukcesami i niepowodzeniami logowania 2FA w poniższych zdarzeniach dziennika audytu:

- `mfa_setup_succeeded` - gdy użytkownik pomyślnie skonfigurował swój drugi czynnik
- Aktualizacja wydarzenia `sign_in_succeeded`, aby uwzględnić atrybut MfaFactorType, jeśli logowanie z uwierzytelnieniem dwuskładnikowym zakończyło się sukcesem
- Aktualizacja wydarzenia `sign_in_failed`, aby uwzględnić atrybut MfaFactorType, jeśli logowanie z uwierzytelnieniem dwuskładnikowym było nieudane z powodu przekroczenia maksymalnej liczby prób (przyczyna nietechniczna)
