---
title: "Aplikacja \u201EEstymacja\u201D"
article_id: 5651786248210
translation_id: 5651786248210
locale: pl-pl
sidebar_position: 8
created_at: '2022-05-20T11:28:11Z'
updated_at: '2025-11-25T16:08:42Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: estimation
---

Estymacje są istotną częścią planowania i rozwoju zwin. Pomagają one dopasować uczestników zespołu do zakresu pracy, identyfikować luki w analizie lub zrozumieniu oraz określać jasne oczekiwania dotyczące realizacji.

Podczas szacowania uczestnicy zespołu przypisują liczbę do zadania odzwierciedlającego wymaganą ilość pracy. Aby przeprowadzać realistyczne szacunki, używany jest system numeracji, który dodaje poprzednie liczby razem. Uczestnicy zespołu mogą omawiać i wyrównać wybrany numer.

Skorzystaj z naszej aplikacji do [estymacji](../essential-tools/02-cards.md), aby przeprowadzać sesje estymacji w trybie multiplayer na tablicy Miro z kartami, [karteczkami](../essential-tools/14-sticky-notes.md) samoprzylepnymi i kartami [Jira](../../integrations-apps/atlassian/03-jira-cards.md).

> **Dostępność**: plany Starter, Business, Enterprise
> **Konfigurują**: uczestnicy zespołu z uprawnieniami do edycji na tablicy.

Aby rozpocząć estymację:

1. Otwórz aplikację Estymacja na pasku narzędzi współpracy i wybierz **Rozpocznij nową sesję**. ![Estimation_app_on_the_toolbar.jpg](images/21857804600850_Estimation%20app%20on%20the%20toolbar.jpg)*Aplikacja estymacji na pasku narzędzi*
2. Wybierz skalę estymacji: w menu rozwijanym wybierz koszulkę (dostępna tylko dla [kart](../essential-tools/02-cards.md) Miro) **lub** technikę estymacji **Fibonacciego.**
3. Przeciągnij obszar estymacji na obiekty, które chcesz oszacować. Możesz wybrać karty, karteczki lub [karty Jira](../../integrations-apps/atlassian/03-jira-cards.md) do estymacji. Możesz wykluczyć określone obiekty z estymacji, klikając niebieskie kropki.
4. Jeśli wybrany wybór zawiera karty Jira, zostaniesz poproszony o wybranie tablicy Jira, do której należą te karty. Dzięki temu estymaty są dokładnie i przewidywalnie zapisywane w systemie Jira. Bez tego kroku Jira nie potrafi przewidzieć zapisywania tych szacunków.
5. Kliknij **Estimate x** cards/stickies, gdy będziesz gotowy do rozpoczęcia estimation.estimation_launch.gifLaunching![](../../../../../../docs/using-miro/facilitation-tools/images/21016786471186_estimation%20launch.gif) *the estimation session**estimation_app_jira_cards.pngKorzystanie z aplikacji Estymacja z kartami Jira*![](../../../../../../docs/using-miro/facilitation-tools/images/21016786474514_estimation_app_jira_cards.png)

Wszyscy uczestnicy tablicy (oraz osoby, które dołączą do tablicy podczas sesji estymacji), będą mogli dołączyć do sesji estymacji. Wszyscy biorący udział muszą mieć dostęp do edycji tablicy i uprawnienia Jira. Estymacje mogą być wykonywane synchronicznie lub asynchronicznie. Wszystkie szacunki są anonimowe.

![join_estimation.jpg](../../../../../../docs/using-miro/facilitation-tools/images/21016751234578_join%20estimation.jpg)
*Wyskakujące okienko, aby dołączyć do sesji estymacji*

Użytkownicy zostaną przekierowani do pierwszego elementu, aby dodać swoje estymaty po kliknięciu **Dołącz do estymacji**. Użytkownicy mogą głosować na wszystkie elementy lub pomijać niektóre elementy i głosować tylko na konkretne. Aby edytować estymat, kliknij ikonę ołówka.

![adding_estimates.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751237010_adding%20estimates.gif)
*Estymacja w toku*

Po zakończeniu sesji moderator może zobaczyć ankietę dotyczącą szacunków dostarczonych dla każdego elementu i awatarów osoby, która dostarczyła estymatę. Po podaniu wszystkich elementów estymat przez wszystkich wymaganych uczestników, moderator może „Wybierz ostateczną estymatę” dla każdego elementu. Prowadzący może również edytować uzgodnione szacunki.

![agreed_estimates.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751238162_agreed%20estimates.gif)
*Estymacja zakończona*

Po uzgodnieniu szacunków dla wszystkich elementów moderator zobaczy wyskakujące okienko z opcją zakończenia sesji i udostępnienia wyników. Prowadzący może również kliknąć **Zakończ dla** wszystkich, aby zakończyć sesję w dowolnym momencie. Spowoduje to wyświetlenie liczby łącznych punktów. Kliknij **Zakończ i udostępnij wyniki** na wyskakującym okienku, a wyniki sesji zostaną zapisane.

![end_session.gif](../../../../../../docs/using-miro/facilitation-tools/images/21016751242386_end%20session.gif)
*Umowa na oszacowanie*

Jeśli oszacujesz karty lub karteczki Miro, estymaty są zapisywane jako tagi na kartach lub karteczkach.

![estimate_tags.jpg](../../../../../../docs/using-miro/facilitation-tools/images/21016786489362_estimate%20tags.jpg)
*Etykiety pokazują estymacje kart*

Jeśli estymujesz karty Jira za pomocą techniki estymacji **Fibonacciego,** estymaty są zapisywane w systemie Jira (obecnie synchronizacja działa tylko dla estymat Fibonacciego). Pamiętaj, że prowadzący powinien autoryzować się za pomocą swoich poświadczeń Jira przed podaniem ostatecznych szacunków. Wyniki estymacji zostaną automatycznie zsynchronizowane z odpowiednimi zgłoszeniami Jira.

**Aby estymacje Fibonacciego były widoczne na kartach Jira i w zadaniach Jira:**

1. Upewnij się, że pole punktów historii jest skonfigurowane w systemie Jira.
2. Sprawdź, czy masz odpowiednie uprawnienia w systemie Jira do aktualizowania wartości pola story points.
