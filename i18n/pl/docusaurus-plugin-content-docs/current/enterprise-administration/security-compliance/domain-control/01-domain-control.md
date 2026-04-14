---
title: "Zarz\u0105dzanie domen\u0105"
article_id: 360034831793
translation_id: 21892828003090
locale: pl-pl
sidebar_position: 1
created_at: '2024-10-10T08:06:39Z'
updated_at: '2026-03-27T15:51:50Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  plans: business, enterprise
  roles: company_admin, system_admin
---

> **Dostępne w:** Business, Enterprise
> **Wymagana rola:** administrator firmy, administrator systemu

Zarządzanie domeną umożliwia administratorom firmowym zarządzanie dostępem użytkowników w ramach ich subskrypcji. Dzięki zarządzaniu domeną, administratorzy mogą egzekwować zgodność z wymogami bezpieczeństwa korporacyjnego i monitorować aktywności zarządzanych użytkowników w ich domenach.

Dowiedz się, jak skonfigurować i zarządzać zarządzaniem domeną w swojej organizacji.

**Dzięki zarządzaniu domeną, administratorzy wersji Enterprise mogą:**

- Przeprowadzać audyty w celu identyfikacji użytkowników powiązanych z zarządzaną domeną, która nie jest włączona do Twojej subskrypcji, i zapraszania ich do dołączenia.
- Zapobiegać tworzeniu nieautoryzowanych subskrypcji przez użytkowników w ramach domeny.
- Automatycznie dodawać nowo zarejestrowanych użytkowników do wyznaczonych zespołów.
- [Blokować dezaktywowanych użytkowników](../../user-management/02-block-deactivated-users.md), aby uniemożliwić im dostęp do Miro przy użyciu ich służbowego adresu e-mail.

**Administratorzy wersji Business:**

- Mogą używać zautomatyzowanej weryfikacji domen do zarządzania domenami. Tylko nowo dodane domeny będą automatycznie weryfikowane.
- Nie mogą zmieniać zasad zarządzania domeną.
- Nie mogą prosić o audyt domeny.

![domain-policies-business.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21046889202834_domain-policies-business.png)

*Zasady domen można wyświetlić w obrębie zarządzanych domen dla użytkowników wersji Business*

Użytkownicy z planem Business będą musieli przejść na wyższą wersję dla innych zaawansowanych funkcji.

:::note
Zarządzanie zbiorcze domenami nie jest obecnie obsługiwane.
:::

## Domena główna

