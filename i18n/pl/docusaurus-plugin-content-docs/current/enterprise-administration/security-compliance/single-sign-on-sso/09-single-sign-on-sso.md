---
title: Pojedyncze logowanie (SSO)
article_id: 360017571414
translation_id: 360017571414
locale: pl-pl
sidebar_position: 9
created_at: '2019-02-11T10:08:59Z'
updated_at: '2026-01-07T13:25:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Dzięki pojedynczemu logowaniu (SSO) przez SAML użytkownicy mogą uzyskać dostęp do Miro za pośrednictwem wybranego dostawcy tożsamości (IdP).

> **Dostępność:** wersje Business i Enterprise.
> **Wymagana rola:** administrator firmy.

## Jak działa logowanie pojedyncze przez SAML

1. Gdy użytkownik Miro próbuje zalogować się do Miro za pomocą SSO, Miro wysyła żądanie przez SAML (Security Assertion Markup Language) do dostawcy tożsamości (IdP).
2. Dostawca tożsamości sprawdza poświadczenia użytkownika i wysyła odpowiedź z powrotem do Miro, aby potwierdzić tożsamość uczestnika.
3. Miro potwierdza odpowiedź i przyznaje dostęp, umożliwiając uczestnikowi zalogowanie się na swoje konto Miro.

## Co się stanie po włączeniu SSO?

**Włączanie logowania pojedynczego po raz pierwszy**

Przy pierwszym skonfigurowaniu pojedynczego logowania istniejący użytkownicy będą mogli mogą nadal pracować w Miro. Jednak po następnym wylogowaniu, wygaśnięciu sesji lub przy próbie zalogowania się z nowego urządzenia będą musieli zalogować się za pomocą SSO.

Inne opcje logowania zostaną wyłączone, w tym standardowy login i hasło oraz logowanie przez Google, Facebook, Slack, AppleID i O365.

**Limit czasu bezczynności**

Jeśli masz włączony [limit czasu bezczynności](../../security-integrations/security-management/02-idle-session-timeout.md), użytkownicy są automatycznie wylogowywani ze swojego profilu Miro i będą musieli ponownie wprowadzić swoje dane uwierzytelniania przez SSO.

**Kilka zespołów i organizacji**

Jeśli użytkownicy należą do wielu zespołów Miro lub organizacji, możesz skonfigurować ich ustawienia tak, aby używali tego samego dostawcy tożsamości (IdP) do uwierzytelniania.

**Użytkownicy zobowiązani do logowania się za pomocą SSO**

Pojedyncze logowanie jest wymagane w przypadku aktywnych użytkowników, którzy są objęci subskrypcją Enterprise *i* mają domenę uwzględnioną w ustawieniach pojedynczego logowania.

- Użytkownicy uzyskujący dostęp do Miro z domen niedodanych do ustawień pojedynczego logowania nie muszą logować się za pomocą SSO i powinni zamiast tego logować się przy użyciu standardowych metod.
- Użytkownicy ze zweryfikowanej domeny, którzy nie korzystają z Twojej subskrypcji Miro Enterprise, muszą logować się za pomocą pojedynczego logowania tylko wtedy, gdy włączona jest [usługa udostępniania Just-in-Time (JIT)](../../user-management/13-user-provisioning-on-enterprise-plan.md). Ci użytkownicy zostaną automatycznie dodani do wstępnie skonfigurowanego zespołu i będą musieli logować się przez SSO.
- [Zarządzani użytkownicy](../../user-management/06-managed-users-on-enterprise-plan.md), którzy należą do zespołu Miro poza Twoją subskrypcją Enterprise, muszą nadal korzystać z pojedynczego logowania do uwierzytelniania. Ci użytkownicy będą mieli dostęp do innych zespołów. Aby ograniczyć dostęp do określonych zespołów, zaktualizuj ustawienia [zarządzania domeną](../../canvas-25-admin-features/domain-control/01-domain-control.md).

**Zarządzanie danymi użytkownika**

Dane użytkownika są automatycznie przypisywane w Miro przez dostawcę tożsamości po pomyślnym logowaniu. Niektórych parametrów, takich jak nazwa i hasło, nie można zmienić. Inne parametry, m.in. dział czy zdjęcie profilowe, są opcjonalne.

