---
title: "Cz\u0119sto zadawane pytania dotycz\u0105ce kart Jira"
article_id: 360013463739
translation_id: 30228782444946
locale: pl-pl
sidebar_position: 17
created_at: '2025-10-14T19:23:28Z'
updated_at: '2025-10-14T19:23:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Ten artykuł odpowiada na najczęściej zadawane pytania dotyczące tego, jak zbudowana jest nasza integracja kart Jira.

**Bezpieczeństwo**

**Jak działa uwierzytelnianie Jira-Miro?**

Zobacz artykuły w Centrum pomocy dla

- **Jira Server lokalny**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Usługi trzecie) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Data Center lokalnie**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Od strony trzeciej) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Cloud**
  Wybierz z ustawień kart Jira.
  - [OAuth 2.0](https://help.miro.com/hc/articles/8588617184402) (3LO)

**Czy dane są zabezpieczone podczas transferu między Jira a Miro?**

Używamy protokołu bezpieczeństwa TLS. Szyfruje on wiadomości HTTP przed transmisją i deszyfruje wiadomości po ich przybyciu. Wspieramy również mutual TLS dla [wersji Enterprise](https://help.miro.com/hc/articles/360017730433).

**Czy wspieracie mutual TLS?**

Tak, [dowiedz się więcej](https://help.miro.com/hc/articles/4410562720658).

**Czy Miro przechowuje dowolne dane klienta w Jira?**

Tak, Miro przechowuje dane kart, które są dodane do tablicy.

**Jak długi jest okres retencji i jak dane będą zabezpieczone?**

W przypadku OAuth 1.0 (Jira Server lub Data Center) dane są również aktualizowane, jeśli webhooks są skonfigurowane podczas procesu ustawiania wtyczki kart Jira. Okres retencji jest nieograniczony. Zastosowane są jedynie ogólne protokoły bezpieczeństwa Miro.

**Czy możemy ograniczyć informacje pobierane z Miro?**

Nie znaleźliśmy żadnej wzmianki w [dokumentacji Atlassian](https://developer.atlassian.com/server/jira/platform/webhooks/) o możliwości ograniczenia informacji do kilku pól.

**Czy możemy uzyskać diagram przedstawiający przepływ danych między Jira a Miro?**

Szczegółowe informacje można znaleźć w [artykułach dla deweloperów Jira](https://developer.atlassian.com/server/jira/platform/oauth/). Nasza integracja jest wdrażana zgodnie z dokumentacją Atlassian.

**Jak obsługiwany jest token?**

Oauth 1.0: Używany jest tylko access token. Access token pozostaje ważny [przez 5 lat chyba że](https://developer.atlassian.com/server/jira/platform/oauth) zostanie cofnięty (nie ma opcji dostosowania, ponieważ tę politykę określa Atlassian. Możesz cofnąć token po stronie Jira za pomocą interfejsu webowego). Pamiętaj, że każdy nowy token powoduje przerwanie działania integracji i konieczność [ponownego jej połączenia](https://help.miro.com/hc/articles/360019501754#Step_2_-_Connection).

OAuth 2.0: Access token jest ważny przez 1 godzinę. Refresh token jest ważny przez 90 dni (jeśli nie korzystasz z integracji przez 90 dni, będziesz musiał(a) się ponownie uwierzytelnić).

**Czy jeden access token jest używany do całego dostępu do Jira klienta?**

Każdy użytkownik Miro zamierzający importować, tworzyć lub edytować karty Jira musi połączyć swoje indywidualne dane dostępowe do Jira. Wszystkie powyższe działania mogą być wykonywane jedynie w imieniu indywidualnych danych dostępowych do Jira.

**Jak są zabezpieczane tokeny żądania, tokeny dostępu, klucze prywatne oraz inne sekrety/dane dostępowe OAuth?**

Podczas integracji używane są wyłącznie tokeny dostępu. Są one bezpiecznie przechowywane w bazie danych i wykorzystywane jedynie po stronie serwera.

Dla OAuth 1.0. (Jira Server oraz Data Center) token authToken stosowany jest wyłącznie dla webhooka. Nie jest to faktyczny token uwierzytelniający używany przez OAuth. Żądania są przesyłane przez zaszyfrowane połączenie. Klucz tajny jest generowany automatycznie i przypisany w zależności od zespołu.

**Jakie punkty końcowe wykorzystuje wasza integracja?**

```
POST /rest/api/2/issue - utworzenie nowego zgłoszenia
```

```
PUT /rest/api/2/issue/id - aktualizacja zgłoszenia
```

```
GET /rest/api/2/user/picker?query=xx
```

```
GET /rest/api/2/myself
```

```
GET /rest/api/2/filter/favourite
```

```
GET /rest/api/2/issue/picker
```

```
GET /rest/api/2/serverInfo
```

```
GET /rest/api/2/issue/$key
```

```
GET /rest/api/2/issue/createmeta
```

```
GET /rest/api/2/issue/$key/editmeta
```

```
GET /rest/api/2/priority
```

```
GET /rest/api/2/issuetype
```

```
GET /rest/api/2/mypermissions
```

Dla OAuth 1.0. (Jira Server i Data Center) dodatkowo używamy:

```
POST /rest/webhooks/1.0/webhook
```

**Czy karty będą działać z Jira Datacenter?**

Tak. Jesteśmy zatwierdzeni przez Atlassian i mamy już wielu klientów, którzy z powodzeniem używają kart Jira z Data Center. Procedura instalacji jest taka sama.

**Jakie adresy IP są używane do komunikacji z systemem Jira?**

Lista naszych statycznych adresów IP znajduje się [tutaj](https://help.miro.com/hc/articles/360017572694).

Należy pamiętać, że są to adresy wykorzystywane wyłącznie do komunikacji z systemem Jira. Adresy IP aplikacji Miro są dynamiczne i aby zapewnić poprawne działanie wszystkich funkcji na tablicach Miro (w tym niektórych związanych z kartami Jira), prosimy o [dodanie naszych domen do listy dozwolonych](https://help.miro.com/hc/articles/360017572694).

**Czy możemy zintegrować Jira z Miro, ale zablokować zgłoszenia Jira z poziomem zabezpieczeń ustawionym na „Prywatne”?**

Nie, to nie jest możliwe. Poziomy zabezpieczeń w Jira nie mają odniesienia do Miro.

**Ogólne**

**Czy możemy połączyć Miro z Jira, jeśli używamy serwera Jira?**

Ponieważ Miro to narzędzie online, możesz się połączyć z Jira tylko wtedy, gdy Twoja instancja jest otwarta na publiczny internet.

**Czy możemy połączyć wiele instancji Jira jednocześnie?**

Tak. Należy jednak pamiętać, że podłączenie instancji Jira polega na ustanowieniu początkowego połączenia, podczas gdy aktywne połączenie odnosi się do aktualnie używanej podłączonej instancji. Aktywne połączenie określa, skąd importowane są karty Jira przy otwieraniu aplikacji kart Jira i dla której instancji użytkownicy mają autoryzację. Dla danego użytkownika może być aktywne tylko jedno (1) połączenie naraz. Z protokołem OAuth 2.0, użytkownik może edytować dowolną kartę Jira powiązaną z dowolną podłączoną instancją, dla której już wcześniej się uwierzytelnił. Dla każdego innego protokołu uwierzytelniania cały zespół współdzieli aktywną instancję i może importować oraz współdziałać tylko z kartami z tej instancji. Możesz zdefiniować wiele ustawień na poziomie organizacji i przełączać się między aktywnymi połączeniami na poziomie zespołu.

**Jaki jest proces migracji z serwera do chmury?**

Podczas migracji do chmury Twój podstawowy adres URL Jira nieuchronnie się zmieni, a integracja ulegnie przerwaniu bez wprowadzenia zmian z naszej strony. Prosimy o [kontakt z pomoca](https://help.miro.com/hc/articles/360020185799) Miro w celu uzyskania pomocy.

**Czy Miro utworzy webhook dla każdego zespołu, projektu czy instancji Miro?**

Jeśli włączysz Automatyczny webhook w swoich ustawieniach Miro, tworzenie webhooków nastąpi automatycznie. Jeśli używasz autoryzacji na poziomie zespołu z Jira, Miro tworzy webhooki per zespół. Jeśli używasz autoryzacji na poziomie organizacji, Miro tworzy webhooki dla każdej organizacji.

**Czy wtyczka karty Jira obsługuje projekty Next-Gen?**

Tak, obsługuje.

Należy zauważyć, że obecnie nie ma pola/linku Epic podczas tworzenia karty Jira dla projektu Next-Gen po stronie Miro.

**Czy niestandardowe pola Jira są obsługiwane?**

Tak, obsługujemy prawie wszystkie pola niestandardowe typów *podstawowych*. Jeśli masz pole typu *złożonego*, może ono nie być obsługiwane i powodować nieoczekiwane zachowania podczas aktualizowania lub tworzenia kart Jira na tablicy.

**Co się stanie z istniejącymi kartami Jira, jeśli przełączymy się na inną instancję Jira?**

Obecnie, gdy przenosisz zgłoszenia Jira z jednego Projektu do innego w Jira, nie będą się one już aktualizować po stronie Miro.

Jako obejście sugerujemy skopiowanie adresu URL zgłoszenia Jira (Ctrl/Cmd+C) i wklejenie go na tablicę Miro (Ctrl/Cmd+V). Dzięki temu karta Jira pokaże nowe wartości i będzie automatycznie aktualizowana.

**Co się stanie z kartami Jira na tablicy, jeśli tablica zostanie przeniesiona do innego zespołu Miro?**

Karty Jira pozostaną na tablicy, ale nikt nie będzie mógł ich modyfikować (nawet jeśli ta sama instancja Jira jest skonfigurowana dla docelowego zespołu).

Po kliknięciu karty zobaczysz komunikat: *"Karta Jira została zaimportowana z innego konta"*. Jeśli chcesz, aby karty były edytowalne, zaimportuj je ponownie na tablicę.

**Czy integracja kart Jira wiąże się z dodatkowymi kosztami?**

Karty Jira są dostępne we wszystkich płatnych wersjach, a także w planie Education, bez dodatkowych opłat (Starter, Business, Education i Enterprise).

**Czy użytkownik ma dostęp do wszystkich kart Jira na tablicy?**

Uprawnienia do integracji kart Jira zapewniają, że użytkownicy mogą tworzyć i edytować karty tylko w projektach Jira, do których mają dostęp.

Wszystkie widgety na tablicy Miro są widoczne dla wszystkich, którzy mają do niej dostęp. Jeśli ktoś nie ma danych dostępowych do Jira lub nie ma odpowiednich danych dostępowych, będzie mógł wyświetlić zminimalizowaną kartę Jira na tablicy Miro (z tytułem i innymi polami), ale nie będzie mógł rozszerzyć karty, aby w pełni ją przejrzeć lub modyfikować.

**Czy Atlassian zakończył wsparcie dla Jira Server?**

Tak, Atlassian zakończył wsparcie dla Jira Server w lutym 2024 roku.

**Czy Miro Planer/karty Jira obsługują niestandardowe pola Jira: niestandardowe typy zgłoszeń i zależności?**

Tak, oba są obsługiwane. Jeśli pola **niestandardowe typy zgłoszeń** i **zależności** są skonfigurowane w Jira, *i* Miro Planer jest uwierzytelniony dla tej instancji Jira, to te niestandardowe pola są dostępne w planerze.

**Czy Miro obsługuje OAuth 2.0 dla Jira Data Center?**

Tak. Zobacz [Połącz się z Jira Data Center za pomocą OAuth 2.0.](https://help.miro.com/hc/articles/25753304280466)

**Karty Jira w tabelach i osiach czasu**

**Jak mogę zaimportować zgłoszenia Jira do tabel i osi czasu?**

Możesz przeciągnąć jedną lub kilka kart Jira bezpośrednio do tabeli lub osi czasu. To obecnie jedyny sposób, by to zrobić.

**Czy wszystkie pola w tabeli są połączone z Jira?**

Nie, w początkowej wersji tylko pięć pól w tabeli synchronizuje się z Jira:

Trzy systemowe pola Jira:

- Tytuł
- Opis
- Data zakończenia (w Jira występuje jako Termin)

Dwa niestandardowe pola Jira:

- Data początkowa
- Estymata

**Jakie pola w tabeli nie synchronizują się z Jira?**

Pola Osoba przypisana oraz Status nie synchronizują się z Jira i są wyłączone w tabelach oraz na osi czasu. Te pola i ich zawartość są obecne, ale nie są widoczne ani edytowalne w tabelach i na osi czasu.

Możesz je jednak edytować bezpośrednio w kartach Jira za pomocą panelu bocznego. Wystarczy, że przeciągniesz wiersz z tabeli lub osi czasu na planszę, aby Twoja karta Jira ponownie się pojawiła.

Wszystkie inne pola poza pięcioma wymienionymi powyżej (tytuł, opis, data zakończenia, data początkowa i estymata) są przechowywane tylko w Miro i nie synchronizują się z Jira.

**Dlaczego nie mogę edytować pola w tabeli lub na osi czasu spośród obsługiwanych pięciu pól Jira powyżej?**

Pole może nie być obecne na ekranie edycji w Jira.

Łatwym sposobem sprawdzenia, czy pole jest dostępne na ekranie edycji, jest:

W Miro otwórz panel boczny dla karty Jira. Sprawdź, czy pole jest tam obecne. Jeśli go nie ma, musisz dodać pole do ekranu edycji w Jira.

Są rzadkie przypadki, w których pola są edytowalne w Jira, ale nie są obecne na ekranie edycji. W takim przypadku nie można ich edytować w Miro.

Czy pole, którego nie możesz edytować, to **Data rozpoczęcia** lub **Szacowanie**? Jeśli tak:

Możliwe, że pole nie jest obecne w Jira lub nie ma go na ekranie edycji (odniesienie do poprzedniego punktu).

Może wystąpić problem z mapowaniem dla pola Data rozpoczęcia lub Szacowanie, ponieważ są to pola niestandardowe w Jira.

Mapujemy te pola zgodnie z następującą logiką:

- **Data początkowa**: Sprawdzamy pola o nazwach: Start Date, StartDate, Target Start
- **Szacowanie**: Sprawdzamy pola o nazwach: Story Points, Story point estimate, Story Point, StoryPoints, StoryPoint
- Jeśli pola Data początkowa lub Szacowanie nie noszą jednej z podanych powyżej nazw, może to być przyczyną problemów z edycją.

**Dlaczego edycja pola daty rozpoczęcia lub Estymacji w tabeli lub na osi czasu w Miro nie działa lub aktualizuje niewłaściwe pole w Jira?**

Obecnie polegamy na automatycznym mapowaniu dla pól Daty Rozpoczęcia i Estymacji w Jira. Ponieważ są to pola niestandardowe w Jira, może wystąpić przypadek, że w konfiguracji Jira istnieje wiele pól spełniających powyższe kryteria.

Wybieramy pierwsze dopasowanie według kolejności nazw pól wymienionych powyżej:

Na przykład, jeśli bilet Jira zawiera pola Story Points i Szacowanie Punktów Opowieści, dopasujemy pierwsze według powyższej listy, czyli Story Points. W związku z tym wszelkie zmiany w polu Estymacji w tabeli będą aktualizować pole Story Points w Jira, a nie Szacowanie Punktów Opowieści.

Obecnie nie ma obejścia tego problemu. Jeśli napotkasz ten problem, prosimy o przesłanie feedbacku do swojego zespołu wsparcia, abyśmy mogli lepiej zrozumieć Twoje potrzeby podczas tworzenia bardziej zaawansowanych możliwości mapowania pól.

**Dlaczego nie mogę importować kart Jira z dwóch różnych instancji do tabeli lub osi czasu?**

Obecnie wspieramy tylko jedną instancję Jira na tabelę lub oś czasu. Po zaimportowaniu karty Jira do tabeli lub osi czasu, tabela lub oś czasu zostaje powiązana z tą konkretną instancją Jira.

Nawet jeśli wszystkie rekordy Jira zostaną usunięte, link do oryginalnej instancji Jira pozostaje. Aby zaimportować karty z innej instancji Jira, należy utworzyć nową tabelę lub oś czasu.

**Dlaczego nie mogę zobaczyć lub edytować pól Status i Osoba odpowiedzialna dla moich rekordów Jira w tabeli lub osi czasu?**

Obecnie pola Status i Osoba odpowiedzialna w Jira nie są obsługiwane w tabelach i na osiach czasu. Zdecydowaliśmy się wyłączyć te pola w tabelach i na osiach czasu, aby zarządzać oczekiwaniami, unikać zamieszania i potencjalnej utraty danych. Pola Status i Osoba odpowiedzialna w Jira oraz ich zawartość istnieją, ale nie pojawiają się w tabelach ani na osiach czasu.

Możesz jednak nadal edytować te pola bezpośrednio w kartach Jira przy użyciu panelu bocznego. Wystarczy przeciągnąć wiersz z tabeli lub osi czasu na planszę, aby ponownie wyświetlić kartę Jira.

**Więcej informacji:**

- [Karty Jira](https://help.miro.com/hc/articles/360017572434)
- [Jak skonfigurować i odinstalować karty Jira](https://help.miro.com/hc/articles/360019501754)
- [Jak skonfigurować webhook dla kart Jira](https://help.miro.com/hc/articles/360017731113)
- [Możliwe problemy z kartami Jira i dodatkiem Jira](https://help.miro.com/hc/articles/360017572654)
