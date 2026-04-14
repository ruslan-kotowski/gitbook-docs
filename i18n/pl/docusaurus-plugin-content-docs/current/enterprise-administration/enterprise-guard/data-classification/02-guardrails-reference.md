---
title: "Odniesienie do zabezpiecze\u0144"
article_id: 28839068735890
translation_id: 28839068735890
locale: pl-pl
sidebar_position: 1
created_at: '2025-08-18T09:35:15Z'
updated_at: '2025-11-25T15:53:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

## Zabezpieczenia treści

Poniższa tabela wymienia zabezpieczenia treści obsługiwane w tej wersji.

|  |  |  |
| --- | --- | --- |
| **Zabezpieczenie** | **Opis** | **Użytkownicy dotknięci** |
| **Blokowanie replikacji zawartości** | - Opcje zarządzania replikacją zawartości w interfejsie użytkownika Miro i w API Miro nie są dostępne. Na przykład opcja aktualizacji, kto może kopiować zawartość tablicy, nie jest dostępna w interfejsie użytkownika, a opcja aktualizacji dostępu do kopiowania przez API aktualizacji tablicy nie jest dostępna.  - Opcje replikacji zawartości nie są dostępne w interfejsie użytkownika Miro. Obejmuje to:     - Duplikowanie tablicy do innych     zespołów innych użytkowników     - Pobieranie plików na tablicy     - Pobieranie obrazów na tablicy     - Pobieranie plików PDF na tablicy     - Kopiowanie treści lub obiektów z      tablicy na inną tablicę     - Eksportowanie tablic jako obrazu     - Eksportowanie tablic jako pliku PDF     - Zapisywanie tablic jako szablonu      szablon     - Replikacja zawartości przez interfejsy API jest      niedostępna. Interfejs API zwraca      błąd 403 jako odpowiedź. | Właściciele i współwłaściciele tablicy nie mają ograniczeń. Właściciele i współwłaściciele tablicy mogą wykonywać działania związane z replikacją zawartości, ponieważ jest to potrzebne właścicielowi tablicy do jej aktualizacji oraz tworzenia sanitarnych wersji tablic do dalszej współpracy.  Wszyscy inni mają ograniczenia. |
| **Zablokuj korzystanie z Miro AI** | - Wszystkie funkcje Miro AI są wyłączone, co uniemożliwia dostęp do funkcji opartych na sztucznej inteligencji, takich jak generowanie tekstu, rozpoznawanie obrazów i inteligentne sugestie.  - Użytkownicy nie będą mogli wchodzić w interakcję ani aktywować żadnych narzędzi opartych na sztucznej inteligencji w ramach Miro.  - Istniejąca zawartość wygenerowana przez Miro AI pozostaje bez zmian, a użytkownicy mogą modyfikować lub rozszerzać tę zawartość. Jednak użytkownicy nie mogą już używać Miro AI do edytowania lub aktualizowania treści. | Wszyscy mają ograniczenia, włącznie z właścicielem i współwłaścicielami tablicy. |

## Zabezpieczenia dotyczące udostępniania

Poniższa tabela zawiera zabezpieczenia dotyczące udostępniania dostępne w obecnym wydaniu.

