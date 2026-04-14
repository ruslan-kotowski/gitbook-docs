---
title: Uwierzytelnianie dwuskładnikowe (2FA) – przewodnik użytkownika
article_id: 27601422748434
translation_id: 27601422748434
locale: pl-pl
sidebar_position: 2
created_at: '2025-06-24T07:36:23Z'
updated_at: '2025-11-06T13:29:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: 2fa
availability:
  notes: 'Dotyczy: Starter, Business, Education, Enterprise'
---

## Czym jest uwierzytelnianie dwuskładnikowe (2FA)

Uwierzytelnianie dwuskładnikowe (2FA) zwiększa bezpieczeństwo Twoich kont online. Kiedy administrator firmy aktywuje uwierzytelnianie dwuskładnikowe (2FA), każde logowanie do Miro za pomocą Twojego e-maila i hasła będzie uzupełnione o dodatkową warstwę bezpieczeństwa. Ten dodatkowy krok zapewnia lepszą ochronę Twojego konta, wymagając weryfikacji poza standardowymi danymi dostępowymi.

:::tip
Dowiedz się, jak włączyć uwierzytelnianie dwuskładnikowe (2FA) dla swojej organizacji w [planach Enterprise](../../enterprise-administration/security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md) oraz [we wszystkich innych abonamentach](01-two-factor-authentication-2fa.md).
:::

## Jak skonfigurować uwierzytelnianie dwuskładnikowe (2FA)

**Nowi użytkownicy:** Podczas początkowego procesu [rejestracji](https://miro.com/signup/) z użyciem adresu e-mail służbowego, zostaniesz poproszony o włączenie uwierzytelniania dwuskładnikowego (2FA).
**Istniejący użytkownicy:** Przy następnym [logowaniu](https://miro.com/login/), jeśli Twoja organizacja wymaga uwierzytelniania dwuskładnikowego (2FA) i nie korzystasz z pojedynczego logowania (SSO), zostaniesz poproszony o skonfigurowanie 2FA.

1. Pobierz aplikację uwierzytelniającą na swoje urządzenie mobilne. Aplikacje uwierzytelniające, takie jak Google Authenticator, Microsoft Authenticator i Authy, generują jednorazowy kod (TOTP) do bezpiecznego logowania się do Miro. Jeśli potrzebujesz wskazówek, którą aplikację uwierzytelniającą wybrać, zapytaj administratora firmy lub administratora IT.

2. Kliknij **Mam aplikację uwierzytelniającą** na ekranie konfiguracji uwierzytelniania dwuskładnikowego w Miro.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../docs/administration/security-compliance/images/27601397095698_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *Potwierdzenie pobrania aplikacji uwierzytelniającej*
3. Korzystając z aplikacji uwierzytelniającej, masz teraz dwie opcje:


   Zeskanuj kod QR

   1. Otwórz aplikację uwierzytelniającą.
   2. Za pomocą aplikacji zeskanuj kod QR.
   3. Po zeskanowaniu kliknij **Zeskanowałem kod**
      w Miro.

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../docs/administration/security-compliance/images/27601422721298_2FA-setup-step-2-Scan-QR-code.png)*Skanowanie kodu QR*

   Ręczne wprowadzenie kodu Miro

   1. Jeśli nie możesz zeskanować kodu QR, kliknij
      na **Nie możesz zeskanować kodu QR?** w
      Miro.
   2. Następnie Miro poda kod uwierzytelniający.
      **Skopiuj** ten kod.
   3. Otwórz swoją aplikację uwierzytelniającą i wklej skopiowany kod.
   4. Po dodaniu kodu do aplikacji, kliknij na
      **Dodano kod** w Miro.

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../docs/administration/security-compliance/images/27601397098898_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*Kopiowanie kodu Miro, aby wkleić do aplikacji uwierzytelniającej*
4. Aplikacja uwierzytelniająca wygeneruje 6-cyfrowy kod weryfikacyjny. Wprowadź ten kod w Miro i kliknij **Zweryfikuj kod**.

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../docs/administration/security-compliance/images/27601422725906_2FA-setup-step-3-enter-6-digit-code.png)
   *Weryfikacja 6-cyfrowego kodu*
