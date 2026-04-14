---
title: Uwierzytelnianie dwuskładnikowe (2FA) dla Enterprise – przewodnik dla użytkowników
article_id: 7935469290002
translation_id: 7935469290002
locale: pl-pl
sidebar_position: 2
created_at: '2022-10-04T09:00:42Z'
updated_at: '2025-11-06T13:50:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Odpowiednie dla: Starter, Business, Education, Enterprise'
---

## Co to jest uwierzytelnianie dwuskładnikowe (2FA)

Uwierzytelnianie dwuskładnikowe (2FA) zwiększa bezpieczeństwo Twoich kont online. Kiedy administrator firmy aktywuje uwierzytelnianie dwuskładnikowe (2FA), każde logowanie do Miro przy użyciu e-maila i hasła będzie uzupełnione o dodatkową warstwę bezpieczeństwa. Ten dodatkowy krok zapewnia lepszą ochronę Twojego konta, wymagając weryfikacji poza zwykłymi danymi logowania.

:::tip
Dowiedz się, jak włączyć uwierzytelnianie dwuskładnikowe (2FA) dla swojej organizacji w [abonamentach Enterprise](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md) oraz [we wszystkich innych abonamentach](../../../administration/security-compliance/01-two-factor-authentication-2fa.md).
:::

## Jak skonfigurować uwierzytelnianie dwuskładnikowe (2FA)

