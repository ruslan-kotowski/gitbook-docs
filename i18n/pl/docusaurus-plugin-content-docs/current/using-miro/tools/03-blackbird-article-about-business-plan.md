---
title: "Przetestuj artyku\u0142 Balckbird dotycz\u0105cy SCIM"
article_id: 25902000474898
translation_id: 25902000474898
locale: pl-pl
sidebar_position: 3
created_at: '2025-04-08T15:00:21Z'
updated_at: '2025-05-07T11:29:05Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

!!!Test artykuł!!!

System do zarządzania tożsamościami między domenami (SCIM) umożliwia automatyzację zarządzania użytkownikami oraz aprowizację i zarządzanie między Miro a Twoim dostawcą tożsamości (IdP).

> **Dostępne w wersjach:**[abonament Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Konfigurują:** Administratorzy firmy

## Ważne informacje

- **SSO oparte na SAML musi być poprawnie skonfigurowane i działać w wersji Enterprise, zanim zaczniesz konfigurować automatyczne zarządzanie administracją.**
  Zobacz [przewodnik](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) po konfigurowaniu SAML SSO.
- **Synchronizacja grup z zespołami Miro jest opcjonalna.**
  Możesz opcjonalnie synchronizować grupy swojego dostawcy tożsamości z zespołami w Miro. Aby jednak uniknąć sytuacji, w której grupa IdP jest przypadkowo lub tymczasowo usunięta, co skutkuje dezaktywacją wszystkich użytkowników w tej grupie w Miro i uruchamia ponowne przypisanie tablic i przestrzeni, nie synchronizuj grup IdP z zespołami Miro. Zespoły mogą być tworzone i zarządzane za pomocą [Teams API](https://developers.miro.com/reference/enterprise-create-team). Aby dowiedzieć się więcej o tym, jak SCIM API umożliwia zarządzanie grupami, zobacz [Miro Developers](https://developers.miro.com/docs/groups).
- **Zmiany adresu e-mail w SCIM obejmują następujące zasady walidacji:**
  - **Sprawdzenie Zarządzanego Użytkownika:** Jeśli obecna domena użytkownika nie jest przypisana przez organizację inicjującą prośbę SCIM, aktualizacja e-mail jest blokowana i wyświetla błąd 400.
  - **Weryfikacja docelowej domeny e-mail:** Jeśli docelowa domena e-mail jest przypisana do organizacji innej niż ta, która inicjuje prośbę SCIM, aktualizacja e-maila jest blokowana i generuje błąd 400. Jeśli docelowa domena adresu e-mail jest przypisana do organizacji inicjującej prośbę SCIM, aktualizacja adresu e-mail jest dozwolona bez konieczności potwierdzania adresu e-mail. Dzienniki audytu rejestrują aktualizacje w każdej organizacji, w której użytkownik jest członkiem.
  - **Zarządzanie domeną i SSO:** Aktualizacje e-mail są dozwolone na podstawie weryfikacji domeny przez zarządzanie domeną (IDC) lub pojedyncze logowanie (SSO). Jeśli docelowa domena e-mail jest zweryfikowana przez CD lub SSO przez organizację inicjującą, aktualizacja może zostać przeprowadzona.
    ![scim-diagram-2.png](images/26547059766162_scim-diagram-2.png)
    *Diagram walidacji zmiany e-maila w przepływie pracy SCIM*

### Reguły, na podstawie których działa Miro SCIM

- Zmiany zsynchronizowane przez SCIM są przede wszystkim stosowane do nowo przypisanych użytkowników. Stan osób, które są już objęte Twoją subskrypcją, zostanie uzupełniony, ale może nie zostać nadpisany, ponieważ zmiany są stosowane na poziomie grupy lub zespołu. Na przykład:
  a) jeśli użytkownik jest uczestnikiem Team1 po stronie Miro, a dostawca tożsamości wyśle aktualizację w celu dodania go do Team2, jego stan w Team1 pozostaje nienaruszony.
  b) Jeśli Twój dostawca tożsamości wyśle aktualizację zawierającą zmiany dla użytkownika1, nie wpłynie to na innych członków zespołu. Jak wspomniano w **Obsługiwanych funkcjach** > **Synchronizuj i wypychaj grupy** do nadpisania stanu zespołu i ponownego zsynchronizowania wszystkich użytkowników jednocześnie, spróbuj zainicjować nowe wypychanie.
