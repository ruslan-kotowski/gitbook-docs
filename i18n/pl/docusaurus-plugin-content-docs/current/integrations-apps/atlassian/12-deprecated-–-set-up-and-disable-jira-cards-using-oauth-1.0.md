---
title: Wycofany – Skonfiguruj i wyłącz karty Jira za pomocą OAuth 1.0
article_id: 360019501754
translation_id: 26579009493778
locale: pl-pl
sidebar_position: 14
created_at: '2025-05-08T15:34:56Z'
updated_at: '2025-11-25T16:03:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Dostępne dla: Jira Cloud, Jira Server (On-Premise) i Datacenter (również
    chroniony przez LDAP) Konfiguracja: Administrator zespołu Miro i administrator
    systemu Jira z uprawnieniami administracyjnymi projektu'
---

:::note
Następująca metoda uwierzytelniania OAuth1.0 nie będzie już wspierana w Miro począwszy od 31 lipca 2025 roku. OAuth1.0 to [wycofany protokół uwierzytelniania w Jira](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively.) i nie powinien być używany. Zmiana ta jest częścią szerszego przejścia na OAuth2.0, które jest zalecane zgodnie z najlepszymi praktykami w zakresie bezpieczeństwa. Użytkownikom zaleca się migrację do OAuth2.0, aby zapewnić ciągłe wsparcie i kompatybilność z usługami Miro.
:::

## Konfigurowanie Miro w Jira

