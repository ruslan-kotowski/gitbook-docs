---
title: Karty Jira
article_id: 360017572434
translation_id: 21892772372498
locale: pl-pl
sidebar_position: 5
created_at: '2024-10-10T08:06:30Z'
updated_at: '2025-11-25T15:59:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Plany: Starter, Business, Education, Enterprise Osoby: Wszyscy użytkownicy
    Platformy: Przeglądarka, Komputer stacjonarny, Urządzenie mobilne Jira: Jira Cloud,
    Jira Server (on-premise), Jira Data Center'
---

Karty Jira pozwalają pracować ze zgłoszeniami Jira bezpośrednio w tablicach Miro. Ta integracja upraszcza przepływ pracy zespołu, przenosząc zgłoszenia Jira do przestrzeni roboczej na retrospektywy, estymacje, priorytetyzację backlogu, mapowanie historyjek użytkownika oraz inne działania zespołowe.

![Jira cards in user story mapping](../../../../../../docs/integrations-apps/atlassian/images/21017348097170_Jira%20cards%20in%20USM.png)

## Importuj zgłoszenia Jira na swoją tablicę

Możesz importować zgłoszenia Jira na swoją tablicę na dwa sposoby:

1. Kopiuj URL zgłoszenia Jira i wklej go na tablicy.
2. Kliknij ikonę **Narzędzia, Multimedia i Integracje** (**+**) na pasku narzędzi Tworzenie, wybierz **Karty Jira**, wybierz jedno lub więcej zgłoszeń i kliknij **Dodaj**.

Podczas importowania zgłoszeń po raz pierwszy musisz połączyć swoje konto Jira:

1. Kliknij **Autoryzuj** w wyświetlonym oknie dialogowym.
2. Zaloguj się do swojego konta Jira, korzystając z danych dostępowych.
3. Autoryzuj połączenie między Miro i Jira.

Po autoryzacji zobaczysz wszystkie dostępne zgłoszenia Jira w selektorze kart Jira.

:::note
Użytkownicy, którzy nie autoryzowali swojego konta Jira, zobaczą uproszczone wyświetlanie karty bez awatarów przypisanych użytkowników.
:::

## Twórz nowe zgłoszenia Jira

Możesz tworzyć zgłoszenia Jira bezpośrednio z Miro na dwa sposoby.

### Twórz używając aplikacji Jira

1. Kliknij ikonę **Narzędzia, media i integracje** (**+**) na pasku narzędzi tworzenia
2. Wybierz **Karty Jira**.
3. Kliknij **Utwórz zgłoszenie**.
4. Uzupełnij wymagane pola.
5. Kliknij **Utwórz**.

### Konwertuj istniejące elementy na zgłoszenia Jira

Możesz konwertować istniejące karteczki lub karty na swojej tablicy na zgłoszenia Jira.

1. Wybierz do 50 karteczek lub kart.
2. Kliknij **Konwertuj na** > **Jira** w menu kontekstowym.
3. Ustaw domyślne wartości (typ zgłoszenia, priorytet, przypisany itp.).
4. Kliknij **Konwertuj**.

:::warning
Notatka:

- Kart w linii zadań USM nie można przekształcić w zgłoszenia Jira.
- Podczas konwersji tagi i data rozpoczęcia z kart Miro nie będą zachowane.
- Informacje o osobie przypisanej muszą być ustawione ponownie po konwersji.
:::

## Wyświetlanie i edycja zgłoszeń Jira

:::warning
Edycja kart Jira nie jest obsługiwana w aplikacji mobilnej ani w wersji na komputer.
:::

Możesz wyświetlać karty Jira na dwa sposoby:

- Widok z boku
- Widok centrowany

### Edytuj zgłoszenia w Miro

1. Kliknij ikonę **Otwórz w panelu bocznym** lub **Otwórz w panelu centralnym**.
2. Wprowadź zmiany.
3. Kliknij **Aktualizuj**, aby zapisać.

### Zmień status zgłoszenia

1. Kliknij ikonę **Workflow**.
2. Wybierz żądany **Status** i **Komentarz**.
3. Kliknij **Aktualizuj**, aby zapisać.

### Edytuj w Jira

1. Wybierz kartę i kliknij ikonę **Źródło**.
2. Edytuj zgłoszenie w Jira w nowej karcie przeglądarki.
3. Zmiany zostaną automatycznie zsynchronizowane z kartą Miro.

## Synchronizacja między Miro a Jira

|  |  |
| --- | --- |
| **Aktualizacja instancji Jira vs aktualizacja karty Miro** | **Kiedy następuje aktualizacja?** |
| Aktualizacja w Jira za pomocą OAuth 1.0 i OAuth 2.0 | Karta Jira w Miro jest aktualizowana natychmiastowo za pomocą [webhooka](https://help.miro.com/hc/articles/360017731113). |
| Aktualizacja w Miro | Karta Jira w Miro jest natychmiast aktualizowana, a odpowiednie zgłoszenie Jira jest aktualizowane jednocześnie. |

## Dostosuj karty Jira

### Zmień kolory kart

1. Wybierz jedną lub więcej kart Jira.
2. Kliknij **kolor wypełnienia** w menu kontekstowym.
3. Wybierz żądany kolor.

### Konfiguruj pola niestandardowe

1. Kliknij ikonę **Narzędzia, media i integracje** (**+**) na pasku tworzenia
2. Wybierz **Karty Jira**.
3. Wybierz **Skonfiguruj karty**.
4. Zaznacz pola, które chcesz wyświetlić.
5. Kliknij **Zapisz**.

:::note
Ważne notatki dotyczące pól:

- Ustawienia dotyczą tylko bieżącej tablicy.
- Nie można usunąć domyślnych pól (Osoba przypisana, Typ zgłoszenia, Priorytet, Status).
- Pola mogą się nie pojawić, jeśli nie mają wartości lub nie są dostępne dla tego typu zgłoszenia.
- Nie są obsługiwane niektóre typy pól (np. kolorowe pola niestandardowe).
:::

## Wyszukiwanie zgłoszeń Jira

Wybór kart Jira najpierw pokazuje ostatnie zadania i oferuje kilka opcji sortowania:

- Typ zgłoszenia
- Priorytet
- Klucz
- Podsumowanie
- Przypisana osoba
- Stan

Użyj słów kluczowych, aby znaleźć konkretne zgłoszenia lub użyj **Jira Query Language** (JQL) do skomplikowanych wyszukiwań:

1. Wybierz przełącznik **Zaawansowane wyszukiwanie** w pasku wyszukiwania.
2. Wpisz swoje zapytanie JQL.

Wyniki będą się aktualizować na podstawie Twojego zapytania.

## Powiązane artykuły

- [FAQ kart Jira](https://help.miro.com/hc/articles/360013463739)
- [Konfigurowanie i usuwanie kart Jira](https://help.miro.com/hc/articles/360019501754)
- [Ustawianie webhooków dla kart Jira](https://help.miro.com/hc/articles/360017731113)
- [Rozwiązywanie problemów z kartami Jira](https://help.miro.com/hc/articles/360017572654)