|  |  |  |
| --- | --- | --- |
| **Zabezpieczenie** | **Opis** | **Dotknięci użytkownicy** |
| **Blokowanie udostępniania publicznego** | - Opcja udostępniania dla *Każdy, kto ma link* nie jest dostępna w interfejsie Miro.  - Publiczne udostępnianie za pomocą API nie jest dostępne. API zwraca błąd 403 jako odpowiedź.  - Blokada udostępniania publicznego nie dotyczy tablic osadzonych za pomocą linku dostępu Live Embed, ponieważ te tablice nie są uznawane za udostępniane poprzez link publiczny. Więcej informacji znajdziesz w artykule [Jak zezwolić na osadzanie lub ograniczyć osadzanie tablic Miro w obsługiwanych aplikacjach.](../../managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md) | Wszyscy mają ograniczenia, włącznie z właścicielem tablicy. |
| **Blokowanie udostępniania zespołom** | - Opcja udostępniania *Wszystkim w zespole* nie jest dostępna w interfejsie Miro.  - Udostępnianie zespołom za pośrednictwem API nie jest dostępne. API zwraca błąd 403 jako odpowiedź. | Wszyscy mają ograniczenia, w tym właściciel tablicy. |
| **Blokowanie udostępniania w organizacji** | - Opcja udostępniania *Każdemu w organizacji* nie jest dostępna w interfejsie Miro.  - Udostępnianie w organizacji za pośrednictwem API nie jest dostępne. API zwraca błąd 403 jako odpowiedź. | Wszyscy mają ograniczenia, w tym właściciel tablicy. |
| **Zablokuj udostępnianie poza dozwolonymi domenami** | - Udostępnianie tablic za pomocą bezpośrednich zaproszeń e-mail jest ograniczone do użytkowników, których adresy e-mail znajdują się w dozwolonych domenach na tej liście. To zabezpieczenie nie wpływa na dostęp udzielony za pośrednictwem linków zespołowych, organizacyjnych lub publicznych, ponieważ są one kontrolowane przez osobne zabezpieczenia.  - Możesz dodać do 20 dozwolonych domen do tej listy.  - To zabezpieczenie zostało zaprojektowane do współpracy z ustawieniem [**Bezpieczeństwo > Udostępnianie > Dozwolone domeny**](../data-security/07-sharing-policy-on-enterprise-plan.md), które można skonfigurować na poziomie zarówno organizacji, jak i zespołu. To oznacza, że jeśli masz włączone ustawienie **Dozwolone domeny**, musisz upewnić się, że domena, do której chcesz umożliwić udostępnianie tablic, jest wymieniona zarówno w ustawieniu Inteligentne zabezpieczenia, jak i w ustawieniu [**Bezpieczeństwo > Udostępnianie > Dozwolone domeny**](../data-security/07-sharing-policy-on-enterprise-plan.md).   **Uwagi:**  - Jeśli tablica była już udostępniona na adresy e-mail, które nie znajdują się na tej liście, użytkownicy, którzy już mają dostęp do tablicy, nadal będą mieli do niej dostęp.  - Istniejący użytkownicy, którzy już mają dostęp do tablicy, ale nie znajdują się na liście dozwolonych domen, są wskazywani w interfejsie zarządzania dostępem do tablicy. Możesz ręcznie usunąć dostęp dla tych użytkowników. - Możesz łatwo wyświetlić informacje o ograniczeniach domen stosowanych na stronie Klasyfikacja.   **Przykład 1:** **Bezpieczeństwo > Udostępnianie > Dozwolone domeny:** miro.com, gmail.com  **Dozwolone domeny dla zabezpieczeń:** miro.com  ***Rezultat:*** Udostępnianie tablicy za pomocą bezpośredniego zaproszenia e-mail jest ograniczone do adresów e-mail kończących się na miro.com. Chociaż gmail.com jest dozwolony w ustawieniach Bezpieczeństwo > Udostępnianie > Dozwolone domeny, nie jest dozwolony przez zabezpieczenie.  **Przykład 2:** **Bezpieczeństwo > Udostępnianie > Dozwolone domeny:** miro.com, gmail.com  **Dozwolone domeny Guardrail:** example.org, example.com  ***Rezultat:*** Udostępnianie tablic za pośrednictwem bezpośredniego zaproszenia e-mail nie jest dozwolone dla żadnej domeny, ponieważ nie ma nakładania się między tymi dwoma listami. | Udostępnianie tablic za pośrednictwem bezpośredniego zaproszenia e-mail jest ograniczone do użytkowników, których adresy e-mail należą do dozwolonych domen na tej liście. Te zabezpieczenie nie wpływa na dostęp przyznawany przez linki zespołowe, organizacyjne lub publiczne, ponieważ są one kontrolowane przez oddzielne zabezpieczenia.  Jeśli tablica została już udostępniona na adresy e-mail, które nie znajdują się na tej liście, osoby, które już mają dostęp do tablicy, nadal będą miały dostęp.   This guardrail is designed to work with the [**Bezpieczeństwo > Udostępnianie > Dozwolone domeny**](../data-security/07-sharing-policy-on-enterprise-plan.md), które można skonfigurować zarówno na poziomie organizacji, jak i zespołu. Zobacz kolumnę z opisem, aby uzyskać szczegółowy opis i przykłady. |