:::warning
W przypadku wystąpienia problemów technicznych zapoznaj się z naszym artykułem na temat [Possible issues and how to resolve them">możliwych problemów i sposobów ich rozwiązywania](https://help.miro.com/hc/articles/360017572654).
:::

:::tip
Dowiedz się więcej o kartach Jira w artykułach [FAQ dotyczące kart Jira](https://help.miro.com/hc/articles/360013463739) oraz [Jak skonfigurować webhook dla kart Jira](https://help.miro.com/hc/articles/360017731113).
:::

Konfiguracja Jira Cloud Jira Server i Jira Data Center

:::note
Pamiętaj, żemenu Jira mogą się różnićw zależności od wersji Jira, którą używasz, jednak ogólny przebieg powinien być taki sam. Instrukcje poniżej można również znaleźć w [pomocy Atlassian](https://confluence.atlassian.com/adminjiraserver071/using-applinks-to-link-to-other-applications-802592232.html).
:::

### Krok 1 - Link do aplikacji

Najpierw utwórz link do aplikacji i skonfiguruj go.

1. Przejdź do **ustawień Jira** > **Produkty** > **Integracje** > **Łącza aplikacji** > **Utwórz łącze:
   ![mceclip1.png](https://help.miro.com/hc/article_attachments/26579015222418)***Zauważ, że interfejs Jira może się różnić w zależności od wersji Jira*
2. Wybierz **Bezpośredni link do aplikacji** i wprowadź `https://miro.com/` w polu **Adres URL aplikacji**.
   Ważne: musisz podać URL w dokładnie takim formacie. Kliknij **Kontynuuj**.
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)
    *Tworzenie linku*
3. W następnym menu, po prostu kliknij ponownie **Kontynuuj**.
4. W menu **Link do przeglądu** upewnij się, że URL nadal jest dokładnie `https://miro.com/`, a następnie wprowadź **nazwę aplikacji** według własnego wyboru. Przewiń w dół, a na dole zaznacz pole **Utwórz link przychodzący**. *Pomiń resztę pól* i kliknij **Kontynuuj**.
   ![mceclip3.png](../../../../../../docs/integrations-apps/atlassian/images/21017004819346_mceclip3.png)  *Tylko pole z nazwą aplikacji musi być wypełnione*
5. Tutaj zobaczysz pola dla wartości Miro. Aby uzyskać wartości, zaloguj się do Miro.
   - Aby zintegrować się na poziomie zespołu, przejdź do **[ustawień zespołu](https://help.miro.com/hc/articles/360021841280)** > **Aplikacje i integracje** > **Karty Jira.**
   - Aby zintegrować na poziomie organizacyjnym, przejdź do [**Ustawienia firmy**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **Aplikacje** > **Zarządzaj aplikacjami** > **Karty Jira** > **Ustawienia**.
     > Jeśli nie masz kart Jira na swojej liście aplikacji, przewiń do góry sekcji, kliknij **Zainstaluj aplikacje**, a następnie zainstaluj aplikację z Miro Marketplace. Po zobaczeniu kart Jira na liście kliknij, aby ją otworzyć.


     Karta wtyczki zostanie otwarta i zobaczysz **Krok 1**, aby uzyskać wymagane wartości:

     ![Jira_Cards_values.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017515668626_Jira Cards values.jpg)*Wartości kart Jira*
     Skopiuj wartości i dodaj je do menu Atlassian **Review Link**.
6. Przez chwilę lub dwie zobaczysz wiadomość o przetwarzaniu:
   ![mceclip4.png](../../../../../../docs/integrations-apps/atlassian/images/21017528655634_mceclip4.png)
    *Ostatni krok tworzenia linku*

To kończy kroki po stronie Atlassian. Link pojawi się na liście Twoich linków do aplikacji.

### Krok 2 - Połączenie

Wróć do ustawień karty Jira w Miro i wybierz jedną z dwóch opcji: utwórz webhook ręcznie lub automatycznie. Jeśli wybierzesz ręcznie, odznacz tę opcję. Więcej informacji znajdziesz w [tym artykule](https://help.miro.com/hc/articles/360017731113). Zdecydowanie zalecamy użycie automatycznego webhooku, aby nie musieć go resetować w przypadku dużych aktualizacji do pluginu.

Na koniec wprowadź adres URL Jira i kliknij **Połącz:**

![step_2.jpg](https://help.miro.com/hc/article_attachments/26579015236114)*Łączenie kart Jira*

Aby uzyskać adres URL Jira, skopiuj podstawowy adres URL swojej instancji Jira. Akceptujemy następujące formaty:

`https://your-server.example.com/`
[https://your-server.example.com/
https://your-ip-address/](https://your-server.example.com/)[https://your-ip-address/](https://your-server.example.com/)

Jeśli Twój URL Jira nie jest akceptowany, proszę zapoznać się z [tym artykułem.](https://help.miro.com/hc/articles/360017572654) Proszę również sprawdzić, czy Miro ma wystarczający dostęp do Twojego Jira, aby [nawiązać połączenie.](https://help.miro.com/hc/articles/360017572694)

Teraz połączyłeś swoją instancję Jira z zespołem Miro.

:::warning
Podczas gdy Atlassian przestaje wspierać Jira Server z dniem lutego 2024 roku, Miro będzie nadal wspierać integrację kart Jira dla Jira Server w dającej się przewidzieć przyszłości.
:::

1. Przejdź do `https://your-jira-server/plugins/servlet/applinks/listApplicationLinks`[.](https://your-jira-server/plugins/servlet/applinks/listApplicationLinks) Jeśli „Linki aplikacji” nie są wybrane, kliknij je. ![jira_server_create_application_links.png](../../../../../../docs/integrations-apps/atlassian/images/21017515683858_jira_server_create_application_links.png)*Łącza aplikacji Jira Server*
2. Kliknij **Utwórz link**. Wybierz „produkt Atlassian” i podaj **URL aplikacji**, „https://miro.com”. Kliknij **Kontynuuj**. ![jira_server_create_link.png](https://help.miro.com/hc/article_attachments/26579009481618)*Konfigurowanie adresu URL aplikacji*
3. Zostaniesz przeniesiony do okna dialogowego „Połącz aplikacje”. Dodaj **nazwę aplikacji** (np. Miro karta Jira) i wybierz "Generyczna aplikacja" dla **typu aplikacji**.
   Powinieneś zobaczyć swój URL aplikacji Jira pod "Tworzysz link z:", a `https://miro.com` pod "Do tej aplikacji:". Kliknij **Kontynuuj**.![jira_server_link_applications.jpg](https://help.miro.com/hc/article_attachments/26579015241490)*Konfigurowanie szczegółów aplikacji Link*
4. Konfiguracja linku zostanie przetworzona. Po zakończeniu zobaczysz swój nowy link w obszarze "Application links" serwera Jira. ![jira_server_application_links_created.png](https://help.miro.com/hc/article_attachments/26579009486226)*Twoja skonfigurowana aplikacja w Jira Server*
5. Następnie musisz skonfigurować szczegóły swojej aplikacji. Kliknij ikonę ołówka przy swojej aplikacji, aby edytować szczegóły aplikacji.
6. W oknie dialogowym Konfiguracja kliknij opcję **Uwierzytelnianie przychodzące**. Wypełnij **Consumer Key, Consumer Name, Public Key**, a opcjonalnie dodaj opis.
   - Dla integracji na poziomie zespołu, te informacje są dostępne w [**Ustawienia zespołu**](https://help.miro.com/hc/articles/360021841280) > **Aplikacje i integracje** > **Karty Jira**.
   - W przypadku integracji na poziomie organizacji te informacje są dostępne pod adresem [**Company settings**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **Aplikacje** > **Zarządzaj aplikacjami** > **Karty Jira** > **Ustawienia**.
     ![jira_server_config_oauth.png](https://help.miro.com/hc/article_attachments/26579015243666)*Konfigurowanie szczegółów uwierzytelniania przychodzącego w Jira Server*
     ![jira_webhooks_jira_server_config.png](https://help.miro.com/hc/article_attachments/26579015245842)*Szczegóły linku aplikacji Jira w Miro*
7. Przewiń do końca opcji uwierzytelniania przychodzącego i kliknij **Zapisz**. Twój status weryfikacji powinien być teraz potwierdzony, a ten serwer Jira może być teraz używany w Miro do korzystania z kart Jira. Upewnij się, że po stronie Miro wybierzesz "Jira Server" i "OAuth 1.0".![jira_server_welcome_to_jira.png](https://help.miro.com/hc/article_attachments/26579009491858)

### Autoryzacja użytkownika

Po połączeniu integracji, każdy z końcowych użytkowników musi połączyć swój osobisty profil Jira, aby ustanowić odpowiednie uprawnienia - zapewnia to, że dostęp każdego użytkownika po stronie Miro jest *dokładnie taki sam, jak po stronie Twojej instancji Jira*. Gdy użytkownicy próbują po raz pierwszy zaimportować lub edytować kartę Jira, zostaną poproszeni o zalogowanie się do Jira za pomocą indywidualnych danych dostępowych.

Po zakończeniu użytkownicy mogą dodawać zadania jako karty na tablicy. Wszystkie zmiany wprowadzone w Jirze są odzwierciedlane na kartach Jira na tablicy.

> Jeśli użytkownik nie posiada danych dostępowych do Jira, ale ma dostęp do tablicy, na której dodano kartę, zobaczy tytuł karty, typ zgłoszenia, priorytet, osobę przypisaną oraz wszystkie atrybuty skonfigurowane do wyświetlania na karcie Jira. Jednak nie będą mogli rozwinąć karty, aby zobaczyć inne atrybuty i je edytować, chyba że się autoryzują. Jeśli użytkownik nie połączy swoich danych dostępowych Jira, nie zobaczy awatara osoby przypisanej, a ogólny wygląd karty będzie inny.

### Używanie jednej instancji Jira dla kilku zespołów Miro

Możesz zainstalować karty na poziomie zespołu lub na poziomie organizacji. Jeśli masz wiele zespołów, możesz skorzystać z ustawień organizacyjnych, aby uniknąć powtarzania procedury konfiguracji dla każdego zespołu. Istniejące łącze aplikacji jest używane przez wszystkie zespoły.

Po połączeniu zespołu lub organizacji z instancją Jira, nowy webhook jest tworzony w Twoich webhookach Jira dla danego zespołu lub organizacji w Miro. Utworzenie webhooka ustanawia kanał dla próśb o aktualizację.

Jeśli określisz ustawienia na poziomie organizacji, zespoły, które już są połączone, zachowają swoje bieżące ustawienia. Jednak mogą w każdej chwili przełączyć się na ustawienia na poziomie organizacji.

Dodatkowo, w razie potrzeby zespoły mogą zastąpić ustawienia na poziomie organizacji, aby połączyć się z inną instancją Jira.

Jeśli jesteś klientem Enterprise, który chce przenieść wiele połączeń na poziomie zespołu do domyślnego połączenia na poziomie organizacji, skontaktuj się ze swoim zespołem konta.

:::warning
Jeśli chcesz połączyć kilka zespołów osobno, zalecamy nadanie webhookowi dla każdego zespołu unikalnej nazwy. Przejdź do strony webhooków Jira i edytuj każdy nowo utworzony webhook.
:::

Łączenie kilku instancji Jira z jednym zespołem Miro nie jest obsługiwane.

## Wyłączanie wtyczki

Aby zintegrować na poziomie zespołu, przejdź do **Ustawienia zespołu** > **Aplikacje i integracje** > **Karty Jira**. Następnie wybierz **Usuń z zespołu**.

Aby ograniczyć użycie aplikacji Jira na poziomie organizacji, przejdź do **Ustawienia firmy** > **Aplikacje** > **Zarządzaj aplikacjami** > **Karty Jira**. Następnie przesuń przełącznik do pozycji wyłączonej.

:::warning
Jeśli wyłączysz Jirę dla organizacji, użytkownicy ze wszystkich zespołów Enterprise nie będą mogli korzystać z kart Jira. Aby dowiedzieć się więcej o zarządzaniu aplikacjami i ich ograniczaniu, zobacz [zarządzanie aplikacjami](https://help.miro.com/hc/articles/4404659741458).
:::

**Więcej informacji:** Zobacz [Jak używać kart Jira](https://help.miro.com/hc/articles/360017572434).