5. Po pomyślnej weryfikacji konta za pomocą 6-cyfrowego kodu, Miro poda kod odzyskiwania. Kliknij **Kopiuj**, aby bezpiecznie zapisać ten kod. Jest to kluczowe, aby posiadać ten kod, ponieważ pozwala on zresetować uwierzytelnianie dwuskładnikowe w przypadku utraty dostępu do aplikacji uwierzytelniającej.

   Aby potwierdzić, że zapisałeś(aś) kod, wybierz **Zaznaczyłam(em), że zapisałem(am) ten kod**, a następnie kliknij **Kontynuuj**, aby zakończyć proces.

   ![Save-2FA-recovery-code.png](../../../../../../docs/administration/security-compliance/images/27601422727314_Save-2FA-recovery-code.png)*Zapisywanie kodu odzyskiwania*

## Logowanie się za pomocą uwierzytelniania dwuskładnikowego (2FA)

Gdy już pomyślnie skonfigurujesz uwierzytelnianie dwuskładnikowe (2FA) dla swojego konta, za każdym razem, gdy będziesz próbować się zalogować, Miro poprosi Cię o wprowadzenie 6-cyfrowego kodu jednorazowego (TOTP) opartego na czasie.

Kod ten jest generowany przez Twoją aplikację uwierzytelniającą i zapewnia dodatkową warstwę bezpieczeństwa dla Twojego konta. Po prostu otwórz swoją aplikację uwierzytelniającą, pobierz aktualny kod i wprowadź go na stronie logowania, aby uzyskać dostęp do swojego konta.

![2fa-user-guide.png](../../../../../../docs/administration/security-compliance/images/27601397105298_2fa-user-guide.png)
*Logowanie do Miro z 2FA*

Masz 3 próby przed koniecznością ponownego rozpoczęcia procesu logowania.

![Too-many-attempts.png](../../../../../../docs/administration/security-compliance/images/27601397107474_Too-many-attempts.png)*Za dużo prób logowania z 2FA*

### Zaufanie dla urządzeń z uwierzytelnianiem dwuskładnikowym (2FA)

Jeśli twój administrator to skonfigurował, możesz wybrać pole wyboru, aby **Zaufaj temu urządzeniu** podczas logowania do swojego konta z 2FA, gdy używasz bezpiecznego urządzenia (nie używaj opcji **Zaufaj temu urządzeniu** podczas logowania z komputera współdzielonego lub publicznie dostępnego). Kiedy to zrobisz, będziesz mógł(a) logować się bez podawania drugiego składnika, aż do upływu określonego czasu. Ten czas jest ustawiany przez twojego administratora na okres od 7 do 90 dni.

![2FA-signin.png](../../../../../../docs/administration/security-compliance/images/27601397108882_2FA-signin.png)

*Czas trwania zaufania do urządzenia jest wyświetlany obok pola wyboru podczas logowania się przy użyciu uwierzytelniania dwuskładnikowego*

Jeśli nie widzisz opcji „Zaufaj temu urządzeniu”, oznacza to, że administrator nie włączył jej dla Twojej organizacji.

W przypadku logowania się na nowym urządzeniu lub po wyczyszczeniu plików cookies na zaufanym urządzeniu, ponowne użycie uwierzytelniania dwuskładnikowego będzie wymagane.

## Jak zresetować uwierzytelnianie dwuskładnikowe (2FA)

Jeśli napotkasz problemy z aplikacją uwierzytelniającą, zgubisz urządzenie lub musisz zresetować 2FA z jakiegokolwiek innego powodu, wykonaj te kroki:

### Mam kod odzyskiwania

1. Kliknij **Zresetuj uwierzytelnianie dwuskładnikowe**.
2. Użyj kodu odzyskiwania zapisanego podczas początkowego konfigurowania 2FA. Przejdziesz przez proces konfiguracji ponownie, aby ponownie skonfigurować aplikację uwierzytelniającą.

![Reset-two-factor-authentication.png](../../../../../../docs/administration/security-compliance/images/27601422733714_Reset-two-factor-authentication.png)*Opcja resetowania uwierzytelniania dwuskładnikowego*