- Wszyscy użytkownicy zatwierdzeni w ramach SCIM mają przypisaną *domyślną licencję* Twojej subskrypcji:
  a) W przypadku subskrypcji Enterprise bez programu elastycznych licencji: pełna licencja. Jeśli w Twojej subskrypcji zabraknie licencji, użytkownicy zaczną otrzymywać licencje w ramach [bezpłatnej ograniczonej](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) licencji.
  b) W przypadku subskrypcji Enterprise z aktywowanym [">programem elastycznych licencji](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md): Licencja bezpłatna lub bezpłatna ograniczona w zależności od [domyślnej licencji subskrypcji](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).
  *- Jeśli chcesz, aby niektórzy użytkownicy byli aprowizowani na podstawie licencji innej niż domyślna:*
  *jak wspomniano powyżej, wszyscy użytkownicy są aprowizowani z domyślną licencją. Możesz jednak natychmiast zaktualizować wszystkie lub niektóre z nich, używając atrybutu **UserType** z wartością pełną. <em>Użytkownicy zaktualizowani z użyciem tego atrybutu otrzymają pełną licencję bez przestojów po stronie użytkownika.*
- Wszyscy użytkownicy zatwierdzeni w ramach SCIM również są objęci funkcją [zarządzania domeną](../../enterprise-administration/canvas-25-admin-features/domain-control/01-domain-control.md). Oznacza to, że jeśli użytkownik jest członkiem tylko jednej grupy zabezpieczeń u dostawcy tożsamości, ale ustawienia zarządzania domeną definiują 3 zespoły jako wyznaczone, użytkownik zostanie również dodany do tych 3 zespołów.
- Aby chronić usługę, Miro ogranicza liczbę połączeń API dostępnych co 30 sekund:

  | Typ prośby | Poziom limitu |
  | --- | --- |
  | GET scim/users    GET scim/users/\{userId\} | Poziom limitu pierwszej stawki 1 |
  | POST scim/users/\{userId\}    PUT scim/users/\{userId\}    POPRAWIENIE scim/users/\{userId\}    USUŃ scim/users/\{userId\} | Trzeci limit stawki – poziom 3 |
  | GET scim/Grupy    POPRAW scim/Groups/\{groupId\} | Czwarty limit stawki Poziom 4 |
  | GET scim/Grupy/\{groupId\} | Trzeci limit stawki Poziom 4 |

  Szczegółowe informacje na temat poziomów limitów można znaleźć [**tutaj.**](https://developers.miro.com/reference#ratelimiting)Jeśli liczba żądań przekroczy limit, Miro zwróci standardowy **429 Zbyt wiele żądań**.

## Obsługiwane funkcje

Szczegółowy schemat Miro SCIM można znaleźć [**tutaj**](https://developers.miro.com/docs/scim).

Miro obsługuje następujące funkcje obsługi administracyjnej:

- **Tworzenie nowych użytkowników**
  Nowi użytkownicy przypisani do aplikacji Miro przez dostawcę tożsamości (IdP) będą tworzeni w ramach Twojej subskrypcji Miro Enterprise jako uczestnicy klasy Enterprise. Użytkownicy, którzy zostali dodani do grupy użytkowników, która jest zsynchronizowana z zespołem Miro o tej samej nazwie, zostaną dodani do zespołu jako uczestnicy zespołu
- **Wysyłanie aktualizacji profilu użytkownika**
  Informacje o obsługiwanych atrybutach i zmianach znajdują się poniżej
- **Synchronizuj i wypychaj grupy**
  Synchronizuj grupy IdP i ich członków z zespołami w ramach subskrypcji Miro Enterprise, aby automatycznie zarządzać członkostwem użytkowników. Trwająca synchronizacja przekaże określone aktualizacje dotyczące użytkowników grupy do zsynchronizowanego zespołu Miro, podczas gdy wypchnięcie zastąpi stan zespołu, traktując grupę jako źródło prawdy (jeśli na końcu Miro wprowadzono jakiekolwiek zmiany manualne przez administratorów firmy).
- **Oddziel nazwy grup/zespołów**
  Miro synchronizuje grupy i zespoły po nazwie, dlatego muszą mieć dokładnie taką samą nazwę. Jednak po utworzeniu początkowej synchronizacji będziesz mógł(a) nadać jednemu lub obu z nich nazwy, które są dla Ciebie wygodne. Przykład oddzielenia można zobaczyć [tutaj](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)
- **Usuń użytkowników z grupy/zespołu (nie z subskrypcji Enterprise, patrz poniżej)**
  Usunięcie użytkownika z grupy spowoduje usunięcie go z zsynchronizowanego zespołu Miro (podczas następnego Pusha grupowego).
- **Dezaktywuj użytkowników**
  Dezaktywacja/usunięcie użytkownika lub wyłączenie dostępu użytkownika do aplikacji w ramach usługi IDP spowoduje *dezaktywację* użytkownika w Twoim abonamencie Miro Enterprise. W zależności od okoliczności dezaktywacja użytkownika może przypisać jego zawartość najstarszym administratorom zespołu:
  - jeśli dezaktywujesz użytkownika po stronie dostawcy tożsamości, ale pozostawisz go przypisanego do aplikacji Miro, członkostwo w zespole po stronie Miro nie zostanie zmienione, a zawartość nie zostanie ponownie przypisana - użytkownik zostanie po prostu przeniesiony ze stanu **Aktywny** do stanu **Dezaktywowany** (i odpowiednio do sekcji użytkowników) i przestanie korzystać z licencji.
  - jeśli aktywujesz dezaktywację, usuwając użytkownika za pomocą dostawcy tożsamości lub dezaktywując go z aplikacji Miro, gdy użytkownik jest członkiem niektórych *zsynchronizowanych* zespołów, użytkownik zostanie dodatkowo usunięty z *tych* zespołów Miro, a ich treści w tych zespołach zostaną przypisane do najstarszych administratorów zespołu.
  - jeśli uruchomisz dezaktywację, *usuwając* użytkownika u dostawcy tożsamości lub *deaktywując* go w aplikacji Miro, gdy użytkownik nie jest członkiem żadnych *zsynchronizowanych* zespołów, członkostwo w zespole nie zostanie zmienione, a jego treści nie zostaną ponownie przypisane.
  **Usuwanie użytkownika** z subskrypcji Enterprise nie jest domyślnie *obsługiwane.* Nadal możesz [ręcznie dodać funkcjonalność za pomocą API](https://developers.miro.com/docs/scim#section-delete-user-by-id), aby użytkownik został całkowicie usunięty z subskrypcji, zamiast ustawiać go na status **Dezaktywowany**. W tym scenariuszu zawartość jest ponownie przypisywana do odpowiednich członków zespołu. Nie można ustawić, którzy administratorzy otrzymają własność nad automatycznie przypisanymi treściami. Można ją jednak ustawić podczas ręcznej [dezaktywacji użytkownika w ustawieniach Miro.](../../enterprise-administration/user-management/01-deactivated-users.md)
- **Ponownie aktywuj użytkowników**
  Przypisanie użytkownika z powrotem do aplikacji lub ponowne aktywowanie profilu użytkownika u dostawcy tożsamości (IDP) spowoduje ponowną aktywację użytkownika w Twojej subskrypcji Miro Enterprise, jeśli był wcześniej aprowizowany i dezaktywowany.
- **Automatyzacja przydzielania grup rozliczeniowych**
  Automatyczne przypisywanie nowych użytkowników do [billing groups](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/01-billing-groups.md) za pomocą SCIM. Po skonfigurowaniu dostawcy tożsamości (IdP) połącz centra kosztów z grupami rozliczeniowymi. Dzięki temu każdy obecny i przyszły użytkownik z tych centrów kosztów zostaje automatycznie posortowany do odpowiedniej kategorii rozliczeniowej.

Możesz również usunąć użytkowników ze swojego abonamentu Enterprise, wysyłając bezpośrednie **usuń** połączenie API – zobacz dokumentację [tutaj](https://developers.miro.com/docs/scim#section-delete-user-by-id). Pamiętaj, że tylko *bezpośrednie* rozmowy spowodują usunięcie użytkowników. **Usuwanie** zdarzeń zainicjowanych *przez Twoje rozwiązanie tożsamości* będzie traktowane jako prośba o **dezaktywację**.

### Obsługiwane atrybuty

:::warning
Pamiętaj, że:
- **E-mail** / parametr podstawowy / unikalny identyfikator / **nazwa użytkownika**) to jedyna wartość wymagana przez Miro i musi mieć postać wiadomości e-mail.
- aktualizacja e-mail jest możliwa tylko dla już zsynchronizowanych użytkowników. Innymi słowy, pierwsza synchronizacja musi nastąpić, gdy ich adres e-mail w IdP i Miro jest taki sam, w przeciwnym razie Miro nie rozpozna użytkownika i zostanie utworzony duplikat profilu Miro pod nowym adresem e-mail.
- aktualizacja e-mail musi mieć miejsce w profilu IdP użytkownika, a nie na liście przypisów.
- W przeciwieństwie do innych atrybutów, aktualizacja **e-maila** użytkownika wyśle mu powiadomienie: zarówno stary, jak i nowy adres e-mail otrzymają wiadomość informującą użytkownika, że teraz powinien używać nowego adresu e-mail do logowania do Miro.
:::

| Nazwa atrybutu | Atrybut SCIM (roszczenie) |
| --- | --- |
| E-mail | Nazwa użytkownika  **Musi być obecny i w formacie e-mail** |
| *Atrybuty wymienione poniżej nie są wymagane i zostaną zaakceptowane przez Miro, jeśli są obecne (inne atrybuty wysłane do Miro zostaną zignorowane).* | |
| Pełna nazwa | displayName;      sformatowany;      givenName + " " + familyName;      Nazwa użytkownika |
| Typ użytkownika | użytkownikTyp       Obsługiwana wartość: Pełne |
| Aktywny | aktywny       Obsługiwana wartość: „true” lub „false” |
| Obraz profilowy | **zdjęcia.^[type=='photo'].wartość** lub     **zdjęcia.^[type==photo].wartość** (Okta)     **zdjęcia[type eq "photo"].wartość** (Entra)        Musi być tekstowym adresem URL do obrazu.        Obsługiwane typy plików: jpg, jpeg, bmp, png, gif       Aby zdefiniować typ pliku, powinieneś mieć zdefiniowane rozszerzenie pliku w url     (np. `https://host.com/avatar_user1.jpg`) lub prośba o adres URL powinna zwracać razem z zawartością pliku nagłówek Content-Type (np. Content-Type = 'image/jpeg')        Maksymalny rozmiar pliku do pobrania to: 31457280 bajtów |
| Rola użytkownika | role.^[podstawowy==true].value (Okta)      role[primary eq "True"].value (Entra)        Obsługiwane wartości:  **ORGANIZATION_INTERNAL_ADMIN** **ORGANIZATION_INTERNAL_USER** |
| Numer pracownika | pracownikNumer |
| Centrum kosztów | costCenter |
| Organizacja | Organizacja |
| Podział | Sekcja |
| Dział | Dział |
| Nazwa menedżera | manager.displayName |
| Identyfikator menedżera | manager.value  Pole "value" ma typ ciągu znaków w standardzie SCIM, ale managerId       wewnętrzne pole Miro ma typ Long. Jeśli atrybut „wartość” nie jest       Wartość liczbowa, którą ignorujemy |

:::warning
Zmiany hasła nie są obsługiwane i nie ma natychmiastowych planów rozpoczęcia obsługi tej zmiany.
⚠️ **Nazwa użytkownika**, **Typ użytkownika** i **roles.value** nie mogą być aktualizowane dla [dezaktywowanych użytkowników](../../enterprise-administration/user-management/01-deactivated-users.md).
:::

Wszystkie atrybuty będą wyświetlane na wyeksportowanej liście użytkowników CSV, którą można pobrać z sekcji [Aktywni użytkownicy](../../enterprise-administration/user-management/12-user-management-overview-on-enterprise-plan.md).

![download_as_CSV_in_company_settings.jpg](images/26547059766802_download%20as%20CSV%20in%20company%20settings.jpg)
*Opcja pobrania listy użytkowników*

![mceclip3.png](images/26547034301714_mceclip3.png)

## Konfigurowanie SCIM

### Krok 1: Włącz opcję SCIM w Miro

Aby włączyć SCIM dla abonamentu Miro Enterprise, przejdź do **ustawień firmy** > **Integracje Enterprise,** włącz funkcję obsługi administracyjnej SCIM**.</strong>** Tam możesz uzyskać podstawowy adres URL i token API do konfigurowania IdP.

![scim.png](images/26547059772818_scim.png)
*SCIM w ustawieniach Miro*

### Krok 2: Skonfiguruj swojego dostawcę tożsamości

Konfiguracja będzie zależeć od używanego dostawcy tożsamości. Miro obsługuje wstępnie skonfigurowane Okta i Entra ID, ale możesz używać dowolnego dostawcy tożsamości, o ile umożliwia on konfigurowanie SCIM.

OKTA – zobacz instrukcję konfiguracji [tutaj](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md).

Entra ID – zobacz instrukcję konfiguracji [tutaj](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

## Generuj nowy token

1. Przejdź do **ustawień firmy** > **Integracje Enterprise.**

2. W sekcji**Obsługa administracyjna SCIM** kliknij**Generuj nowy token**.

![scim.png](images/26547059772818_scim.png)
*SCIM w ustawieniach Miro*

2. W oknie **Generuj nowy token SCIM** kliknij **Generuj**.

![wygeneruj_token.png](images/26547059774994_generate_token.png)

3. Po wygenerowaniu nowego tokena, musisz skonfigurować nowy token w swoim dostawcy tożsamości.

## Możliwe problemy i sposoby ich rozwiązania

*1. Użytkownicy nie otrzymują aprowizowanych z powodu błędu listy dozwolonych.*
![mceclip0.png](images/26547034308498_mceclip0.png)
*Przykład błędu od dostawcy tożsamości Okta*

Upewnij się, że adres domeny użytkownika został dodany do listy dozwolonych [w **ustawieniach** zabezpieczeń](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

*2. Jeśli uwierzytelniasz użytkowników końcowych za pomocą jednego rozwiązania identyfikacyjnego (IDP1), ale chcesz włączyć SCIM za pomocą innego (IDP2), jest to możliwe pod dwoma warunkami:*

1. identyfikator IDP2 może wykonywać wywołania API za pomocą tokena okaziciela.
2. Obaj dostawcy tożsamości są zsynchronizowani (więc użytkownicy zaprowizowani przez SCIM również istnieją w IDP1, dzięki czemu mogą się uwierzytelniać w Miro).

Aby uzyskać więcej informacji, [skontaktuj się z zespołem pomocy technicznej Miro](https://help.miro.com/hc/en-us/requests/new?referer=help-center-article).
