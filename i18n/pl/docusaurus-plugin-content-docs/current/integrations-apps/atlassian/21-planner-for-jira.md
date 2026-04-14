---
title: Planer dla Jira
article_id: 10648975837970
translation_id: 31352781008914
locale: pl-pl
sidebar_position: 22
created_at: '2025-11-25T16:19:34Z'
updated_at: '2026-02-09T13:21:25Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Dzięki planerowi dla Jira, prowadzący i zespoły mogą prowadzić i uczestniczyć w wydarzeniach planistycznych na tablicy Miro, a także synchronizować aktualizacje z tablicą Jira w czasie rzeczywistym — oszczędzając godziny pracy ręcznej.

> **Dostępne dla:** abonament Business, abonament Enterprise

Podczas wydarzeń planistycznych zespołów i firmy, takich jak Inkrementy Programu (PI), Duże Spotkania, roadmapy i sprinty, zespoły deweloperskie dyskutują i uzgadniają swoje działania.

:::tip
Planer jest teraz dostępny dla [Azure DevOps](https://help.miro.com/hc/articles/15280547945618).
:::

## Jak utworzyć planer dla Jira

1. Przejdź do [paska narzędzi tworzenia](https://help.miro.com/hc/articles/360017730553-Toolbars) po lewej stronie Twojej tablicy.
2. Kliknij **Więcej aplikacji** (**+**) i wyszukaj ‘Planner’.
3. Kliknij **Planner**, aby uruchomić aplikację.
4. Na tablicy pojawi się kursor. Kliknij dowolne miejsce, aby umieścić pusty planer.
5. Kliknij rozwijane menu **tablica Jira** i wybierz tablicę, którą chcesz połączyć z Planerem. Jeśli nie autoryzowałeś jeszcze swojego konta Jira w Miro, zostaniesz poproszony o zalogowanie się.
6. Pierwsze pole **Kolumny** to twój *typ kolumny*. Po wybraniu tablicy Jira, typ kolumny domyślnie ustawi się na **Status** i pokaże do 3 kolumn. Kliknij na pierwsze pole **Kolumny**, aby wybrać inny typ kolumny z rozwijanego menu (możesz wybrać Sprint, Status, Priorytet, Fix versions, Komponenty lub pole niestandardowe).
7. Użyj drugiego pola **Kolumny** , aby dopracować swój Planer. Na przykład, jeśli wybrałeś 'Sprint' jako pole Kolumny, możesz wybrać, które sprinty mają być wyświetlane.
8. Dodaj **swimlane'y** do planera, oprócz kolumn, aby jeszcze lepiej zorganizować zadania względem drugiego pola Jira (możesz wybierać między Sprint, Status, Priorytet, Wydania do naprawy, Komponenty lub pole niestandardowe).

:::note
Aktualnie planer obsługuje tylko jedną tablicę Jira. Jednak możesz stworzyć wiele planerów na jednej tablicy Miro.
:::

![Creating-a-planner-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696033042_Creating-a-planner-widget.gif)*Tworzenie planera*

## Jak pracować z planerem

Przeciągaj karty Jira między kolumnami, aby je zaktualizować. Na przykład przeciągnięcie karty Jira z backlogu do sprintu w planerze zaktualizuje ją zarówno w Miro, jak i Jira.

![Dragging-stories-between-columns-planning-widget.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696028306_Dragging-stories-between-columns-planning-widget.gif)*Przenoszenie kart Jira między sprintami*

Wybierz pole dla **torów**, aby podzielić pracę na wiersze oraz kolumny. Przeniesienie kart między torami zaktualizuje zarówno pola *kolumny*, jak i *toru* w zgłoszeniu Jira.

![Choosing-a-swimlane.png](../../../../../../docs/integrations-apps/atlassian/images/21017725756946_Choosing-a-swimlane.png)*Wybieranie pola dla torów*

Domyślnie planer wyświetla wszystkie zgłoszenia w Twoim backlogu. Aby skupić się na bieżącym sprincie, wybierz w prawym górnym rogu ikonę filtru, a następnie zaznacz **Sprint**. Następnie wybierz filtr **Sprint** i włącz **Filtruj według aktywnego sprintu**. Wybierz **Zastosuj**, aby użyć filtru sprintu.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Filtruj zgłoszenia według aktywnego sprintu.*

Możesz także użyć rozwijanej listy **Typ zgłoszenia** i wybrać, które typy zgłoszeń mają być wyświetlane w Twoim Planerze. Na przykład, możesz filtrować tylko po Story.

![Filtering-by-issue-type-planning-widget.png](../../../../../../docs/integrations-apps/atlassian/images/21017725749138_Filtering-by-issue-type-planning-widget.png)*Filtrowanie według typu zgłoszenia*

Uczestnicy mogą komentować karty Jira, aby śledzić bieżące dyskusje i notatki.

![Commenting_on_a_story.png](../../../../../../docs/integrations-apps/atlassian/images/21017696024594_Commenting%20on%20a%20story.png)*Komentowanie karty Jira w planerze*

:::note
Karty Miro, karteczki oraz inne obiekty nie mogą być umieszczane w planerze.
:::

## Możliwości i obciążenie

Podejmuj świadome decyzje o priorytetach podczas planowania Sprint i PI poprzez wizualizację całkowitej liczby story points w łatwych do odczytania kolumnach. Zwiększ efektywność swojego zespołu i zapewnij optymalne rozłożenie pracy.

### Włącz pole story points w kartach Jira

1. Przejdź do [paska narzędzi tworzenia](https://help.miro.com/hc/articles/360017730553-Toolbars#Creation_toolbar) po lewej stronie swojej tablicy.
2. Kliknij **Więcej aplikacji** (**+**) i wyszukaj 'karty Jira'.
3. Kliknij **karty Jira**, aby uruchomić aplikację.
4. Kliknij **Konfiguruj karty**.
5. Przewiń w dół i włącz **Story Points**.

![Enabling-Story-Points-for-Jira-Cards.gif](../../../../../../docs/integrations-apps/atlassian/images/21017696030866_Enabling-Story-Points-for-Jira-Cards.gif)
*Włączanie story pointów dla kart Jira*

### Wykorzystanie możliwości i obciążenia

Po włączeniu story pointów możesz utworzyć nowy planer lub odświeżyć tablicę z istniejącym planerem. Dopóki przynajmniej jedno zgłoszenie na tablicy ma przypisane story pointy, zobaczysz od razu pola **Możliwości** i **Obciążenie** na górze każdej kolumny w planerze.

![Balancing-Capacity-and-Load.gif](../../../../../../docs/integrations-apps/atlassian/images/21017725755794_Balancing-Capacity-and-Load.gif)*Równoważenie możliwości i obciążenia*

### Zrozumienie możliwości i obciążenia

**Pojemność**: Ręcznie wprowadź pojemność dla każdej kolumny w swoim planerze. Jeśli pojemność jest mniejsza niż obciążenie, kolumna zmieni kolor na czerwony, sygnalizując, że przekroczyłeś limit pojemności zespołu. Ten wizualny sygnał skłania do rozważenia przeniesienia zgłoszeń, aby utrzymać zrównoważony rozkład pracy.

**Obciążenie**: Reprezentuje sumę story points dla wszystkich kart w danej kolumnie. Karty bez przypisanych punktów będą liczone jako 0 w tym obliczeniu.

## Konfiguracja Jira

Aby skonfigurować planer, najpierw wybierz tablicę Jira, z której chcesz zaimportować zgłoszenia. Może to być tablica either z Jira Scrum lub Kanban.

Podczas tworzenia planera możesz wybrać, które pole z Jira użyć dla swoich kolumn i wierszy (torów), w tym:

- Sprinty
- Stan
- Wersja poprawki
- Komponent
- Priorytet
- Osoba przypisana
- Dowolne pole niestandardowe z jednokrotnym wyborem z listy rozwijanej
- Dowolne pole niestandardowe z wielokrotnym wyborem z listy rozwijanej

Obecnie nie obsługujemy innych pól Jira ani pól związanych z datą.

Opcja „Sprint” pojawi się tylko wtedy, gdy pole sprintu jest dostępne na ekranie edycji zgłoszenia w Jira. Zazwyczaj jest ono wstępnie skonfigurowane dla Jira Server/Data Center, ale często w Cloud wymaga ręcznego dodania pola sprintu. Przeczytaj więcej o [konfigurowaniu ekranów zgłoszeń](https://support.atlassian.com/jira-cloud-administration/docs/configure-issue-screens/).

:::note
Zamknięte sprinty nie mogą być wyświetlane w Planerze.
:::

### Jak utworzyć Planer przy użyciu niestandardowego JQL

Aby utworzyć planer używając niestandardowego JQL, zacznij od stworzenia tablicy Jira z zapytaniem JQL. Po utworzeniu tablicy Jira, postępuj zgodnie z instrukcjami powyżej dotyczącymi tworzenia planera. Kiedy dojdziesz do kroku 5, pamiętaj, aby wybrać tablicę Jira utworzoną za pomocą spersonalizowanego zapytania JQL.

## Synchronizacja planera

### Z Miro do Jira

Gdy przesuniesz kartę między polami niestandardowymi w Miro, Jira zostaje zaktualizowana automatycznie. Może to zająć kilka sekund.

### Z Jira do Miro

Jeśli wprowadzisz zmiany w sprincie w Jira, zobaczysz powiadomienie **Dostępne aktualizacje** w menu kontekstowym planera. Może to potrwać kilka sekund po wprowadzeniu zmian w Jira.

Kliknij planer, aby otworzyć menu kontekstowe, i kliknij ikonę **Synchronizuj z Jira**, aby zsynchronizować najnowsze zmiany.

![Sync-planning-widget-with-jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017696029970_Sync-planning-widget-with-jira.png)*Synchronizacja aktualizacji z Jira do Miro*

## Mapowanie zależności

Uczestnicy mogą wizualnie mapować zależności między zadaniami na planerze. Dowiedz się więcej o [Zależnościach dla Jira](https://help.miro.com/hc/articles/10649083010834).