**Nowi użytkownicy:** Podczas wstępnego [rejestrowania się](https://miro.com/signup/) za pomocą firmowego adresu e-mail zostaniesz poproszony o włączenie uwierzytelniania dwuskładnikowego (2FA).
**Istniejący użytkownicy:** Podczas następnego [logowania](https://miro.com/login/), jeśli Twoja organizacja wymaga 2FA i nie korzystasz z pojedynczego logowania (SSO), zostaniesz poproszony o ustawienie 2FA.

1. Pobierz aplikację uwierzytelniającą na swoje urządzenie mobilne. Aplikacje uwierzytelniające, takie jak Google Authenticator, Microsoft Authenticator i Authy, generują jednorazowy kod (TOTP) oparty na czasie na potrzeby bezpiecznego logowania się do Miro. W przypadku pytań o wybór aplikacji, skontaktuj się z administratorem firmy lub administratorem IT.

2. Kliknij **Mam aplikację uwierzytelniającą** na ekranie konfiguracji 2FA w Miro.

   ![2FA-setup-step-1-Confirmation-of-authenticator-app-download.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653633554_2FA-setup-step-1-Confirmation-of-authenticator-app-download.png)
   *Potwierdzenie pobrania aplikacji uwierzytelniającej*
3. Używając aplikacji uwierzytelniającej, masz teraz dwie opcje:


   Zeskanuj kod QR

   1. Otwórz swoją aplikację uwierzytelniającą.
   2. Użyj aplikacji do zeskanowania kodu QR.
   3. Po zeskanowaniu, kliknij **Zeskanowałem kod** w Miro.

      ![2FA-setup-step-2-Scan-QR-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683263122_2FA-setup-step-2-Scan-QR-code.png)*Skanowanie kodu QR*

   Ręczne wprowadzenie kodu Miro

   1. Jeśli nie możesz zeskanować kodu QR, kliknij
      na **Nie możesz zeskanować kodu QR?** w Miro.
   2. Miro następnie zapewni kod uwierzytelniający. **Skopiuj** ten kod.
   3. Otwórz swoją aplikację uwierzytelniającą i wklej skopiowany kod.
   4. Po dodaniu kodu do aplikacji kliknij
      **Dodałem kod** w Miro.

      ![2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653636754_2FA-setup-step-2-copy-code-and-add-to-authenticator-app..png)*Kopiowanie kodu Miro do wklejenia w aplikacji uwierzytelniającej*
4. Aplikacja do uwierzytelniania wygeneruje 6-cyfrowy kod weryfikacyjny. Wprowadź ten kod w Miro i kliknij **Zweryfikuj kod**.

   ![2FA-setup-step-3-enter-6-digit-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017653634706_2FA-setup-step-3-enter-6-digit-code.png)
   *Weryfikacja 6-cyfrowego kodu*
5. Po pomyślnym zweryfikowaniu konta za pomocą 6-cyfrowego kodu, Miro dostarczy kod odzyskiwania. Kliknij **Kopiuj**, aby bezpiecznie zapisać ten kod. Posiadanie tego kodu jest kluczowe, ponieważ pozwala na zresetowanie 2FA w przypadku utraty dostępu do aplikacji uwierzytelniającej.

   Aby potwierdzić zapisanie kodu, wybierz **Zapisałem ten kod**, a następnie kliknij **Kontynuuj**, aby zakończyć proces.

   ![Save-2FA-recovery-code.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683265554_Save-2FA-recovery-code.png)*Zapisywanie kodu odzyskiwania*

## Logowanie z użyciem uwierzytelniania dwuskładnikowego (2FA)

Po pomyślnym skonfigurowaniu uwierzytelniania dwuskładnikowego (2FA) dla swojego konta, za każdym razem, gdy spróbujesz się zalogować, Miro poprosi Cię o wprowadzenie 6-cyfrowego kodu jednorazowego (TOTP) opartego na czasie.

Kod ten jest generowany przez Twoją aplikację uwierzytelniającą i zapewnia dodatkową warstwę bezpieczeństwa dla Twojego konta. Po prostu otwórz swoją aplikację uwierzytelniającą, pobierz bieżący kod i wprowadź go na stronie logowania, aby uzyskać dostęp do konta.

![2fa-user-guide.png](https://help.miro.com/hc/article_attachments/30847475224978)
*Logowanie do Miro z 2FA*

Masz 3 próby, zanim zostaniesz poproszony o ponowne rozpoczęcie procesu logowania.

![Too-many-attempts.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683267346_Too-many-attempts.png)*Zbyt wiele prób logowania za pomocą 2FA*

### Zaufanie urządzeniom uwierzytelnionym za pomocą 2FA

Jeśli Twój administrator to ustawił, możesz zaznaczyć pole wyboru **Zaufaj temu urządzeniu** podczas logowania do konta za pomocą 2FA, korzystając z bezpiecznego urządzenia (nie używaj **Zaufaj temu urządzeniu** przy logowaniu z urządzenia współdzielonego lub publicznego). Po zaznaczeniu tej opcji będziesz mógł się logować bez wprowadzania drugiego etapu uwierzytelnienia, aż do upływu określonego czasu. Ten czas jest ustalany przez administratora i wynosi od 7 do 90 dni.

![2FA-signin.png](https://help.miro.com/hc/article_attachments/30847475229970)

*Czas trwania zaufania do urządzenia jest wyświetlany obok pola wyboru podczas logowania się z uwierzytelnianiem dwuskładnikowym*

Jeśli nie widzisz opcji "Zaufaj temu urządzeniu", oznacza to, że Twój administrator nie włączył jej dla Twojej organizacji.

Jeśli logujesz się z nowego urządzenia — lub po wyczyszczeniu cookies na zaufanym urządzeniu — uwierzytelnianie dwuskładnikowe będzie ponownie wymagane.

## Jak zresetować uwierzytelnianie dwuskładnikowe (2FA)

Jeśli masz problemy z aplikacją uwierzytelniającą, zgubiłeś urządzenie lub musisz zresetować swoje uwierzytelnianie dwuskładnikowe z jakiegokolwiek innego powodu, wykonaj te kroki:

### Mam kod odzyskiwania

1. Kliknij **Zresetuj uwierzytelnianie dwuskładnikowe**.
2. Użyj kodu odzyskiwania zapisanego podczas początkowego ustawiania 2FA. Przejdziesz ponownie przez proces konfiguracji, aby skonfigurować aplikację autoryzującą.

![Reset-two-factor-authentication.png](../../../../../../../docs/enterprise-administration/security-compliance/two-factor-authentication-2fa/images/21017683268114_Reset-two-factor-authentication.png)*Opcja resetowania uwierzytelniania dwuskładnikowego*

### Nie mam kodu odzyskiwania

Jeśli zgubiłeś kod odzyskiwania lub nie możesz skorzystać z samodzielnego odzyskiwania, musisz poprosić o zresetowanie 2FA przez administratora.

Jeśli domena Twojego e-maila nie jest częścią zweryfikowanych domen Twojej organizacji, administrator nie może zainicjować resetowania za Ciebie. Musisz samodzielnie poprosić o reset 2FA — wtedy administrator będzie mógł to zatwierdzić.

Administratorzy mogą resetować uwierzytelnianie dwuskładnikowe tylko dla użytkowników, których domeny e-mailowe są zweryfikowane w ich organizacji, jeśli administrator inicjuje resetowanie. Jeśli użytkownik wystąpi o reset, każdy administrator w organizacji może go zatwierdzić.

Postępuj zgodnie z tymi krokami:

1. Kliknij **Poproś swojego administratora o reset**.
   ![2fa-user-reset.png](https://help.miro.com/hc/article_attachments/30847475235218)
   *Poproś administratora o reset 2FA, jeśli nie masz kodu odzyskiwania*
2. Jeśli należysz do więcej niż jednej organizacji używającej 2FA, będziesz musiał wybrać, do administratora której organizacji chcesz złożyć prośbę.
3. Otrzymasz e-mail z kodem weryfikacyjnym.
4. Podaj kod weryfikacyjny.
5. Zostanie wyświetlone potwierdzenie, że prośba została wysłana do wybranego administratora.
6. Gdy administrator zresetuje Twoje uwierzytelnianie dwuskładnikowe, będziesz musiał przejść proces konfiguracji przy następnym logowaniu.

## Często zadawane pytania

Dlaczego muszę skonfigurować uwierzytelnianie dwuskładnikowe?

Uwierzytelnianie dwuskładnikowe zwiększa bezpieczeństwo Twojej organizacji. Wszyscy użytkownicy niekorzystający z pojedynczego logowania muszą używać uwierzytelniania dwuskładnikowego do logowania, jeśli ten wymóg jest egzekwowany przez administratora firmy.

Czy muszę używać 2FA przy każdym logowaniu?

Tak. Po zakończeniu początkowej konfiguracji musisz korzystać z aplikacji uwierzytelniającej przy każdym logowaniu, aby zapewnić bezpieczeństwo swojego konta.

Próbowałem ustawić 2FA, ale otrzymałem błąd „Nieprawidłowy kod”, chociaż mój kod jest poprawny. Co powinienem zrobić?

Upewnij się, że strefa czasowa, data i czas na Twoim urządzeniu są prawidłowo ustawione. Jeśli problem nadal występuje, spróbuj skonfigurować 2FA na innym urządzeniu.

Co zrobić, jeśli przypadkowo zaufam współdzielonemu urządzeniu?

Jeśli przypadkowo zaufasz współdzielonemu urządzeniu, musisz usunąć pliki cookie dla Miro na tym urządzeniu. Zrobienie tego jest proste:

1. Kliknij ikonę suwaka po lewej stronie paska adresu w przeglądarce.
2. Kliknij w menu "Pliki cookie i dane witryn".
3. Następnie kliknij "Zarządzaj danymi witryn na urządzeniu".
4. Kliknij ikonę kosza obok każdego wymienionego tam URL, aby usunąć pliki cookie i dane witryn.

Zauważ, że po usunięciu danych witryny z urządzenia będziesz musiał ponownie zalogować się, używając uwierzytelniania dwuskładnikowego.

Co zrobić, jeśli utracę dostęp do zaufanego urządzenia?

Jeśli utracisz dostęp do zaufanego urządzenia przed wygaśnięciem okresu zaufania, możesz skorzystać z opcji **Wyloguj się wszędzie**, aby usunąć dostęp ze wszystkich zalogowanych urządzeń (z wyjątkiem urządzenia, z którego obecnie korzystasz). Spowoduje to wylogowanie ze wszystkich innych urządzeń i cofnięcie uwierzytelniania dwuskładnikowego z dowolnych zaufanych urządzeń. Link **Wyloguj się wszędzie** znajdziesz w swoich Ustawieniach profilu. Następnie będziesz musiał(a) ponownie przeprowadzić proces logowania z 2FA na urządzeniach, do których masz dostęp.
