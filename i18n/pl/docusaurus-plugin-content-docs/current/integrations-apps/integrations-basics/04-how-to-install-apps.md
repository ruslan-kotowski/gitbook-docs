---
title: Jak zainstalować aplikacje
article_id: 360017731093
translation_id: 360017731093
locale: pl-pl
sidebar_position: 4
created_at: '2019-02-11T10:12:46Z'
updated_at: '2025-08-05T07:54:07Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
availability:
  notes: 'Ludzie: Wszyscy użytkownicy Wersje: Wszystkie wersje Platformy: Przeglądarka,
    aplikacja komputerowa Administratorzy zespołu mogą ograniczyć instalację dla nie-administratorów.
    Administratorzy firmy w wersji Enterprise mogą dodatkowo ograniczyć dostęp tylko
    do zatwierdzonych aplikacji.'
---

Możesz rozszerzyć funkcjonalność Miro, instalując aplikacje z Miro Marketplace. Ten artykuł prowadzi Cię przez instalowanie i odinstalowywanie aplikacji, zrozumienie uprawnień aplikacji oraz zapewnia przegląd tworzenia niestandardowych integracji.

## Zainstaluj aplikacje z Miro Marketplace

[Miro Marketplace](https://miro.com/marketplace/) to Twoje centralne miejsce do odkrywania i dodawania aplikacji, które wzbogacą Twoje doświadczenie z Miro. Możesz zainstalować aplikacje bezpośrednio z Twojej tablicy lub odwiedzając stronę internetową Marketplace.

![Miro_marketplace.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021611044242_Miro%20marketplace.jpg)*Miro Marketplace*

Istnieją dwa główne sposoby, aby użytkownicy mogli dodać aplikacje:

1. **Z Twojej tablicy:** Kliknij ikonę **Narzędzia, media i integracje (+)** na pasku narzędzi tworzenia, a następnie użyj pola wyszukiwania „Search integrations” na karcie Marketplace. Jeśli znajdziesz już wymienioną aplikację, kliknij ją, aby dodać. Możesz także przeglądać dostępne aplikacje z tego panelu.
   ![marketplace-add-apps.png](../../../../../../docs/integrations-apps/integrations-basics/images/21260776452626_marketplace-add-apps.png)*Marketplace na pasku narzędzi tworzenia*
2. **Ze strony internetowej Marketplace:** Możesz również przejść bezpośrednio na stronę internetową [Miro Marketplace](https://miro.com/marketplace/), aby przeglądać i instalować aplikacje z ich odpowiednich list.

**Dla administratorów firmy:**
Administratorzy firmy w dostępnych wersjach mogą również instalować aplikacje dla całego zespołu poprzez ustawienia zespołu. Aby to zrobić, przejdź do **ustawień Zespołu** > **Aplikacje i integracje** > **Instaluj aplikacje**. Ta sekcja umożliwia scentralizowane zarządzanie i wdrażanie aplikacji w całym zespole.

![apps_and_integrations_page.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021832338450_apps%20and%20integrations%20page.jpg)*Sekcja zainstalowanych aplikacji w ustawieniach zespołu dla administratorów*

## Odinstaluj aplikacje

Możesz zarządzać i odinstalowywać aplikacje w ustawieniach zespołu. Należy pamiętać, że użytkownicy niebędący administratorami mogą mieć ograniczenia dotyczące odinstalowywania aplikacji, w zależności od konfiguracji zespołu.

:::warning
Użytkownicy niebędący administratorami nie mogą odinstalowywać aplikacji, jeśli nie są upoważnieni do ich instalowania przez administratora w ustawieniach zespołu.
:::

Aby zarządzać aplikacjami zespołu, przejdź do **Ustawienia zespołu > Aplikacje i integracje**. Ta strona zawiera listę wszystkich aplikacji aktualnie zainstalowanych dla Twojego zespołu lub przez Ciebie osobiście.

![apps_settings.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021898097682_apps%20settings.jpg)*Aplikacje i integracje w ustawieniach zespołu*

Aby odinstalować aplikację, wykonaj te kroki:

1. Z listy **Aplikacje i integracje** wybierz aplikację, którą chcesz usunąć.
2. Kliknij **Odinstaluj dla zespołu** lub **Odinstaluj dla mnie**. Dostępna opcja zależy od tego, jak aplikacja została zainstalowana i jakie masz uprawnienia administracyjne.

![uninstall_an_app.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021797466258_uninstall%20an%20app.jpg)*Opcja odinstalowania aplikacji*

## Uprawnienia do instalacji aplikacji

Administratorzy zespołu i firmy mają różne opcje kontroli, aby zarządzać tym, kto może instalować aplikacje i które aplikacje są dostępne dla ich organizacji, zapewniając bezpieczeństwo i zgodność.

Administratorzy zespołu mogą skonfigurować, czy członkowie zespołu niebędący administratorami mogą instalować aplikacje. To ustawienie znajduje się w **ustawieniach zespołu > Aplikacje i integracje** w ramach opcji zarządzania aplikacjami.

![allow_non-admins_to_install_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021903025170_allow%20non-admins%20to%20install%20apps.jpg)*Opcja "Zezwalaj użytkownikom niebędącym administratorami na instalację aplikacji" w ustawieniach zespołu*

Dla użytkowników w [wersji Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), administratorzy firmy mają dostęp do bardziej szczegółowych opcji kontroli. Mogą zarządzać **Zatwierdzonymi aplikacjami** poprzez **Ustawienia firmy** > **Aplikacje**. Ta funkcja pozwala administratorom na tworzenie listy aplikacji zatwierdzonych przez firmę, ograniczając użytkownikom możliwość instalowania aplikacji, które nie znajdują się na tej liście. [Dowiedz się więcej o zarządzaniu odkrywaniem i ustawieniami instalacji aplikacji dla wersji Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).

![Enterprise_apps.jpg](../../../../../../docs/integrations-apps/integrations-basics/images/5021890162962_Enterprise%20apps.jpg)*Zarządzanie zatwierdzonymi aplikacjami w ustawieniach firmy w wersji Enterprise*

## Integracje niestandardowe i platforma dla deweloperów

Jeśli potrzebujesz specjalnej funkcjonalności niedostępnej w Miro Marketplace, możesz stworzyć własne, dostosowane rozwiązania, korzystając z [platformy dla deweloperów Miro](https://miro.com/api/). Ta platforma oferuje solidne narzędzia, w tym interfejsy API REST, wtyczki internetowe i elementy osadzone, aby pomóc Ci budować potężne integracje dostosowane do Twoich potrzeb.

Oto kluczowe punkty do rozważenia przy tworzeniu niestandardowych integracji:

- **Pierwsze kroki:** Możesz zacząć budować swoją aplikację, [tworząc zespół deweloperów](https://developers.miro.com/). Standardowe zespoły deweloperów są przeznaczone do celów rozwoju i testowania i mają pewne ograniczenia:
  - Maksymalnie 5 użytkowników w zespole.
  - Maksymalnie 3 tablice w zespole.
  - Znak wodny jest wyświetlany na tablicach.
  - Funkcja eksportu tablicy jest niedostępna.
- **Deweloperzy wersji Enterprise:** Jeśli Twoja organizacja korzysta z [wersji Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), możesz utworzyć zespół programistów w ramach swojej subskrypcji. Te zespoły programistyczne nie są objęte ograniczeniami standardowych zespołów i korzystają ze wszystkich funkcji bezpieczeństwa klasy Enterprise. [Dowiedz się więcej o zespołach deweloperów w ramach wersji Enterprise](../../enterprise-administration/managing-apps-on-enterprise-plan/04-enterprise-developer-teams.md).

Aby uzyskać dodatkowe informacje, wsparcie oraz nawiązać kontakt z innymi deweloperami, możesz odwiedzić [Forum Platformy dla deweloperów](https://community.miro.com/developer-platform-forum-57).
