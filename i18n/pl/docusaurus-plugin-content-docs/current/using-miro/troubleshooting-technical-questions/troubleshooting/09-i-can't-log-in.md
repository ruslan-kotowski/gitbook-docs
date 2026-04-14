---
title: "Nie mog\u0119 si\u0119 zalogowa\u0107"
article_id: 360020993079
translation_id: 360020993079
locale: pl-pl
sidebar_position: 9
created_at: '2021-04-09T06:31:47Z'
updated_at: '2025-11-25T16:04:24Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Postępuj zgodnie z tym przewodnikiem, jeśli masz problemy z logowaniem się do swojego profilu Miro.

## Problemy z adresem e-mail i/lub hasłem

Mój adres e-mail/hasło nie działa

Oto dwa rozwiązania, które możesz odkryć:

1. Sprawdź dwukrotnie, czy adres e-mail/hasło używane do logowania nie ma literówek.
2. Jeśli wprowadzone dane dostępowe są poprawne, [zresetuj hasło](../../managing-your-profile/05-how-to-change-your-password.md).
3. Jeśli Twój adres e-mail lub hasło zawiera którykolwiek z symboli **& " < >**, prosimy [skontaktować się z naszym zespołem pomocy.](https://help.miro.com/hc/requests/new?)

:::warning
Pamiętaj, że Twój **profil zostaje zablokowany** po 10 próbach wprowadzenia adresu e-mail i hasła. Może być konieczne najpierw [odblokowanie profilu](../../tools/troubleshooting/14-profile-lockout.md), a następnie zresetowanie hasła.
:::

Nie mogę zresetować hasła

Jeśli nie otrzymasz wiadomości e-mail zresetowania hasła, mogą być trzy powody:

1. **Adres e-mail jest nieprawidłowy**
Upewnij się, że w przesłanym e-mailu nie ma literówek. Jeśli znajdziesz literówkę, spróbuj ponownie poprosić o reset.

2. **Adres e-mail nie jest jeszcze zarejestrowany w Miro**
W takim przypadku link do resetowania hasła nie zostanie wysłany na Twój adres e-mail. Zarejestruj nowy profil na stronie [rejestracji](https://miro.com/signup/). Jeśli Twój adres e-mail jest zarejestrowany, zobaczysz odpowiedni komunikat:
![mceclip0.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695734034_mceclip0.png)

3. **Występują problemy z dostarczaniem wiadomości e-mail**

- Otwórz swoje **foldery Spam, Promocje, Kosz, Społeczności** i **Aktualizacje** i sprawdź, czy jest tam wiadomość e-mail z prośbą o resetowanie.
- Może się również zdarzyć, że zapora sieciowa uniemożliwia dotarcie wiadomości e-mail do skrzynki odbiorczej.

  Skontaktuj się ze swoim *administratorem systemu* i poproś go o dodanie do listy dozwolonych naszych domen i subdomen: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) oraz [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/) i dodanie adresów IP naszego systemu wysyłania e-maili do listy dozwolonych po swojej stronie.

  Oto lista dedykowanych adresów IP: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. [Tutaj znajduje się artykuł](../../tools/troubleshooting/02-allowlist-miro-mailers.md) zawierający więcej informacji na temat nadawców, których powinieneś dodać do listy dozwolonych.

Zresetowałem hasło, ale nadal nie mogę się zalogować

Jeśli nadal nie masz dostępu do swojego profilu:

1. Upewnij się, że wprowadzasz nowe hasło.
2. Zaloguj się do trybu prywatnego (incognito) przeglądarki lub wypróbuj inną przeglądarkę.

Loguję się za pomocą jednego adresu e-mail, ale zostaję przekierowany i jestem zalogowany za pomocą innego adresu e-mail.

Problem może wystąpić, jeśli do logowania używasz alternatywnej metody uwierzytelniania (Google, Slack, Office 365, Apple ID, Facebook).