### Nie mam kodu odzyskiwania

Jeśli zgubiłeś kod odzyskiwania lub nie możesz użyć opcji samodzielnego odzyskiwania, musisz poprosić administratora o zresetowanie 2FA.

Administratorzy mogą zresetować uwierzytelnianie dwuskładnikowe tylko dla użytkowników, których domeny e-mail są zweryfikowane w ich organizacji, jeśli admin inicjuje reset. Jeśli użytkownik złoży prośbę o reset, każdy administrator w organizacji może ją zatwierdzić.

1. Kliknij **Poproś administratora o reset**.
   ![2fa-user-reset.png](../../../../../../docs/administration/security-compliance/images/27601397113106_2fa-user-reset.png)
   *Poproś administratora o reset 2FA, jeśli nie masz kodu odzyskiwania*
2. Jeśli należysz do więcej niż jednej organizacji korzystającej z 2FA, musisz wybrać, do którego administratora organizacji chcesz złożyć prośbę.
3. Otrzymasz e-mail z kodem weryfikacyjnym.
4. Wprowadź kod weryfikacyjny.
5. Zostanie wyświetlone potwierdzenie, że prośba została wysłana do wybranego administratora.
6. Gdy administrator zresetuje Twoje uwierzytelnianie dwuskładnikowe, będziesz musiał przejść przez proces konfiguracji 2FA przy następnym logowaniu.

## Często zadawane pytania

Dlaczego muszę skonfigurować 2FA?

Uwierzytelnianie dwuskładnikowe zwiększa bezpieczeństwo Twojej organizacji. Wszyscy użytkownicy spoza SSO muszą korzystać z uwierzytelniania dwuskładnikowego, jeśli ten wymóg jest egzekwowany przez administratora firmy.

Czy muszę używać uwierzytelniania dwuskładnikowego przy każdym logowaniu?

Tak. Po ukończeniu początkowej konfiguracji, musisz używać aplikacji uwierzytelniającej przy każdym logowaniu, aby zapewnić bezpieczeństwo swojego konta.

Próbowałem(a) skonfigurować uwierzytelnianie dwuskładnikowe, ale otrzymałem(am) komunikat o błędzie "Nieprawidłowy kod", mimo że mój kod jest poprawny. Co powinienem(am) zrobić?

Upewnij się, że strefa czasowa, data i godzina na Twoim urządzeniu są poprawnie ustawione. Jeśli problem będzie się powtarzał, spróbuj skonfigurować uwierzytelnianie dwuskładnikowe na innym urządzeniu.

Co zrobić, jeśli przypadkowo zaufałem współdzielonemu urządzeniu?

Jeśli przypadkowo zaufałeś współdzielonemu urządzeniu, musisz usunąć pliki cookie dla Miro na tym urządzeniu. Zrób to w prosty sposób:

1. Kliknij ikonę suwaka po lewej stronie paska adresu w przeglądarce.
2. Kliknij w menu "Pliki cookie i dane witryn".
3. Kliknij "Zarządzaj danymi witryn na urządzeniu".
4. Kliknij ikonę kosza obok każdej wymienionej tam URL, aby usunąć pliki cookie i dane witryn.

Pamiętaj, że po usunięciu danych witryn z urządzenia będziesz musiał ponownie się zalogować używając uwierzytelniania dwuskładnikowego.

Co zrobić, jeśli stracę dostęp do zaufanego urządzenia?

Jeśli stracisz dostęp do zaufanego urządzenia przed wygaśnięciem okresu zaufania, możesz użyć opcji **Wyloguj się ze wszystkich urządzeń**, aby usunąć dostęp na wszystkich zalogowanych urządzeniach (z wyjątkiem urządzenia, z którego obecnie korzystasz). Spowoduje to wylogowanie ze wszystkich innych urządzeń i unieważnienie 2FA na wszystkich zaufanych urządzeniach. Link **Wyloguj się ze wszystkich urządzeń** znajdziesz w Twoich Ustawieniach profilu. Następnie będziesz musiał ponownie przejść proces logowania z użyciem uwierzytelniania dwuskładnikowego na urządzeniach, do których masz dostęp.