Twoja główna domena decyduje o tym, jak Miro identyfikuje wewnętrznych i zewnętrznych użytkowników w Twojej organizacji. Aby dowiedzieć się, jak wyświetlić, zmienić lub zarządzać główną domeną, zobacz [Zarządzanie główną domeną](https://help.miro.com/hc/en-us/articles/34249718672274).

## Skonfiguruj zarządzanie domeną

### Krok 1: Dodaj domeny

1. Otwórz swój pulpit Miro.
2. Kliknij swoje zdjęcie profilowe w prawym górnym rogu.
3. Wybierz **Ustawienia** z menu rozwijanego.
4. W lewym panelu przejdź do **Zabezpieczenia i zgodność**, a następnie kliknij **Zarządzane domeny**

   > ✏️ W wersji Business opcja **Zarządzane domeny** znajduje się w sekcji **Konto**.
5. Kliknij **+ Dodaj domenę** i wprowadź pełną nazwę domeny (np. yourcompany.com).
   ![Managed-domains-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318776338_Managed-domains-settings.png)
*Ustawienia zarządzania domenami*

:::note
Jeśli masz włączoną opcję [**Blokuj dezaktywowanych użytkowników**](../../user-management/02-block-deactivated-users.md), to wszyscy dezaktywowani użytkownicy powiązani z nowo zweryfikowaną domeną zostaną zablokowani automatycznie.
:::

### Krok 2: Zweryfikuj domeny

1. Po dodaniu domeny otrzymasz kod weryfikacyjny w ustawieniach **Zarządzanej domeny**. Skopiuj ten kod.

   ![Complete-domain-verification.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318779282_Complete-domain-verification.png)
*Kopiowanie kodu weryfikacyjnego*
2. Jeśli zarządzasz swoimi wpisami DNS, zaktualizuj ustawienia DNS, dodając wpis TXT z kodem weryfikacyjnym jako jego **Wartość**. (Jeśli ktoś inny zarządza Twoimi wpisami DNS, przekaż mu kod weryfikacyjny z instrukcją aktualizacji wpisów DNS.)
3. Zaloguj się na stronę swojego dostawcy domen (GoDaddy, Amazon, Cloudflare itp.) i przejdź do sekcji **DNS** **rekordy**.
4. Utwórz nowy **wpis TXT** z następującymi specyfikacjami:
   **Wartość/Odpowiedź/Opis:** *„miro-verification=[WPROWADŹ KOD WERYFIKACYJNY]”*
   **Nazwa/Host/Alias:** Pozostaw to pole puste lub wpisz @, aby uwzględnić subdomenę.
   **Czas życia (TTL):** „86400” (można też odziedziczyć z domyślnej konfiguracji).

   ![Creating-new-TXT-record.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318775314_Creating-new-TXT-record.png)
   *Tworzenie nowego wpisu TXT*

:::note
Możesz zaktualizować wpis TXT poprzez konsolę administracyjną lub pulpit dostawcy DNS hostującego domenę. Wyświetl [listę dostawców DNS](https://support.google.com/a/topic/1409901).
:::

### Krok 3: Sprawdź weryfikację domeny

1. Po zaktualizowaniu wpisu DNS natychmiast sprawdź status weryfikacji swojej domeny w ustawieniach **Zarządzanej domeny**, klikając **Sprawdź weryfikację**.
2. Jeśli domena nie zostanie zweryfikowana natychmiast, Miro automatycznie będzie sprawdzać kod weryfikacyjny co 2 godziny przez następne 30 dni.

### Krok 4: Powiadomienie o stanie weryfikacji

1. Po pomyślnej weryfikacji domeny otrzymasz powiadomienie e-mailowe potwierdzające stan weryfikacji.
2. Proszę nie usuwać wpisu DNS po zakończeniu weryfikacji, ponieważ może być potrzebny do przyszłych weryfikacji.
   ![Check-domain-verification.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017348597650_Check-domain-verification.png)
*Sprawdzanie weryfikacji domeny*

## Zasady weryfikacji domen

- Musisz utworzyć oddzielny wpis TXT dla każdej głównej domeny oraz każdej subdomeny, z której korzystasz. Powtórz kroki 1-4 powyżej dla każdej domeny lub subdomeny, którą chcesz zweryfikować.
- Twoja domena musi być dokładnym odwzorowaniem.

  > ✏️ Subdomeny są niedozwolone.
- Upewnij się, że wszystkie strefy używane w konfiguracji zweryfikowanej domeny są uwzględnione.
- Nazwa domeny w pełni kwalifikowana (FQDN) powinna odpowiadać adresowi Twojej domeny. Na przykład, [www.mycompanydomain.com](http://www.mycompanydomain.com).
- Jeśli korzystasz zarówno z wewnętrznego, jak i zewnętrznego DNS, zalecamy zweryfikowanie obu, aby zapewnić kompleksowe zarządzanie domeną.

## Zarządzanie użytkownikami i dostępem

### Edytuj ustawienia domeny

Ustawienia domeny określają sposób zarządzania istniejącymi i nowo zarejestrowanymi użytkownikami w Twojej domenie/domenach.

1. Gdy domena zostanie zweryfikowana, kliknij w menu z 3 kropkami (**...**) i wybierz **Edycja ustawień domeny**.
   ![Edit-domain-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318773138_Edit-domain-settings.png)
*Edycja ustawienia domeny*
2. Zostaną wyświetlone opcje dotyczące obsługi nowych użytkowników w Twojej domenie:

- **Automatycznie przechwytuj nowych użytkowników**: Automatycznie dodawaj użytkowników, którzy rejestrują się w Miro z domeną zarządzaną do subskrypcji tej domeny z domyślnym typem licencji. Możesz także określić, do których zespołów użytkownicy zostaną dodani (wymagane).
- **Blokuj użytkownikom możliwość tworzenia własnych subskrypcji**: Zabroń zarządzanym użytkownikom w Twojej domenie(/domenach) tworzenia nowych zespołów poza Twoją subskrypcją. Jednak Ci użytkownicy nadal mogą być zapraszani do zespołów w Twojej domenie(/domenach) i współpracować zewnętrznie.

  ![Managed-domain-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318773778_Managed-domain-settings.png)
*Opcje obsługi nowych użytkowników dla twojej domeny*

  > ✏️ Jeśli włączysz **Blokuj użytkownikom możliwość tworzenia własnych subskrypcji**, użytkownicy nie mogą się samodzielnie rejestrować, chyba że zostaną zaproszeni, aktywna jest funkcja "auto-capture" lub JIT.

### Użytkownicy wewnętrzni i zewnętrzni

Kiedy domena zostanie potwierdzona, szczegóły użytkownika będą zawierały klasyfikację jako **wewnętrzny** lub **zewnętrzny**.

![](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/33613933595794_image.png) *Szczegóły użytkownika pokazują, czy użytkownik jest zewnętrzny czy wewnętrzny względem Twojej zweryfikowanej domeny*

Wewnętrzni użytkownicy posiadają adres e-mail z domeny potwierdzonej przez Twoje konto Enterprise. Na przykład, `użytkownik@acme.com`, gdzie `acme.com` jest jedną z Twoich zweryfikowanych domen.

Zewnętrzni użytkownicy posiadają adres e-mail spoza jakiejkolwiek domeny potwierdzonej przez Twoje konto Enterprise. Na przykład, `użytkownik@not-domain.com`, gdzie `not-domain.com` nie jest jedną z Twoich zweryfikowanych domen.

:::note
Szczegóły użytkownika są widoczne w jego profilu. W konsoli administracyjnej szczegóły użytkowników są również widoczne na liście użytkowników, gdzie opcjonalnie możesz filtrować według klasyfikacji **wewnętrznej** lub **zewnętrznej**.
:::

Klasyfikacja wewnętrzna lub zewnętrzna jest automatyczna i opiera się na tym, czy domena użytkownika jest przejęta i zweryfikowana przez Twoje konto Enterprise.

## Konsolidacja zespołów samoobsługowych do wersji Enterprise

Jako administrator firmy możesz zebrać wszystkie zespoły utworzone z Twoich domen w ramach wersji Enterprise. To zapewnia zwiększone bezpieczeństwo, lepszą współpracę i usprawnia zarządzanie przez zjednoczenie wszystkich zespołów w jednym miejscu. Dodatkowo, możesz także przeprowadzać audyt domen, aby zidentyfikować i skonsolidować użytkowników i zespoły, które są częścią zarządzanej przez Ciebie domeny, ale obecnie znajdują się poza Twoją subskrypcją.

Więcej informacji znajdziesz w [dokumentacji Konsolidacji zespołów](../../managing-enterprise-teams-and-content/06-self-serve-teams-to-enterprise-plan-consolidation.md).

## Prośby o zmianę e-maila

Jeśli Twoja firma zarejestrowała domenę, każdy użytkownik powiązany z tą domeną nie będzie mógł zmienić swojego adresu e-mail w Miro bez zgody administratora firmy. Podczas próby zmiany e-maila użytkownicy otrzymają następujący komunikat: **Nie możesz zmienić adresu e-mail z adresu w domenie należącej do organizacji lub na taki adres.** Zaleca się, aby użytkownicy skontaktowali się ze swoim administratorem firmy, który następnie skontaktuje się z pomocą Miro, aby uzyskać pomoc.

## Często zadawane pytania

Czy mogę używać zarządzania domeną z subdomeną?

Tak, subdomeny są traktowane jako oddzielne jednostki od domen głównych. Postępuj zgodnie z procesem konfiguracji dla każdej subdomeny, którą chcesz zweryfikować.

Jak używać pojedynczego logowania z zarządzaniem domeną?

Będziesz musiał(a) najpierw skonfigurować zarządzanie domeną przed włączeniem uwierzytelniania [pojedynczego logowania](../../security-integrations/single-sign-on-sso/09-single-sign-on-(sso).md).

Co zrobić, jeśli moja domena się zmienia lub chcę dodać subdomenę?

Jeśli nazwa Twojej domeny ulega zmianie, usuń domenę i rozpocznij proces weryfikacji od nowa z nową domeną lub z dowolnymi dodanymi subdomenami.

Gdzie znajdę rekordy DNS dla mojej domeny?

Aby zlokalizować rekordy DNS swojej domeny, musisz uzyskać dostęp do platformy rejestratora domeny, gdzie zarejestrowałeś domenę. Jeśli nie jesteś pewien, kto jest Twoim rejestratorem, możesz znaleźć tę informację, korzystając z **who.is** do wyszukania domeny. Po zidentyfikowaniu rejestratora, zaloguj się na jego stronie internetowej i przejdź do sekcji zwykle oznaczonej jako **Domeny** lub **Zarządzanie DNS**. Tutaj znajdziesz ustawienia lub rekordy DNS dla swojej domeny.

Dlaczego nie widzę opcji **Zarządzane domeny** w moich ustawieniach **Bezpieczeństwo i zgodność**?

Jeśli nie widzisz opcji **Zarządzane domeny**, może to być spowodowane dwoma powodami:

- Nie masz subskrypcji na wersję Enterprise, która zawiera tę funkcję.
- Nie masz roli administratora firmy wymaganej do dostępu do tego ustawienia.

Prosimy o zweryfikowanie szczegółów swojego abonamentu oraz roli z administratorem firmy, aby uzyskać dalszą pomoc.

Czy mogę usunąć wpis TXT dla mojej domeny po jej weryfikacji?

Usunięcie wpisu TXT po weryfikacji nie wpłynie natychmiast na działanie zarządzania domeną, jednak zdecydowanie zaleca się zachowanie tego wpisu. Utrzymanie wpisu TXT jest kluczowe dla ewentualnych procesów ponownej weryfikacji w przyszłości. Usunięcie wpisu TXT mogłoby skomplikować te procesy i wymagać ponownego przejścia kroków weryfikacyjnych.