![new-sing-in-third-party.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
*Alternatywne opcje logowania na stronie logowania*

Możliwe, że przypadkowo połączyłeś swój adres e-mail Google/Office 365/itp. z Twoim profilem Miro zarejestrowanym pod innym adresem e-mail. Jeśli tak się stanie, spróbuj wykonać następujące czynności:

1. Usuń niewłaściwą relację e-mail, przechodząc do **Ustawień profilu** > **Integracje** i klikając **Wyloguj** obok Google/Office 365/itp.</span>
   ![usuń_połączenie.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Usuwanie powiązania za pomocą logowania Google*
2. Wyloguj się i zaloguj ponownie za pomocą adresu e-mail.

:::note
Skonfiguruj połączenie z adresem e-mail Google/Office 365/Slacka, który jest zgodny z adresem e-mail Twojego profilu Miro, aby zapobiec zgłoszeniu.
:::

## Logowanie SSO nie działa

Sprawdź artykuł: [Możliwe problemy z logowaniem SSO](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Niekończące się ładowanie podczas logowania

Dla użytkowników, którzy mają niekończące się problemy z ładowaniem po wprowadzeniu swoich danych dostępowych Miro, zalecamy następujące czynności:

1. Zaloguj się w **innej przeglądarce**.
2. Zaloguj się, używając przeglądarki w trybie **prywatnym (incognito).</strong>** Jeśli problem nie został powielony w trybie incognito albo innej przeglądarce, wyczyść pamięć podręczną przeglądarki.

   Jak wyczyścić pamięć podręczną Chrome

   1. Przejdź na `https://miro.com/` i otwórz **narzędzia dla programistów** Chrome (**Command + Option + J** *na Macu*, **Ctrl + Shift + J** *w systemie Windows*).
   2. Wybierz kartę **Aplikacja > Pamięć masowa**. Zobaczysz niebieski przycisk **Wyczyść dane witryny.**​  Kliknij przycisk i spowoduje to usunięcie wszelkich danych Miro zapisanych w przeglądarce Chrome, aby móc rozpocząć nową sesję roboczą.
   ![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
   *Opcja wyczyszczenia danych witryny w Chrome*
3. Jeśli używasz **VPN**, wyłącz lub włącz go.
4. Sprawdź w dziale IT, czy Twoja firma używa zapór sieciowych lub serwera proxy, które mogą blokować Miro. Podążaj za [tymi wytycznymi](../../tools/troubleshooting/01-add-miro-to-allowed-apps.md), aby **umieścić Miro na liście dozwolonych** lub zapewnić obejście.
5. Sprawdź połączenie internetowe. Jeśli przepustowość sieci nie osiąga minimum 8 Mb/s, **przełącz się na inną, najlepiej** **szybszą sieć**.
6. Spróbuj połączyć się z **mobilnym hotspotem**, jeśli jest dostępny. Następnie, ponownie połącz się z oryginalną siecią.
7. Jeśli to nie pomoże, [prześlij prośbę](https://miro.com/contact/recover/) i [wyślij dzienniki konsoli przeglądarki do pomocy technicznej](../../tools/troubleshooting/07-how-to-troubleshoot-and-report-a-bug.md).</span>

## Problemy z logowaniem w aplikacji komputerowej Miro

1. Jeśli nie możesz uzyskać dostępu do Miro w aplikacji komputerowej, zaloguj się za pomocą przeglądarki. Jeśli nadal nie możesz się zalogować, wykonaj <span>powyższe kroki. Jeśli możesz uzyskać dostęp do Miro w przeglądarce, wykonaj poniższe kroki.
2. Resetuj dane aplikacji.

Jak zresetować dane aplikacji w systemie Windows

Naciśnij **Alt > Pomoc**i wybierz resetowanie danych aplikacji, jak pokazano na poniższym zrzucie ekranu:

​​![resetuj_dane_aplikacji_na_Windows.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725434514_reset%20app%20data%20on%20Windows.jpg)
*Resetowanie danych aplikacji w aplikacji komputerowej dla systemu Windows*

Jeśli nie możesz znaleźć menu, prawdopodobnie używasz aplikacji pobranej z MS Store. W takim przypadku, aby zresetować dane aplikacji, otwórz Windows **Ustawienia** > **Aplikacje** > **Aplikacje i funkcje** > znajdź **Miro** na liście > **Opcje zaawansowane**> **Resetuj**.

Jeśli to nie pomoże od razu, usuń wszystkie pliki aplikacji z **C:\Users\username\AppData\Roaming\RealtimeBoard** i **C:\Users\username\AppData\Local\RealtimeBoard**

> **✏️** Jeśli folder **Appdata** jest ukryty, zobacz [tutaj](https://support.microsoft.com/windows/view-hidden-files-and-folders-in-windows-10-97fbc472-c603-9d90-91d0-1166d1d9f4b5) jak go wyświetlić.

Jak zresetować dane aplikacji na komputerze Mac

Kliknij Miro w menu u góry i wybierz **Resetuj dane aplikacji**, jak pokazano na poniższym zrzucie ekranu:

![resetuj_dane_aplikacji_na_Mac.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017695741458_reset%20app%20data%20on%20Mac.jpg)
*Resetowanie danych aplikacji na komputerze Mac*

Następnie spróbuj ponownie zalogować się do aplikacji i sprawdź, czy zgłoszenie zostało rozwiązane.

Jeśli resetowanie nie przyniesie natychmiastowej pomocy, otwórz okno Findera > naciśnij **Command + Shift + G** > wklej  **~/Library/Application Support/RealtimeBoard** i usuń wszystkie pliki aplikacji.

3. Jeśli problem nie ustąpi, upewnij się, że używasz najnowszej wersji aplikacji pobranej [z naszej strony internetowej.](https://miro.com/apps/)

## Logowanie Google/Office 365/Slack/itp.

Nie mogę zalogować się przez Google/Office/Slack/etc.

1. Zaloguj się do Miro przy użyciu standardowych danych dostępowych (adres e-mail i hasło).</span> Jeśli nie pamiętasz lub nie masz hasła, [zresetuj hasło](../../managing-your-profile/05-how-to-change-your-password.md).
2. Przejdź do **Ustawień profilu** > **Integracje**, kliknij **Wyloguj** obok Google/Office 365/itp. i ponownie skonfiguruj połączenie.
   ![remove_connection.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725424658_remove%20connection.jpg)
   *Usuwanie powiązania za pomocą logowania Google*

Nie mogę zalogować się przez Google/Office/Slack/itp. w aplikacji komputerowej

Poznaj te kroki rozwiązywania problemów.

Logowałem się do Miro za pośrednictwem Google/Office 365/itp., ale moja usługa e-mail uległa zmianie. Jak się teraz zalogować?

Zaloguj się do Miro przy użyciu nowych danych dostępowych usługi (adres e-mail i hasło). Jeśli nie pamiętasz lub nie masz hasła, [zresetuj je](../../managing-your-profile/05-how-to-change-your-password.md).

## Problemy z logowaniem na tablecie lub urządzeniu mobilnym

1. Sprawdź, czy możesz zalogować się do wersji przeglądarkowej. Jeśli nie, zalecamy tekroki rozwiązywania problemów.
2. Jeśli logowanie działa dla Ciebie w przeglądarce, może się zdarzyć, że dane uwierzytelniania Twojego urządzenia są uszkodzone. Przejdź do **ustawień aplikacji > Pamięć masowa > Wyczyść pamięć** lub ponownie zainstaluj aplikację Miro na swoim urządzeniu.

## Wskazówki dotyczące rozwiązywania problemów

Jeśli nie możesz znaleźć powyższego rozwiązania, zaloguj się do Miro przy użyciu **innej przeglądarki** lub **trybu incognito**. Jeśli wszystko jest dobrze w trybie incognito przeglądarki, wyczyść pamięć podręczną przeglądarki i pliki cookie oraz zaloguj się do Miro w trybie standardowym.

Jak wyczyścić pamięć podręczną Chrome

1. Przejdź do `https://miro.com/` i otwórz **Narzędzia dla programistów**Chrome (**Command + Option + J** *na Macu*, **Ctrl + Shift + J***w systemie Windows*).
2. Wybierz kartę **Aplikacja > Pamięć masowa**. Zobaczysz niebieski przycisk **Wyczyść dane witryny.**​  Kliknij przycisk, a spowoduje to usunięcie wszelkich danych Miro zapisanych w przeglądarce Chrome, aby móc rozpocząć nową sesję roboczą.

![clear_site_data.jpg](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725432466_clear%20site%20data.jpg)
*Opcja wyczyszczenia danych witryny w Chrome*

Jeśli to nie pomoże, [skontaktuj się z pomocą techniczną Miro](https://miro.com/contact/recover/). Szczegółowo opisz zgłoszenie.

:::note
Jeśli masz problemy z rejestracją w Miro, sprawdź [Problemy z kodem potwierdzającym](../../tools/troubleshooting/12-issues-with-confirmation-code-or-password-reset-emails.md).
:::
