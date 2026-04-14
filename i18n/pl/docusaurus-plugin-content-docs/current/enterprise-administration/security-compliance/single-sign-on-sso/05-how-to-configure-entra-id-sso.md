---
title: Jak skonfigurować SSO Entra ID
article_id: 360022722233
translation_id: 360022722233
locale: pl-pl
sidebar_position: 5
created_at: '2019-05-07T12:03:08Z'
updated_at: '2025-11-25T16:04:59Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Dostępne w wersjach: Wersja Business, wersja Enterprise Wymagana rola: Administratorzy
    firmy'
---

> *💡 Zdecydowanie zaleca się konfigurowanie SSO w oddzielnym oknie przeglądarki w trybie incognito.* Dzięki temu utrzymasz sesję w standardowym oknie, co pozwoli Ci wyłączyć autoryzację SSO w przypadku błędnej konfiguracji.

Jeśli chcesz skonfigurować instancję testową przed włączeniem SSO na produkcji, proszę [skontaktuj się z zespołem pomocy](https://help.miro.com/hc/requests/new?referer=help-center-article). Tylko osoby, które skonfigurują SSO, zostaną dodane do tej instancji testowej.

> **⚠️ Zobacz nasz główny artykuł o SSO** [**tutaj**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) **aby zapoznać się z zasadami, obsługiwanymi funkcjami i opcjonalną konfiguracją po stronie Miro.**

## Dodawanie i konfigurowanie aplikacji

 1. Znajdź wstępnie skonfigurowaną aplikację Miro w galerii aplikacji Enterprise Entra ID ([Aplikacje dla przedsiębiorstw](https://portal.Entra.com/#blade/Microsoft_AAD_IAM/StartboardApplicationsMenuBlade/AllApps/menuId/) > +Nowa Aplikacja).

2. Utwórz aplikację i kliknij **2.** **Skonfiguruj pojedyncze logowanie** (lub wybierz **Pojedyncze logowanie** z lewej strony i wybierz metodę logowania **SAML**).

3. Zobaczysz, że **podstawowa konfiguracja SAML** jest już gotowa:

:::warning
jeśli po skonfigurowaniu wszystkiego logowanie przez SSO się nie powiedzie, spróbuj zmienić Entity ID z `https://miro.com`na `https://miro.com/`
:::

:::warning
Adres URL logowania, Relay State i adres URL wylogowania (dla pojedynczego wylogowania) muszą pozostać puste, ponieważ te funkcje nie są obsługiwane.
:::

**Atrybuty i roszczenia** są również już gotowe:

:::warning
Pamiętaj, że:
a) UPN stanie się głównym parametrem, na podstawie którego użytkownik w Miro będzie rozpoznawany i ten parametr nie będzie mógł być aktualizowany po stronie Entra. Gdy potrzebujesz zaktualizować adresy e-mail użytkowników w Miro bez użycia SCIM, prosimy [skontaktować się z naszym zespołem pomocy](https://help.miro.com/hc/requests/new?referer=help-center-article).
b) Miro zaakceptuje [**GivenName,** **Surname,** **DisplayName** oraz **ProfilePicture**](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md). Inne atrybuty nie są obsługiwane przez SSO, ale mogą być przekazywane przez [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).
:::

### Tworzenie certyfikatu

1. W Microsoft Entra upewnij się, że **certyfikat podpisywania SAML** >**Opcja podpisywania** to albo **Podpisz asercję SAML**, albo **Podpisz odpowiedź i asercję SAML**.

2. **Pobierz** plik **Base64**.

## Konfigurowanie SSO w Twojej wersji Miro

1. Otwórz pobrany plik **Base64** w edytorze tekstowym, a następnie skopiuj certyfikat **x509** z pliku.

2. W Miro, w sekcji **Bezpieczeństwo > Uwierzytelnianie**, wklej skopiowany certyfikat **x509** do pola **Certyfikat klucza x509**.

3. W ustawieniach Microsoft Entra skopiuj **Login URL**, a następnie przejdź do strony **Bezpieczeństwo > Uwierzytelnianie** w Miro i wklej go do pola **SAML Sign-in URL**.

4. Na stronie **Bezpieczeństwo >**  **Uwierzytelnianie** w Miro, w sekcji **Użytkownicy z tych domen będą się logować przez SSO**, upewnij się, że dodasz co najmniej jedną domenę firmy.

:::warning
W Miro upewnij się, że opcja **Synchronizacja zdjęć profilowych z dostawcą tożsamości** nie jest zaznaczona. Entra ID nie obsługuje synchronizacji zdjęć profilowych użytkowników. Kiedy opcja **Synchronizacja zdjęć profilowych z dostawcą tożsamości** nie jest zaznaczona, użytkownicy mogą ustawiać własne zdjęcia profilowe.
:::

5. Kliknij **Zapisz**.

Twoja konfiguracja SSO jest teraz zakończona.

## Konfigurowanie roszczeń, gdy UPN i e-mail różnią się

Możesz skonfigurować ustawienia, aby używać dowolnego atrybutu Entra w formacie e-mail jako **NameID** w Miro.

### Logowania, które inicjuje dostawca tożsamości (IdP) i dostawca usługi (SP)

*W przypadku logowania inicjowanego przez dostawcę tożsamości (IdP)*, Entra przesyła Miro wartość, którą zdecydujesz się użyć jako **NameID** (**user.mail** w poniższym przykładzie).

W tym przepływie, twoi użytkownicy końcowi uzyskują dostęp do Miro przez ikonę na swojej konsoli portalu (na przykład na stronie `https://myapplications.microsoft.com/`). Stamtąd do Miro jest wysyłana prośba i *użytkownik jest logowany z użyciem **NameID**, które zdefiniowałeś.*Miro będzie oczekiwać, że ten atrybut będzie zgodny z **e-mailem** użytkownika w Miro. Niezgodność spowoduje niepowodzenie uwierzytelniania.

*W przypadku logowania inicjowanego przez dostawcę usługi (SP)*, Miro wyśle prośbę specjalnie o **UPN** użytkownika i będzie oczekiwać, że będzie on zgodny z **e-mailem** użytkownika w Miro. Niezgodność spowoduje niepowodzenie uwierzytelniania.

Teraz pole **URL logowania SAML** w ustawieniach Miro powinno zawierać **URL logowania** aplikacji Miro twojej instancji Entra. To będzie URL, na który Miro przekieruje użytkownika ze [strony logowania Miro](https://miro.com/sso/login/).

Gdy użytkownik zostanie przekierowany na URL logowania z aplikacji, generowane jest żądanie SAML. W ramach tego przepływu użytkownik loguje się z adresem e-mail, który wprowadził na stronie logowania Miro i który Miro następnie pozyskuje od Entra, wymagając, aby był to atrybut UPN.

### Jak skonfigurować

Aby umożliwić użytkownikom dostęp do Miro za pomocą ich **e-maila** z Entra zamiast **UPN**, możesz wypełnić pole **URL logowania SAML** w Miro adresem URL aplikacji z konsoli Entra. Następnie przepływ inicjowanego przez dostawcę usługi (SP) będzie wyglądał następująco:

1. Użytkownik uzyskuje dostęp do Miro, wpisując swój e-mail Miro, który jest adresem e-mail, jaki ma w Miro. Miro rozumie, że osoba powinna być zalogowana do zdefiniowanego profilu użytkownika.
2. Użytkownik jest kierowany do linku aplikacji używanego do logowania inicjowanego przez dostawcę tożsamości (IdP).
3. Link wykorzystuje **NameID** atrybut *który zdefiniowałeś* i wysyła go do Miro.
4. Użytkownik jest zatem zalogowany do Miro na wcześniej zdefiniowany profil użytkownika z **NameID**, który został przez Ciebie zdefiniowany.

Jeśli chcesz także włączyć automatyczne aprowizowanie dla Miro, zajrzyj do [tego artykułu](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

Jeśli napotkasz jakiekolwiek problemy podczas konfiguracji, sprawdź [ten artykuł](../../../using-miro/tools/troubleshooting/10-i-can't-log-in-via-sso.md).

## Narzędzie testowe Entra

Aby dostać się do narzędzia testowego, wybierz kartę **Pojedyncze logowanie** w ustawieniach aplikacji i przewiń w dół do końca sekcji.

Entra sugeruje użycie procesu testowego logowania w celu sprawdzenia połączenia i rozwiązywania problemów z komunikatami o błędach. Po teście otrzymasz instrukcje dotyczące rozwiązania sytuacji.

Pamiętaj, z jakimi danymi dostępowymi zarządzanymi przez Entra/ADFS jest uwierzytelniany Twój komputer roboczy. Jeśli próbujesz użyć innego zestawu, aby zalogować się do Miro, próba logowania może się nie powieść, ponieważ dostawca tożsamości przekaże główny zestaw danych dostępowych i dojdzie do niezgodności. Na przykład, może to się zdarzyć, jeśli jesteś administratorem SSO i testujesz procedurę logowania przy użyciu innych danych dostępowych użytkownika.

## Alternatywnie możesz przetestować w Miro

1. Wykonaj powyższe kroki, aby skonfigurować ustawienia SSO.
2. Kliknij przycisk **Przetestuj konfigurację SSO**.
3. Przejrzyj wyniki:
   1. Jeśli nie zostaną znalezione żadne problemy, zostanie wyświetlony komunikat potwierdzający **pomyślne przeprowadzenie testu konfiguracji SSO**.
   2. Jeśli wykryte zostaną problemy, wyświetli się komunikat z potwierdzeniem **niepowodzenia testu konfiguracji SSO**, a następnie pojawią się szczegółowe komunikaty o błędach wskazujące na to, co należy naprawić.

##
