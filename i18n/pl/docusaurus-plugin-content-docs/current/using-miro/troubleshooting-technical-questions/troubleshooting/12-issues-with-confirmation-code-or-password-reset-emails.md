---
title: "Problemy z otrzymywaniem kod\xF3w potwierdzaj\u0105cych lub wiadomo\u015B\
  ci e-mail do resetowania has\u0142a"
article_id: 360017731373
translation_id: 360017731373
locale: pl-pl
sidebar_position: 12
created_at: '2019-02-11T10:14:22Z'
updated_at: '2024-10-25T14:25:54Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Brak otrzymania kodu potwierdzającego lub wiadomości e-mail w celu zresetowania hasła może być spowodowany wieloma przyczynami. Poniżej przedstawiamy kilka opcji, które mogą pomóc rozwiązać ten problem.

## Typowe powody braku otrzymania kodu lub wiadomości e-mail

Dwa najczęstsze powody, dla których możesz nie otrzymywać wiadomości e-mail do resetowania hasła lub nie móc poprosić o nowy kod potwierdzający, to:

1. Twoja firma używa zapory sieciowej, która blokuje wiadomości e-mail z domen miro.com. Poproś administratora IT o umożliwienie otrzymywania wiadomości e-mail z domen [miro.com](http://miro.com/). Jeśli jesteś administratorem, zapoznaj się z poniższymi instrukcjami dotyczącymi dodania domen Miro do listy dozwolonych.
2. Twoja firma używa pojedynczego logowania. Zobacz sekcję poniżej, aby uzyskać instrukcje dotyczące rozwiązania tego problemu.

## Jak rozwiązać problemy z brakiem wiadomości e-mail lub kodu potwierdzającego

1. Jeśli Twoja firma używa pojedynczego logowania (SSO), musisz zalogować się za pomocą firmowych poświadczeń SSO. Jeśli spróbujesz zresetować hasło do Miro, przekierujemy Cię z powrotem na stronę pojedynczego logowania. W takim przypadku spróbuj użyć firmowych poświadczeń SSO. Jeśli to nie zadziała, wypróbuj kolejne kroki przedstawione poniżej.
2. Zapora sieciowa może uniemożliwiać dotarcie wiadomości e-mail do skrzynki odbiorczej. Skontaktuj się z administratorem systemu i poproś o dodanie do listy dozwolonych naszych domen i subdomen: miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com oraz realtimeboard.com*, *.realtimeboard.com.

   Oto lista dedykowanych adresów IP: 198.2.178.132, 198.2.178.117, 198.2.128.203, 198.2.178.252, 198.2.178.205. Przeczytaj więcej o [umożliwianiu odbierania wiadomości e-mail od Miro.](../../tools/troubleshooting/02-allowlist-miro-mailers.md)
3. Upewnij się, że w podanym adresie e-mail nie ma literówek. Jeśli znajdziesz literówkę, [zarejestruj ponownie profil](../../../getting-started/start-here/02-how-to-register-with-miro.md) lub zresetuj hasło za pomocą prawidłowego adresu e-mail.
4. Sprawdź foldery **Spam, Oferty**, **Kosz, Społeczności** i **Powiadomienia** u swojego dostawcy poczty e-mail.
5. Możesz również zarejestrować się lub zalogować za pomocą alternatywnych opcji rejestracji lub logowania: za pomocą Google, Slack, Office 365, Apple lub Facebooka.
   > ⚠️ Pamiętaj, że alternatywne sposoby logowania **nie** są połączone z firmowymi loginami SSO. Jeśli używasz Miro w środowisku korporacyjnym, użyj poświadczeń ustawionych dla Ciebie przez administratora Miro.

   ![new-sing-in-third-party.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725436050_new-sing-in-third-party.png)
   *Dostępne metody uwierzytelniania*

Jeśli nie możesz się zarejestrować lub zalogować za pomocą innych metod uwierzytelniania:

- Sprawdź, czy skrzynka odbiorcza jest pełna i czy nie skończył się limit miejsca na wiadomości e-mail. Jeśli jest pełna, może być konieczne usunięcie niektórych wiadomości e-mail, aby móc otrzymać nowe. Po usunięciu wiadomości e-mail wróć do naszej strony rejestracji i kliknij **Wyślij kod ponownie.**
- Wiadomość e-mail powinna zostać natychmiast wysłana. Jeśli tak się nie stanie, może być konieczne odczekanie do 24 godzin.
- Jeśli używasz firmowych poświadczeń SSO i nie możesz się zalogować, przeczytaj o [typowych błędach dotyczących SSO i jak je rozwiązać](../../tools/troubleshooting/10-i-can't-log-in-via-sso.md).

### Inne problemy z potwierdzeniem

Mój kod jest nieprawidłowy

Jeśli wprowadzony kod jest **nieprawidłowy:**

1. Sprawdź skrzynkę odbiorczą i upewnij się, że wprowadzasz ostatnio otrzymany kod. Jeśli kod jest nadal nieprawidłowy, kliknij **Wyślij kod ponownie** i wprowadź kod z nowej wiadomości e-mail.
2. Innym sposobem zakończenia rejestracji jest kliknięcie **Potwierdź adres e-mail** w wiadomości e-mail z kodem potwierdzającym. W takim przypadku nie potrzebujesz kodu potwierdzającego.
   ![confirm email button.png](../../../../../../../docs/using-miro/troubleshooting-technical-questions/troubleshooting/images/21017725339026_confirm%20email%20button.png)
   *Opcja potwierdzenia adresu e-mail*

Przekroczono limit prób potwierdzenia adresu e-mail

Jeśli nie udało Ci się potwierdzić adresu e-mail po 4 próbach, na stronie rejestracji zobaczysz informację:  **Próby potwierdzenia adresu e-mail zostały przekroczone**.

Poczekaj 60 sekund i kliknij **Wyślij kod ponownie** – spowoduje to wygenerowanie nowego kodu. Wprowadź kod i zakończ rejestrację.

Przypadkowo zamknięta została karta, w której wprowadzam kod potwierdzający.

[Zaloguj się](https://miro.com/login/) za pomocą adresu e-mail i hasła podanego podczas rejestracji, a ponownie przekierujemy Cię na stronę [z potwierdzeniem](https://miro.com/email-confirm/).

:::note
Jeśli nie potwierdzisz adresu e-mail, otrzymasz przypomnienia po 12 i 24 godzinach. Jeśli adres e-mail nie zostanie potwierdzony w ciągu 7 dni, **profil zostanie usunięty**. Nowy profil będzie można zarejestrować za pomocą tego samego adresu e-mail.
:::

:::note
Kody potwierdzające można wysłać tylko za pośrednictwem poczty e-mail.
:::

:::note
Jeśli nadal masz problemy, [skontaktuj się z pomocą techniczną Miro](https://miro.com/contact/recover/).
:::