- Nazwy użytkowników Miro są aktualizowane po każdym pomyślnym uwierzytelnieniu użytkownika. Aby dowiedzieć się więcej o konfigurowaniu nazw użytkowników Miro, przeczytaj informacje o zaawansowanych ustawieniach pojedynczego logowania. Jeśli chcesz zmienić adres e-mail użytkownika, możesz to zrobić tylko za pośrednictwem [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md). Jeśli nie korzystasz z SCIM, [skontaktuj się z zespołem pomocy](https://help.miro.com/hc/requests/new?referer=help-center-article).

![Allowed-Email-Domains-Image1.png](https://help.miro.com/hc/article_attachments/12810848665490)*Domeny w ustawieniach SSO*

> **💡**Aby zapobiec zablokowaniu konta, utwórz konto użytkownika „awaryjnego” za pomocą adresu e-mail w domenie nieznajdującej się na liście w ustawieniach SSO, np. uzytkownikawaryjny@gmail.com. Możesz także poprosić dział pomocy o wyłączenie pojedynczego logowania dla całej organizacji.

## Konfigurowanie SSO

### Dostawcy tożsamości (IdP)

Użyj dowolnego dostawcy tożsamości. Poniżej wymieniamy najpopularniejsze platformy dostawców tożsamości:

- [OKTA](../../security-integrations/single-sign-on-sso/07-how-to-configure-okta-sso.md)
- [Azure AD](../../security-integrations/single-sign-on-sso/05-how-to-configure-entra-id-sso.md) od firmy Microsoft
- [OneLogin](../../security-integrations/single-sign-on-sso/08-how-to-configure-onelogin-sso.md)
- [ADFS](../../security-integrations/single-sign-on-sso/02-how-to-configure-adfs-sso.md) od firmy Microsoft
- [Auth0](../../security-integrations/single-sign-on-sso/03-how-to-сonfigure-auth0-sso.md)
- [Google SSO](../../security-integrations/single-sign-on-sso/06-how-to-configure-google-sso.md)
- [Jumpcloud SSO](https://support.jumpcloud.com/support/s/article/single-sign-on-sso-with-miro).

### Konfigurowanie dostawcy tożsamości

> ****💡****Jeśli organizacja korzysta z abonamentu Enterprise i chce dodać [wielu dostawców tożsamości](../../security-integrations/single-sign-on-sso/01-adding-multiple-identity-providers.md) (IdP), zarejestruj się, aby korzystać z [prywatnej wersji beta](https://coda.io/form/Miro-Multi-IdP-Private-Beta-Sign-Up_dkoTJMza_jV).

1. Przejdź do sekcji konfiguracji dostawcy tożsamości i postępuj zgodnie z instrukcjami dostawcy, aby skonfigurować pojedyncze logowanie.

2. Dodaj następujące metadane. Zalecamy pominąć wszystkie pola opcjonalne i nie zmieniać żadnych wartości domyślnych.

#### Specyfikacje (metadane)

|  |  |
| --- | --- |
| **Protokół** | SAML 2.0 |
| **Powiązanie** | Przekierowanie HTTP dla dostawcy usługi do IdP HTTP Post dla IdP do dostawcy usługi |
| **Adres URL usługi** (URL inicjowany przez dostawcę usługi)  Inne nazwy: URL uruchamiania, URL odpowiedzi, URL pojedynczego logowania jednostki uzależnionej, docelowy URL, URL pojedynczego logowania, URL punktu końcowego dostawcy tożsamości itp. | https://miro.com/sso/saml |
| **URL usługi konsumenta potwierdzenia**   Inne nazwy: dozwolony URL wywołania zwrotnego, niestandardowy URL ACS, URL odpowiedzi | https://miro.com/sso/saml |
| **Identyfikator jednostki**   Inne nazwy: identyfikator, identyfikator zaufania strony uzależnionej | https://miro.com/ |
| **Domyślny stan przekazywania** | musi być pozostawiony *pusty* w konfiguracji |
| **[Wymogi podpisywania](https://developers.onelogin.com/saml/examples/response)** | Niepodpisana odpowiedź SAML z *podpisaną* asercją  Podpisana odpowiedź SAML z *podpisaną* asercją |
| **Metoda SubjectConfirmation** | „urn:oasis:names:tc:SAML:2.0:cm:bearer” |
| Odpowiedź SAML dostawcy tożsamości musi zawierać **certyfikat klucza x509** wydany przez dostawcę tożsamości.  Wyświetl szczegółowe [przykłady SAML](https://www.samltool.com/generic_sso_res.php). Pobierz [plik metadanych Miro SP](https://drive.google.com/file/d/1BN58fiwC062F5MC-PsO3QN7JlCbKNCSJ/view) (XML). | |

:::warning
Szyfrowanie i pojedyncze wylogowanie nie są obsługiwane.
:::

#### Dane dostępowe użytkownika

Wszelkie dodatkowe pola poza poniższym nie są wymagane. Zalecamy pominąć wszystkie pola opcjonalne i nie zmieniać żadnych wartości domyślnych.

|  |  |
| --- | --- |
| Wymagane atrybuty danych logowania użytkownika | |
| **NameID**(równa się adresowi e-mail użytkownika)  Inne nazwy: SAML_Subject, klucz podstawowy, nazwa logowania, format nazwy użytkownika aplikacji itp. | &lt;NameID Format="urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress"&gt; |
| **Opcjonalne atrybuty do wysłania z asercją**  (aktualizowane przy każdym nowym uwierzytelnianiu za pośrednictwem SSO; używane w przypadku dostępności) | - „DisplayName” lub „http://schemas.microsoft.com/identity/claims/displayname” (używana jako preferowana nazwa)   [mceclip0.png](http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname)   - „FirstName”, „GivenName” lub „http://schemas.xmlsoap.org/ws/2005/05/identity/claims/givenname”; - „LastName”, „Surname” lub „http://schemas.xmlsoap.org/ws/2005/05/identity/claims/surname”; - „ProfilePicture” – zakodowany adres URL obrazu |

### Włączanie SSO w ustawieniach Miro

:::note
Włączenie pojedynczego logowania w ustawieniach nie włącza go natychmiast dla użytkowników. Pojedyncze logowanie będzie dostępne dopiero po zweryfikowaniu domen.
:::

Wersja Business Wersja Enterprise

1. Kliknij kolejno **ustawienia firmy** > **Bezpieczeństwo** > **Pojedyncze logowanie**.
2. Włącz przełącznik **SSO/SAML.

![Single-sign-on-settings-Business-Plan.png](https://help.miro.com/hc/article_attachments/14379133186834)**

1. Kliknij kolejno **Ustawienia firmy** > **Bezpieczeństwo i zgodność** > **Uwierzytelnianie** > **Pojedyncze logowanie**.
2. Włącz przełącznik **SSO/SAML.

![authentication_sso_enable.png](https://help.miro.com/hc/article_attachments/12810848670994)**

Konfigurowanie SSO w ustawieniach Miro

Po włączeniu funkcji SSO/SAML w ustawieniach pojedynczego logowania wypełnij poniższe pola:

1. **Adres URL logowania SAML** (w większości przypadków otwiera stronę dostawcy tożsamości, na której użytkownicy mają wprowadzić swoje dane logowania).
2. **Certyfikat klucza publicznego x.509** (wydany przez dostawcę tożsamości).
3. Wszystkie domeny i subdomeny dozwolone lub wymagane (ACME.com lub ACME.dev.com) do uwierzytelniania za pośrednictwem serwera SAML.

![sso_auth_settings.png](https://help.miro.com/hc/article_attachments/12810834499602)*Ustawienia pojedynczego logowania Miro*

### Odnawianie certyfikatu SSO/SAML

Jeśli certyfikat klucza publicznego x.509 wygasł, pojedyncze logowanie będzie nadal działać, ale zdecydowanie zalecamy jego odnowienie, aby nadal bezpiecznie korzystać z Miro. Certyfikaty klucza publicznego x.509 zapewniają bezpieczeństwo, prywatność, autentyczność oraz integralność informacji udostępnianych między dostawcą tożsamości a Miro.

Certyfikaty te są ważne tylko przez okres, który można ustalić (i zweryfikować) u dostawcy tożsamości. Skontaktuj się z dostawcą tożsamości, aby zweryfikować datę wygaśnięcia.

W tym celu należy wykonać dwa kroki:

1. Odnów certyfikat u dostawcy tożsamości. W tym celu postępuj zgodnie z instrukcjami dostawcy.
2. Dodaj odnowiony certyfikat do konfiguracji pojedynczego logowania Miro.

#### Dodawanie odnowionych certyfikatów do Miro

:::warning
Zalecamy wymianę certyfikatu x.509 podczas mniej obciążonych okresów w organizacji (na przykład w weekend lub po godzinach pracy), ponieważ pomoże to uniknąć zakłóceń logowania.
:::

1. Kliknij kolejno **Ustawienia firmy** > **Uwierzytelnianie** > **Pojedyncze logowanie**.
2. Usuń zawartość w polu **Certyfikat klucza x.509**.
3. Wklej nowy klucz w tym polu.
4. Przewiń w dół i kliknij **Zapisz**.
   ![sso_renew_x509_cert.gif](https://help.miro.com/hc/article_attachments/13863118752274)*Odnawianie certyfikatu x.509 w Miro*

### Weryfikowanie domen pojedynczego logowania

> **Konfigurują:** administratorzy firmy.

:::tip
Domeny już zweryfikowane przez [zarządzanie domeną](../../canvas-25-admin-features/domain-control/01-domain-control.md) nie wymagają ponownej weryfikacji.
:::

Po wprowadzeniu nazwy domeny trzeba będzie ją zweryfikować. Dopóki domena nie zostanie dodana do listy domen w ustawieniach pojedynczego logowania, a następnie zweryfikowana, użytkownicy nie będą mogli korzystać z SSO. Jeśli domena nie jest zweryfikowana, w ustawieniach SSO pojawi się komunikat **ZWERYFIKUJ E-MAIL**.

![sso_verify_email.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017515386386_sso_verify_email.png)*Niezweryfikowana domena w ustawieniach pojedynczego logowania w Miro*

### Wymagania dotyczące pomyślnej weryfikacji domeny

- Weryfikację musi przeprowadzać administrator firmy. Jeśli jesteś administratorem firmy i chcesz wysłać e-mail weryfikacyjny komuś, kto **nie** jest administratorem firmy, wówczas ta osoba może przesłać Ci e-mail weryfikacyjny z linkiem potwierdzającym w celu dokończenia procesu.
- Użyty adres e-mail musi być prawdziwy, aby móc otrzymać e-maila weryfikacyjnego.
- Domeny publiczne (np. @gmail.com, @outlook.com itp.) nie są dozwolone.
- Funkcja SSO musi być włączona, a nazwa domeny dodana w ustawieniach pojedynczego logowania.

### Sposób weryfikowania domen

1. Po dodaniu domeny otworzy się wyskakujące okienko z prośbą o podanie adresu e-mail w celu weryfikacji domeny. Podaj adres e-mail w tej samej domenie, którą dodano w ustawieniach SSO, aby udowodnić, że reprezentujesz tę domenę.
2. Kliknij **Wyślij weryfikację**.
3. Otrzymasz e-maila weryfikacyjnego w ciągu 15 minut.
4. Musisz kliknąć link weryfikacyjny w wiadomości e-mail. Aby wykonać ten krok, musisz być administratorem firmy.
5. Aby zakończyć weryfikację, kliknij **Zapisz**.
6. Użytkownicy ze zweryfikowanej domeny mogą teraz logować się przez SSO.

![domain_confirmation_modal.jpg](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528384914_domain%20confirmation%20modal.jpg)
*Wyskakujące okienko weryfikacji domeny SSO*

:::tip
Jeśli zarządzasz kilkoma domenami i subdomenami (subdomeny są rozpoznawane jako oddzielne nazwy i wymagają oddzielnej weryfikacji), najpierw zweryfikuj co najmniej jedną nazwę domeny, a następnie [prześlij prośbę do zespołu pomocy](https://help.miro.com/hc/requests/new?referer=help-center-article) z pełną listą domen (muszą być oddzielone przecinkami), abyśmy potwierdzili je naraz. Jeśli masz więcej niż 10 domen, Miro zweryfikuje je dla Ciebie. Organizacje z mniej niż 10 domenami muszą dokonać weryfikacji samodzielnie. W ramach abonamentu Business można zweryfikować tylko 3 domeny.
:::

## Testowanie konfiguracji SSO

Przetestuj konfigurację pojedynczego logowania, zanim ją włączysz, aby zmniejszyć ryzyko problemów z logowaniem dla użytkowników.

1. Wykonaj powyższe kroki, aby skonfigurować ustawienia pojedynczego logowania.
2. Kliknij przycisk **Przetestuj konfigurację SSO**.
3. Przejrzyj wyniki:

- W przypadku braku problemów wyświetli się komunikat z potwierdzeniem **pomyślnie przeprowadzonego testu konfiguracji SSO**.
- Jeśli wykryte zostaną problemy, wyświetli się komunikat z potwierdzeniem **niepowodzenia testu konfiguracji SSO**, a następnie pojawią się szczegółowe komunikaty o błędach wskazujące na to, co należy naprawić.

![Testing-SSO-configuraton.png](https://help.miro.com/hc/article_attachments/18968510419858)
*Testowanie konfiguracji pojedynczego logowania*

## Opcjonalne zaawansowane ustawienia SSO

Sekcja ustawień opcjonalnych jest przeznaczona dla użytkowników zaawansowanych, którzy mają wiedzę na temat konfiguracji SSO.

### Usługa udostępniania Just-in-Time dla nowych użytkowników

Ułatw użytkownikom rozpoczęcie korzystania z Miro od razu, bez konieczności oczekiwania na zaproszenie lub przechodzenia przez długi proces wdrażania. Upewnij się, że bezpłatne zespoły nie są tworzone poza zarządzaną subskrypcją (wymagane jest zarządzanie domeną). Pojedyncze logowanie jest wymagane, aby móc włączyć usługę udostępniania Just-in-Time dla nowych użytkowników. Wszyscy użytkownicy zatwierdzeni w ramach JIT mają przydzieloną domyślną licencję subskrypcji:

|  |  |  |
| --- | --- | --- |
| **Typ subskrypcji** | **Typ licencji** | **Działanie po wyczerpaniu licencji** |
| Wersja Business | Pełna | Użytkownicy nie są automatycznie dodawani, a funkcja JIT przestaje działać |
| Wersja Enterprise (bez [programu licencji elastycznych](../../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)) | Pełna | Użytkownicy korzystają z usługi w ramach [bezpłatnej ograniczonej](../../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) licencji |
| Wersja Enterprise (z programem licencji elastycznych) | Bezpłatna lub bezpłatna ograniczona | Zależy od ustawień [domyślnej licencji](../../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md) |

### Włączanie usługi udostępniania Just-in-Time

Po aktywacji usługi udostępniania Just-in-Time zostanie ona automatycznie zastosowana do wszystkich nowych użytkowników, którzy zarejestrują się w Miro. Natomiast istniejący użytkownicy Miro nadal będą potrzebować zaproszenia, aby dołączyć do Twojego abonamentu.

1. Przejdź do ustawień SSO.
2. Zaznacz pole **Automatycznie dodawaj wszystkich nowo zarejestrowanych użytkowników z domen z listy do swojego konta Enterprise**.
3. **Wybierz domyślny zespół dla nowo zarejestrowanych użytkowników** z listy rozwijanej.
4. Kliknij **Zapisz**.

Po dodaniu określonych domen w ustawieniach pojedynczego logowania wszyscy użytkownicy, którzy zarejestrują się za pomocą adresów w tych domenach, zostaną automatycznie dodani do subskrypcji Enterprise. Użytkownicy zostaną przypisani do zespołu wybranego w ustawieniach Just-in-Time (JIT).

![Copy of user_provisioning_jit_provisioning.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21017528391698_Copy%20of%20user_provisioning_jit_provisioning.png)*Włączanie usługi udostępniania Just-in-Time na stronie integracji Enterprise*

Wszyscy *nowo zarejestrowani użytkownicy* z domen wymienionych w ustawieniach zostaną automatycznie dodani w ramach wersji Enterprise do **tego****konkretnego zespołu**po zarejestrowaniu się w Miro.

:::warning
W wersji Enterprise ten zespół będzie również wyświetlany na liście zespołów możliwych do wyszukania, jeśli włączysz opcję [Zespół możliwy do wyszukania](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md).
:::

### Ustawienie DisplayName jako domyślnej nazwy użytkownika

Domyślnie Miro będzie używać atrybutów **FirstName** + **LastName**. Możesz też poprosić o użycie **DisplayName**. W takim przypadku Miro zastosuje **DisplayName**, *jeśli atrybut jest obecny* w odpowiedzi SAML użytkownika.

Jeśli atrybut **DisplayName** nie jest obecny, ale **FirstName** + **LastName** są, Miro użyje atrybutów **FirstName** + **LastName.** Skontaktuj się z zespołem pomocy Miro, aby ustawić **DisplayName** jako preferowaną nazwę użytkownika SSO.

Jeśli żaden z tych trzech atrybutów nie jest obecny w komunikacji SAML, Miro wyświetli adres e-mail użytkownika jako nazwę użytkownika.

|  |  |
| --- | --- |
| **Ustawienie** | **Domyślna nazwa użytkownika** |
| Nazwa użytkownika Miro | FirstName + LastName |
| Ustawienie alternatywne | DisplayName (jeśli występuje w żądaniu SAML użytkownika) |
| Ustawienie rezerwowe | FirstName + LastName (jeśli atrybut DisplayName nie jest obecny) |
| Preferowana nazwa użytkownika SSO | DisplayName ([skontaktuj się z zespołem pomocy Miro](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md)) |
| Brak atrybutów | Adres e-mail wyświetlany jako nazwa użytkownika |

Jeśli widzisz inne informacje, możliwe, że jest konieczne uwierzytelnienie przez SSO. Możliwe również, że odpowiedź SAML nie zawiera wartości potrzebnych do aktualizacji.

### Synchronizowanie zdjęć profilowych użytkownika z IdP

:::warning
Zalecamy włączyć tę opcję, jeśli nie włączasz SCIM lub Twój dostawca tożsamości nie obsługuje atrybutu **ProfilePicture**(na przykład **ProfilePicture** nie jest obsługiwany przez platformę Azure). W innych przypadkach zaleca się przesyłanie **ProfilePicture** przez [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) z natychmiastowymi aktualizacjami.
:::

Gdy to ustawienie jest włączone:

- Zdjęcie profilowe skonfigurowane po stronie dostawcy tożsamości zostanie ustawione jako zdjęcie profilowe w profilu Miro użytkownika.
- Użytkownicy nie mogą samodzielnie aktualizować ani usuwać swoich zdjęć profilowych.

Podobnie jak w przypadku atrybutu nazwy użytkownika użytkownicy nie będą mogli natychmiast zmienić swoich danych w Miro, a *synchronizacja* danych nie jest natychmiastowa. Strona dostawcy tożsamości wysyła aktualizację do Miro dopiero podczas *następnego* uwierzytelnienia użytkownika przez SSO (pod warunkiem, że ustawienie „Synchronizuj zdjęcia profilowe użytkowników z dostawcą tożsamości” jest nadal aktywne w danej chwili).

Jeśli zdjęcie profilowe jest ustawione u dostawcy tożsamości i chcesz, aby atrybut został przekazany w komunikacji SAML, Miro będzie oczekiwać następującego schematu:

```
<saml2:Attribute Name="ProfilePicture" NameFormat="urn:oasis:names:tc:SAML:2.0:attrname-format:uri">
<saml2:AttributeValue
xmlns:xs="http://www.w3.org/2001/XMLSchema"
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:type="xs:string">https://images.app.goo.gl/cfdeBqKfDKsap1icxecsaHF
</saml2:AttributeValue>
</saml2:Attribute>
```

### SSO z miejscem przechowywania danych

Jeśli korzystasz z [miejsca przechowywania danych Miro](../../canvas-25-admin-features/data-security/03-eu-data-center-residency.md) i masz osobny adres URL (workspacedomain.miro.com), musisz dostosować konfigurację dostawcy tożsamości.

W tym celu dodaj [ORGANIZATION_ID] do adresu URL.

Atrybut ORGANIZATION_ID znajdziesz na pulpicie Miro. Kliknij kolejno swój **Profil** w prawym górnym rogu > **Ustawienia** >a atrybut jest widoczny na pasku adresu URL.

|  | Wartość standardowa | Wartość w ramach miejsca przechowywania danych |
| --- | --- | --- |
| **URL usługi konsumenta potwierdzenia** (inne nazwy: dozwolony URL wywołania zwrotnego, niestandardowy URL ACS, URL odpowiedzi): | https://miro.com/sso/saml | https://workspace-domain.miro.com/ sso/saml/ORGANIZATION_ID |
| **Identyfikator jednostki**(identyfikator, identyfikator zaufania strony uzależnionej): https://miro.com/ | https://miro.com/ | https://workspace-domain.miro.com/ ORGANIZATION_ID |

### Konfigurowanie uwierzytelniania wieloskładnikowego (2FA) dla użytkowników spoza SSO

Uwierzytelnianie dwuskładnikowe (2FA) stanowi dodatkową warstwę zabezpieczeń. W przypadku korzystania z 2FA użytkownicy muszą wykonać jeszcze jeden krok podczas logowania, aby zweryfikować swoją tożsamość. To dodatkowe zabezpieczenie gwarantuje, że tylko upoważnione osoby mają dostęp do subskrypcji.
Więcej informacji zawiera nasz [przewodnik dla administratora na temat uwierzytelniania dwuskładnikowego](../../security-integrations/two-factor-authentication-2fa/01-enterprise-two-factor-authentication-2fa-–-admin-guide.md).

## Rozwiązywanie możliwych problemów

Moje adresy domeny nie są akceptowane w ustawieniach SSO i wyświetla się komunikat o zajętej domenie.

Ze względów bezpieczeństwa obsługujemy tylko domeny organizacji tylko w ramach *jednego konta firmowego (subskrypcja Enterprise)*. Możliwe, że Twoje domeny są już skonfigurowane w ramach innego abonamentu Business lub [Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md), co uniemożliwia włączenie SSO dla żądanej domeny. Sprawdź tę kwestię najpierw ze współpracownikami.

Po kliknięciu linku podanego w e-mailu weryfikacyjnym domeny nie mogę przeprowadzić weryfikacji.

Link powinien przekierowywać na stronę **integracji Enterprise**. Jeśli tak się nie dzieje, sprawdź, czy używasz oprogramowania antyphishingowego, które może przerywać przepływ danych. Upewnij się również, że jesteś administratorem firmy w Miro w momencie kliknięcia linku. Tylko administratorzy firmy mogą uzyskiwać dostęp do stron ustawień.

Musimy zmienić adresy e-mail naszych użytkowników. / Zmieniliśmy adresy e-mail naszych użytkowników, a teraz nie mają oni dostępu do swoich tablic.

Jeśli Twoja firma zmienia nazwę domeny i dlatego trzeba zmienić dane logowania pojedynczego dla adresów e-mail użytkowników, [skontaktuj się z naszym zespołem pomocy](https://help.miro.com/hc/requests/new?referer=help-center-article).

Chcemy używać oddzielnej bramki (np. MFA takiej jak Duo Dag) dla procedury pojedynczego logowania.

Takie rozwiązanie jest możliwe. Miro będzie obsługiwać preferowane rozwiązanie, jeśli działa ono w ramach SAML 2.0.

Włączyliśmy pojedyncze logowanie, ale dane profili użytkowników (imiona i nazwiska, zdjęcia profilowe, jeśli są one obsługiwane przez dostawcę tożsamości) w Miro nie są synchronizowane z danymi dostawcy tożsamości.

Nazwa użytkownika Miro i jego zdjęcie profilowe są aktualizowane po każdym pomyślnym uwierzytelnieniu użytkownika, *jeśli* SAMLResponse zawiera nowe niepuste wartości. Aby dowiedzieć się więcej o konfigurowaniu nazwy użytkownika w Miro, przeczytaj informacje o zaawansowanych ustawieniach opcjonalnych pojedynczego logowania.

Jeśli jeden lub wszyscy użytkownicy napotkają błąd podczas próby zalogowania się do Miro, zapoznaj się z [tą listą typowych błędów](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md) oraz ich rozwiązań.
