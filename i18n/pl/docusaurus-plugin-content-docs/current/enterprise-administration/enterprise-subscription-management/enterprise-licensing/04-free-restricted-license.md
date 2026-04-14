---
title: "Bezp\u0142atna ograniczona licencja"
article_id: 360011746739
translation_id: 360011746739
locale: pl-pl
sidebar_position: 4
created_at: '2020-02-05T07:29:16Z'
updated_at: '2026-02-19T10:40:27Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-and-licences
---

Gdy nowi użytkownicy dołączają do Miro, w zależności od [modelu licencjonowania Enterprise](02-enterprise-licensing.md), mogą otrzymać bezpłatną ograniczoną licencję.

> **Dotyczy:** Wersja Enterprise

## Kiedy użytkownicy otrzymują bezpłatną ograniczoną licencję

**W programie elastycznych licencji (FLP)**, użytkownik może otrzymać bezpłatną ograniczoną licencję, gdy:

- Domyślna licencja dla nowych użytkowników jest ustawiona na bezpłatną ograniczoną
- Administrator firmy zaprasza użytkownika i wybiera dla niego bezpłatną ograniczoną licencję w oknie zaproszenia
- Administrator firmy konwertuje użytkownika na bezpłatną ograniczoną w **Ustawienia firmy > Aktywni użytkownicy**

:::note
Dowiedz się więcej o [programie elastycznych licencji (FLP)](03-flexible-licensing-program-flp.md) i [zarządzaniu licencjami w ramach FLP](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

**Na licencjach nieelastycznych (non-FLP)** użytkownikowi można przydzielić bezpłatną ograniczoną licencję, gdy:

- Użytkownik jest automatycznie dodawany (przez [zarządzanie domeną](../../canvas-25-admin-features/domain-control/01-domain-control.md) lub [obsługę administracyjną Just-in-Time](../../user-management/13-user-provisioning-on-enterprise-plan.md)) do organizacji, która podczas jego rejestracji w Miro ma niewystarczającą liczbę licencji Advanced, Standard lub Full (legacy).
- Użytkownik jest zapraszany do zespołu w organizacji, która ma niewystarczającą liczbę licencji Advanced, Standard lub Full (legacy).

Kiedy wielu użytkowników jest zapraszanych jednocześnie, otrzymują licencje w kolejności adresów e-mail na liście zaproszonych. Jeśli w organizacji brakuje licencji, użytkownicy na końcu listy otrzymają bezpłatną ograniczoną licencję. W tym przypadku osoba zapraszająca otrzyma powiadomienie o ograniczonym dostępie dla niektórych użytkowników.

## Jak działają bezpłatne ograniczone licencje dla użytkowników

Użytkownicy z bezpłatną ograniczoną licencją mogą wyświetlać i komentować tablice w zespołach, w których uczestniczą, oraz mogą prosić o uprawnienia do edycji i standardową licencję lub pełną (starszą) licencję od administratorów firmy. Mogą również wyszukiwać i dołączać do zespołów w organizacji wraz z innymi członkami.

:::note
Administratorzy firmy mogą [konfigurować ustawienia zarządzania prośbami](../../user-management/09-request-management-on-enterprise-plan.md).
:::

### Dostęp do tablicy z bezpłatną ograniczoną licencją

Następujące uprawnienia dotyczą użytkowników posiadających bezpłatną ograniczoną licencję: wyświetlanie, komentowanie lub edycja, w zależności od przyznanego poziomu dostępu.

|  |  |
| --- | --- |
| **Jak tablica została udostępniona** | **Poziom dostępu** |
| Przez link publiczny | Użytkownicy z licencją Free Restricted mogą mieć wyświetlanie i/lub edycję w zależności od przyznanego poziomu dostępu. |
| Przez link zespołu lub firmy | Użytkownicy z licencją Free Restricted mogą mieć wyświetlanie i/lub komentowanie w zależności od przyznanego poziomu dostępu. |
| [Osadzony link](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md) | Bezpłatni użytkownicy z ograniczoną licencją mogą wyświetlać i/lub komentować w zależności od przyznanego poziomu dostępu.  Bezpłatni użytkownicy z ograniczoną licencją nie będą mogli edytować ani prosić o uprawnienia do edycji, nawet jeśli dostęp do edycji jest przyznany poprzez uprawnienia osadzenia. |

## Jak zarządzać bezpłatnymi ograniczonymi licencjami

> **Kto może to zrobić:** administratorzy firmy

Na wszystkich subskrypcjach administrator firmy może zmienić licencję użytkownika z bezpłatnej ograniczonej na standardową lub pełną (starszą) licencję w sekcji **Aktywni użytkownicy** w ustawieniach zespołu lub firmy.

**Program elastycznych licencji (FLP)**

W subskrypcjach programu elastycznych licencji (FLP) administrator firmy może również w dowolnym momencie zmienić licencję zaawansowaną, standardową lub pełną (legacy) na bezpłatną ograniczoną licencję.

Kiedy użytkownik z bezpłatną ograniczoną licencją prosi o uprawnienia do edycji, administratorzy firmy otrzymują prośbę na podstawie swoich [ustawień zarządzania prośbami](../../user-management/09-request-management-on-enterprise-plan.md).

:::note
Dowiedz się więcej o [zarządzaniu licencjami w programie elastycznych licencji (FLP)](05-license-management-on-the-flexible-licensing-program-flp.md).
:::

## Często zadawane pytania

**Co się stanie z moimi bezpłatnymi ograniczonymi licencjami, gdy dodam więcej licencji Standard lub Full (legacy) do mojej wersji nie-FLP?**

Istniejący użytkownicy z bezpłatnymi, ograniczonymi licencjami nie są automatycznie zmieniani na nowe licencje Standard lub Full (legacy). Administratorzy firmy mogą ręcznie zmieniać licencje na wyższą wersję.
