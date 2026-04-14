---
title: "Zale\u017Cno\u015Bci dla Jira"
article_id: 10649083010834
translation_id: 10649083010834
locale: pl-pl
sidebar_position: 7
created_at: '2023-03-22T10:22:08Z'
updated_at: '2025-11-25T16:22:15Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

Mapuj istniejące zależności lub twórz nowe pomiędzy kartami Jira na swoim [planerze](../../integrations-apps/atlassian/21-planner-for-jira.md) lub gdziekolwiek na swojej tablicy Miro, a one natychmiast zsynchronizują się w Jira. Dzięki aplikacji Zależności możesz identyfikować, wizualizować, omawiać i rejestrować zależności między zespołami w czasie rzeczywistym podczas ćwiczeń planowania.

> ****💡**** Ta funkcja jest teraz dostępna dla [Azure DevOps](08-dependencies-for-azure-devops.md).

> **Dostępne dla:** Abonament Business, Enterprise
>
> **Dostępne na:** Przeglądarka komputerowa, aplikacja komputerowa

## Jak działają zależności

Zależności pojawiają się jako warstwa linii łączących i pokazują relacje między kartami Jira.

Są widoczne tylko wtedy, gdy otworzysz zależności na tablicy. Uczestnicy mogą filtrować różne typy zależności, aby omawiać blokery i relacje.

![Dependencies-app.png](../../../../../../docs/using-miro/facilitation-tools/images/13244544218258_Dependencies-app.png)
*Zależności zmapowane między kartami Jira na widżecie Planer*

## Jak utworzyć nową zależność

1. Przejdź do paska narzędzi po lewej stronie tablicy.
2. Kliknij ikonę **Zależności**. Jeśli ikona Zależności nie znajduje się już na Twoim pasku narzędzi, musisz ją dodać z **Narzędzia, Media i Integracje** (**+**).
3. Otworzy się panel Zależności.
4. Kliknij **Nowa zależność**.
5. Kliknij **Pierwsza karta** i wybierz zgłoszenie Jira z listy rozwijanej lub wyszukaj je.
6. Wybierz **Typ zależności** spośród dostępnych w Twojej instancji Jira (na przykład blokuje, klonuje, duplikaty lub odnosi się do).
7. Kliknij **Drugą kartę** i wybierz zgłoszenie Jira z listy rozwijanej lub poprzez wyszukiwanie.
8. Kliknij **Zapisz szkic**, lub **Zapisz do Jira**bezpośrednio.

:::tip
Wersje robocze zależności są zapisywane tylko w Miro. Możesz tworzyć wersje robocze zależności jako propozycje dla innych uczestników i zespołów podczas ćwiczeń planowania. Po ich przeglądzie i omówieniu możesz zapisać je w Jira lub usunąć.
:::

![dependencies-entry-point.png](../../../../../../docs/using-miro/facilitation-tools/images/21537435953426_dependencies-entry-point.png)
*Tworzenie nowej zależności i zapisywanie jej w Jira*

## Jak wyświetlać i filtrować zależności

1. Przejdź do paska narzędzi po lewej stronie tablicy.
2. Kliknij ikonę **Zależności**. Jeśli ikona Zależności nie znajduje się już na pasku narzędzi, dodaj ją z sekcji **Narzędzia, Multimedia i Integracje** (**+**).
3. Panel Zależności otworzy się, a wszelkie istniejące zależności pojawią się jako linie na tablicy.
4. Kliknij ikonę **Filtr** na górze panelu Zależności.
5. Użyj przełączników, aby filtrować według **typu zależności** i **statusu synchronizacji**.
6. Użyj rozwijanego menu **Pokaż linie**, aby kontrolować, kiedy zależności są wyświetlane. Wybierz **Zawsze**, aby zobaczyć wszystkie aktywne zależności. Wybierz **Po zaznaczeniu**, aby zobaczyć zależności tylko wtedy, gdy klikniesz konkretną kartę Azure lub typ zależności.

Linie przerywane pokazują zależności w wersji roboczej, a linie ciągłe zależności zsynchronizowane z Jira. Kolor linii reprezentuje typ zależności.

![Filtering-dependencies.gif](../../../../../../docs/using-miro/facilitation-tools/images/13245295619730_Filtering-dependencies.gif)
*Filtrowanie widoku zależności* *w widżecie planowania*

## Jak edytować, zapisać, przywrócić lub usunąć zależność

1. Przejdź do paska narzędzi tworzenia po lewej stronie tablicy.
2. Kliknij ikonę **Zależności**.
3. Otworzy się panel Zależności.
4. Kliknij ikonę **Edycja** obok zależności.

![The_option_to_edit_a_Dependency.jpg](../../../../../../docs/using-miro/facilitation-tools/images/10866625733778_The%20option%20to%20edit%20a%20Dependency.jpg)
*Edycja zależności*

Możesz zmienić **pierwszą kartę** i **drugą kartę** zależności, a także **typ zależności.**

*![Editing_a_dependency.gif](../../../../../../docs/using-miro/facilitation-tools/images/10866808392722_Editing%20a%20dependency.gif)**Zmiana pierwszej karty i typu zależności*

Kliknij **Zapisz w Jira**, aby zapisać i zsynchronizować szkic zależności z Jira.

![Save_to_Jira.png](../../../../../../docs/using-miro/facilitation-tools/images/10868740630034_Save%20to%20Jira.png)
*Zapisywanie szkicu zależności w Jira*

Kliknij **Przywróć do szkicu**, aby przywrócić zsynchronizowaną zależność do szkicu.

![Revert_to_draft.png](../../../../../../docs/using-miro/facilitation-tools/images/10868741500690_Revert%20to%20draft.png)
*Przywracanie zsynchronizowanej zależności w Jira do szkicu*

Kliknij ikonę **Kosz**, aby usunąć zależność.
![Delete_dependency.png](../../../../../../docs/using-miro/facilitation-tools/images/10868804195986_Delete%20dependency.png)*Usuwanie zależności*
