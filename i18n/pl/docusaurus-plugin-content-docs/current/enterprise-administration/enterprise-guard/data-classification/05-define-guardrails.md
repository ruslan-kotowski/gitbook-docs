---
title: Zdefiniuj zabezpieczenia
article_id: 16494716849810
translation_id: 16494716849810
locale: pl-pl
sidebar_position: 4
created_at: '2024-01-19T19:01:45Z'
updated_at: '2025-11-25T15:40:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Definiowanie zabezpieczeń to trzeci krok konfiguracji przepływu automatycznej klasyfikacji i zabezpieczeń. W tym kroku przepływu skonfigurujesz zabezpieczenia, które są ograniczeniami obowiązującymi dla każdego poziomu klasyfikacji, takimi jak blokowanie udostępniania publicznego, blokowanie udostępniania z zespołami, blokowanie udostępniania w organizacji lub blokowanie replikacji treści. Na przykład możesz skonfigurować zabezpieczenia, aby blokować publiczne udostępnianie, blokować udostępnianie z zespołami, blokować udostępnianie w organizacji oraz blokować replikację treści dla użytkowników tablic sklasyfikowanych jako POUFNE.

### Wymagania wstępne

- Musisz ukończyć pierwszy i drugi krok przepływu automatycznej klasyfikacji i zabezpieczeń, [1: <a> Zdefiniuj poziomy klasyfikacji](07-define-classification-levels.md) i [2: Zdefiniuj automatyczną klasyfikację](07-define-classification-levels.md).
- Musisz znać zabezpieczenia, które chcesz przypisać do każdego poziomu klasyfikacji, w oparciu o swoje wymagania dotyczące bezpieczeństwa i zarządzania.
- Musisz mieć [rolę administratora treści wrażliwych](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby uzyskać rolę administratora treści wrażliwych, skontaktuj się z administratorem firmy.

Administratorzy mają dwie opcje wprowadzenia Inteligentnych zabezpieczeń w swojej organizacji:
- **Tryb domyślny:** Domyślnie zabezpieczenia nie wpływają na aktywne opcje udostępniania na tablicach, aby nie zakłócać współpracy, nawet gdy tablice są przeklasyfikowywane podczas automatycznej klasyfikacji.

- **Tryb restrykcyjny:** Po włączeniu przełącznika "Zastosuj zabezpieczenia w trybie restrykcyjnym", zabezpieczenia nadpisują wszystkie aktywne opcje udostępniania. Zapewnia to administratorom najwyższy poziom kontroli, ale może również skutkować natychmiastową utratą dostępu do tablic przez niektórych użytkowników.

![zabezpieczenia.png](images/26201318500754_guardrails.png)

## Przypisz zabezpieczenia

Aby przypisać zabezpieczenia do poziomu klasyfikacji, wykonaj następujące kroki:

1. Na stronie **Definiowanie zabezpieczeń** kliknij ikonę **Edycja** poziomu klasyfikacji, dla którego chcesz przypisać zabezpieczenia. Na przykład, jeśli chcesz przypisać zabezpieczenia dla poziomu klasyfikacji CONFIDENTIAL, kliknij ikonę edycji w wierszu poziomu klasyfikacji CONFIDENTIAL.
2. Wybierz pole wyboru dla każdej etykiety barierki ochronnej, którą chcesz przypisać do tego poziomu klasyfikacji. Na przykład, jeśli chcesz zablokować publiczne udostępnianie, udostępnianie zespołom, udostępnianie w organizacji, replikację treści dla użytkowników tablic sklasyfikowanych jako POUFNE, udostępnianie poza dozwolonymi domenami oraz użycie Miro AI, zaznacz następujące pola wyboru:
   - **Blokowanie replikacji zawartości
   **-<strong> Zablokuj korzystanie z Miro AI (wersja beta)**
   - **Blokowanie udostępniania publicznego**
   - **Blokowanie udostępniania zespołom**
   - **Blokowanie udostępniania w organizacji**
   **- Zablokuj udostępnianie poza dozwolonymi domenami (wersja beta)**
   Po zaznaczeniu tego pola wyboru musisz dodać domeny, które chcesz zezwolić, wpisując i wybierając z listy domen dozwolonych w organizacji lub wpisując nową domenę w polu i klikając + **Dodaj**.
   Aby uzyskać więcej informacji o każdym zabezpieczeniu treści i udostępniania, zobacz [Przegląd i scenariusze inteligentnych zabezpieczeń](01-intelligent-guardrails-overview.md).**
3. Domyślnie zabezpieczenia nie wpływają na aktywne opcje udostępniania na tablicach, aby nie zakłócać bieżącej współpracy, w tym także gdy tablice są przeklasyfikowane podczas automatycznej klasyfikacji.

   Jeśli chcesz zastosować zabezpieczenia i nadpisać wszystkie aktywne opcje udostępniania, włącz przełącznik **Zastosuj zabezpieczenia w trybie restrykcyjnym**. Może to spowodować utratę dostępu do tablic przez użytkowników. Zapewnia to administratorom najściślejszy poziom kontroli, ale może również skutkować natychmiastową utratą dostępu do tablic przez niektórych użytkowników.
   ![zabezpieczenia.png](images/26201318500754_guardrails.png)
4. Kliknij **Gotowe**.
   Twoja konfiguracja została zapisana, ale zacznie obowiązywać dopiero po kliknięciu **Opublikuj** na stronie [**Przegląd skutków**](06-review-impact.md).
5. Gdy skończysz definiowanie zabezpieczeń dla różnych poziomów klasyfikacji, przejdź do [Ukończ konfigurację zabezpieczeń](05-define-guardrails.md).

## Zakończ konfigurację zabezpieczeń

Po zakończeniu przypisywania zabezpieczeń dla różnych poziomów klasyfikacji kliknij **Dalej**. Twoja konfiguracja została zapisana, ale wejdzie w życie dopiero po kliknięciu **Opublikuj** na stronie [Przeglądaj skutki](06-review-impact.md).
