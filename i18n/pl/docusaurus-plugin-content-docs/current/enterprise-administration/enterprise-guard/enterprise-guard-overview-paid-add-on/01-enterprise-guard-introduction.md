---
title: Wprowadzenie do Enterprise Guard
article_id: 15699815402514
translation_id: 15699815402514
locale: pl-pl
sidebar_position: 0
created_at: '2023-12-11T23:40:22Z'
updated_at: '2025-11-25T15:40:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

W dzisiejszej erze cyfrowej szybki wzrost ilości danych, szczególnie informacje wrażliwe, stał się istotnym problemem dla przedsiębiorstw. Miro, znane z gotowej do przedsiębiorstwa, internetowej przestrzeni roboczej do współpracy, która sprzyja innowacjom i pracy zespołowej, zaobserwowało znaczny wzrost złożoności i ilości treści w swoich tablicach. Znaczna liczba tablic Miro zawiera dane wysoce wrażliwe, takie jak informacje umożliwiające identyfikację osoby (PII), chronione informacje zdrowotne (PHI), informacje o kartach płatniczych (PCI) i więcej, co stanowi wyzwanie w zakresie zarządzania ryzykiem i zapewnienia zgodności. Trend ten podkreśla znaczenie wprowadzania zaawansowanych środków bezpieczeństwa i zgodności, aby zapobiec potencjalnym naruszeniom danych i wyciekom własności intelektualnej.

## Wprowadzenie Enterprise Guard: kompleksowe rozwiązanie dotyczące zabezpieczeń i nadzoru dla Miro

W odpowiedzi na te wyzwania, Miro wprowadza **Enterprise Guard**, zaawansowany dodatek zapewniający bezpieczeństwo i zgodność. Enterprise Guard oferuje pakiet funkcji, które umożliwiają organizacjom skuteczne identyfikowanie, klasyfikowanie, zabezpieczanie i zarządzanie poufnymi treściami na tablicach Miro. To rozwiązanie jest dostosowane do zapewnienia zgodności i solidnej ochrony danych na dużą skalę.

Dzięki integracji Enterprise Guard z ekosystemem przedsiębiorstwa Miro, organizacje mogą teraz wykorzystać bardziej solidne, zautomatyzowane i kompleksowe ramy bezpieczeństwa. Ten dodatek nie tylko chroni dane–umożliwia przedsiębiorstwom dalsze wprowadzanie innowacji i współpracę na Miro w sposób bezpieczny, bez zakłócania działania biznesu.

## Wydanie wersji General Availability Enterprise Guard: kluczowe funkcje

![Kluczowe funkcje wersji General Availability usługi Enterprise Guard](images/26702301024658_Enterprise-Guard-Data-Security.png)

- **Wykrywanie danych:** Enterprise Guard umożliwia proaktywny i dokładny proces [wykrywania danych](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md), co jest kluczowe dla identyfikacji danych wrażliwych, takich jak numery kart kredytowych, numery ubezpieczenia społecznego i inne krytyczne informacje rozproszone na różnych tablicach Miro. Ta proaktywna strategia jest kluczowa w identyfikowaniu i ograniczaniu potencjalnych podatności, pomagając zapobiegać naruszeniom danych i zapewniać zgodność.
- **eDiscovery:** Włącz bezpieczne zachowanie, śledzenie i eksport danych z tablicy, aby wspierać potrzeby prawne, zgodności i bezpieczeństwa. Funkcja eDiscovery w Enterprise Guard pomaga organizacjom spełniać zobowiązania regulacyjne dzięki możliwościom [prawnych blokad danych](../../canvas-25-admin-features/ediscovery/02-legal-hold-overview.md), [logów treści](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md) i [eksportu tablic](../../canvas-25-admin-features/ediscovery/13-board-export-api-overview.md).

  Prawne blokady danych zapobiegają trwałemu usunięciu treści istotnych dla dochodzeń lub spraw prawnych, zachowując wszystkie tablice, z którymi użytkownik objęty blokadą wchodzi w interakcje – w tym wszystkie ich wersje. Dzienniki treści dostarczają szczegółowych zapisów aktywności użytkowników, które można eksportować i integrować z zewnętrznymi narzędziami do audytu lub przeglądu prawnego. Dzięki interfejsom API eDiscovery klienci Enterprise mogą również eksportować dane tablic na dużą skalę, zapewniając dostępność kluczowych informacji dla procesów prawnych i zgodności.
- **Klasyfikacja automatyczna**: Ustaw kryteria dla Miro, aby [automatycznie klasyfikować swoje tablice](../../canvas-25-admin-features/data-classification/03-auto-classification-overview-and-scenarios.md) na podstawie wykrytej na nich poufnej zawartości.
- **Inteligentne zabezpieczenia****:** [Egzekwuj reguły bezpieczeństwa w czasie rzeczywistym](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md) i ogranicz, co użytkownicy mogą robić z tablicą, takie jak ograniczanie możliwości powielania zawartości tablicy i udostępniania na różnych poziomach (publiczny, zespół, organizacja), w oparciu o ręczną lub automatyczną klasyfikację tablicy. Zapewnia to trwałą prywatność i zgodność bez zakłócania działalności biznesowej.
- **Zasada kosza**: [Zasada kosza](https://help.miro.com/hc/articles/13860817985426) Enterprise Guard oferuje zaawansowaną kontrolę nad usuwaniem i przywracaniem tablic Miro. Organizacje mogą ustawić automatyczne terminy usuwania danych (30, 60, 90, 180 dni), aby zachować zgodność z wymaganiami regulacyjnymi, równoważąc retencję danych z minimalizacją ryzyka przedsiębiorstwa.
- **Retencja:** Zapewnij ochronę danych i zgodność, umożliwiając administratorom definiowanie, edytowanie i usuwanie zasad dostosowanych do potrzeb ich organizacji. Te zasady odgrywają kluczową rolę w ochronie tablic Miro w organizacji, umożliwiając Ci zachowanie niektórych tablic przez określony czas. [Retencja](https://help.miro.com/hc/articles/16855776325778) zapewnia, że tablice Miro nie będą usunięte przypadkowo lub celowo, dopóki nie zakończy się okres retencji. Wykorzystując polityki retencji, organizacje mogą zapewnić ochronę danych, zgodność i zachowanie informacji o krytycznym znaczeniu dla biznesu.
- ****Usuwanie:**** Włącz automatyczne czyszczenie tablic poprzez ich archiwizację i usuwanie na podstawie zasad retencji. [Usuwanie](../../canvas-25-admin-features/content-lifecycle-management/03-disposition-overview.md) zapewnia, że tablice są przechowywane tylko tak długo, jak to konieczne, a po okresie nieaktywności są automatycznie przenoszone do kosza. Od tego momentu standardowe ustawienia kosza określają, kto może przywracać tablice i kiedy zostaną trwale usunięte — wspierając zgodność, wydajność operacyjną i bezpieczeństwo danych.
- **Zarządzanie kluczami szyfrowania****(ZKS)****:** [EKM](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md) zapewnia scentralizowaną kontrolę nad kluczami szyfrowania, umożliwiając organizacjom monitorowanie działań związanych z kluczami oraz cofanie dostępu w razie potrzeby, co zapewnia dodatkową warstwę bezpieczeństwa danych.
