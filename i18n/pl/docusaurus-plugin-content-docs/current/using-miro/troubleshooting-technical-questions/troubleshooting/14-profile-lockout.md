---
title: Blokada profilu
article_id: 360017571374
translation_id: 360017571374
locale: pl-pl
sidebar_position: 14
created_at: '2019-02-11T10:08:55Z'
updated_at: '2026-02-24T12:02:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Blokada profilu jest standardowa dlawszystkich użytkowników Miro i wersji, a dostosowanie jej nie jest dostępne. Użytkownicy próbujący [uwierzytelniać się przez zewnętrznych dostawców tożsamości](../../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) nie będą objęci tą funkcją.

Po błędnym zalogowaniu się do swojego profilu masz **10 prób** na wpisanie poprawnego hasła dla pary e-mail i hasło. Pierwsze 5 prób jest standardowych, bez dodatkowej złożoności.

Kolejne próby dodają captcha (tylko dla aplikacji internetowej i komputerowej). Jeśli nie uda Ci się podać poprawnego hasła **10 razy z rzędu** dla pary e-mail i hasło, Twój profil użytkownika zostanie zablokowany na**1 godzinę**, w trakcie której wszystkie próby zalogowania się do profilu zakończą się niepowodzeniem, nawet jeśli podane hasło jest poprawne.

:::tip
Podczas godziny blokady możesz spróbować zalogować się bez hasła lub używając dostawcy społecznościowego.
:::

Gdy Twój profil użytkownika zostanie zablokowany, Miro wyśle Ci e-maila z sześciocyfrowym kodem do odblokowania profilu. Link w e-mailu przekieruje Cię na stronę potwierdzenia, gdzie musisz podać sześciocyfrowy kod. Jeśli podany kod jest poprawny, profil zostaje odblokowany, a wszystkie próby są resetowane. W e-mailu zaleca się również zmianę hasła.

Zablokowany profil zostaje odblokowany **automatycznie** po upływie 1 godziny, a wszystkie nieudane próby zostają zresetowane.

### Co zrobić, jeśli nie otrzymasz kodu

Jeśli nie możesz znaleźć e-maila w swojej skrzynce odbiorczej, wykonaj następujące kroki rozwiązywania problemów:

- Upewnij się, że nie ma literówek w e-mailu, który podałeś(-aś). Jeśli znajdziesz literówkę, spróbuj zalogować się za pomocą prawidłowego adresu
- Otwórz swoje **foldery Spam, Oferty, Wiadomości-śmieci, Społecznościowe** oraz **Aktualizacje** i sprawdź, czy wiadomość potwierdzająca od Miro tam jest
- Sprawdź, czy Twoja skrzynka odbiorcza nie jest pełna, aby upewnić się, że nie osiągnąłeś(-aś) limitu pamięci w swojej skrzynce e-mailowej. Jeśli jest pełna, możesz potrzebować usunąć niektóre istniejące wiadomości, aby móc otrzymywać nowe. Po usunięciu wiadomości kliknij **Wyślij kod ponownie**, aby otrzymać e-mail rejestracyjny
- Może się zdarzyć, że zapora sieciowa uniemożliwia dostarczenie e-maila do Twojej skrzynki odbiorczej. Skontaktuj się z *administratorem systemu* i poproś, aby dodał nasze domeny i subdomeny do listy dozwolonych: [miro.com](http://miro.com/)*, *.[miro.com](http://miro.com/), [mirostatic.com](http://mirostatic.com/)*, *.[mirostatic.com](http://mirostatic.com/) i [realtimeboard.com](http://realtimeboard.com/)*, *.[realtimeboard.com](http://realtimeboard.com/). [Tutaj znajdziesz artykuł](../../tools/troubleshooting/02-allowlist-miro-mailers.md) z większą ilością informacji o mailerach, które należy dodać do listy dozwolonych.
- Użytkownicy AOL/CompuServe: upewnij się, że Twoje Kontrola poczty zostały ustawione na odbieranie e-maili z Internetu. Jeśli masz zablokowane e-maile internetowe, zmień kontrolę poczty, wprowadzając **Kontrola poczty** na AOL lub CompuServe. Następnie wróć do naszego formularza rejestracyjnego, aby ponownie wysłać kod potwierdzający
- Zazwyczaj kod powinien dotrzeć natychmiast, ale z powodu specyfiki Twojego systemu pocztowego, może być konieczność czekania do 24 godzin
- Jeśli żadna z rozwiązań nie pomoże,  [zgłoś problem do pomocy Miro](../../tools/troubleshooting/06-contacting-miro-support.md).
