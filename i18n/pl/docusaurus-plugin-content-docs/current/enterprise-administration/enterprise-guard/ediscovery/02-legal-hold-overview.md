---
title: "Przegl\u0105d prawnej blokady danych"
article_id: 21922434361618
translation_id: 21922434361618
locale: pl-pl
sidebar_position: 1
created_at: '2024-10-11T12:20:34Z'
updated_at: '2025-11-25T15:48:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

Funkcja prawnej blokady danych jest zaprojektowana w celu wsparcia procesów zgodności i eDiscovery poprzez zachowanie tablic, które są przedmiotem dochodzenia lub są istotne dla trwających spraw prawnych.

[Administratorzy eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) mogą zapobiec trwałemu usunięciu treści poprzez tworzenie prawnych blokad danych opartych na określonych użytkownikach i ich działaniach w Miro. Ta funkcjonalność jest niezbędna do zapewnienia, że istotne informacje są zachowane i zabezpieczone w trakcie postępowania sądowego.

Na przykład, gdy użytkownik objęty prawną blokadą danych wchodzi w interakcję z tablicą, ta tablica jest automatycznie objęta blokadą, aby zapobiec jej trwałemu usunięciu.

Dodatkowo, wszystkie wersje tablicy są również zachowane, co zapewnia, że treść tablicy jest przechowywana do celów prawnych.

![legalholdoverview.png](images/26679482126098_legalholdoverview.png)

:::note
Musisz mieć [rolę administratora eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md), aby wykonywać zadania związane z prawną blokadą danych. Aby poprosić o rolę administratora eDiscovery, skontaktuj się z administratorem firmy.
:::

## Kluczowe korzyści prawnej blokady danych

- **Zachowanie informacji:** Prawna blokada danych zapewnia, że wszystkie istotne dane są zachowane, zapobiegając trwałemu usunięciu. Jest to kluczowe dla zgodności i dochodzeń prawnych, ponieważ gwarantuje, że dane przedstawiane w sprawach prawnych pozostają dokładne i niezmienione.
- **Zgodność z wymaganiami prawnymi:** Prawna blokada danych wspiera organizacje w przestrzeganiu obowiązków prawnych i regulacyjnych poprzez zapewnienie, że niezbędne informacje są przechowywane i dostępne w razie potrzeby, co pomaga uniknąć kar lub wyzwań prawnych.
- **Łagodzenie ryzyka:** Chroniąc ważne dane, prawna blokada danych zmniejsza ryzyko utraty danych, które mogłoby skutkować poważnymi konsekwencjami prawnymi lub finansowymi.
- **Audyt i monitorowanie:** Za każdym razem, gdy tworzona lub modyfikowana jest prawna blokada danych, generowany jest dziennik audytu, zapewniając pełną widoczność i śledzenie. Wszystkie dzienniki audytu w organizacji są przechowywane bezterminowo, gdy co najmniej jedna prawna blokada danych jest aktywna. Zapewnia to rozliczalność i przejrzystość w zarządzaniu prawnymi blokadami danych.

## Jak działa prawna blokada danych

- **Interakcje z użytkownikiem lub tablicą:** Gdy użytkownik objęty prawną blokadą danych otwiera, modyfikuje lub w jakikolwiek sposób wchodzi w interakcję z tablicą (zmieniając nazwę lub dodając zawartość), tablica ta zostaje oznaczona i zachowana. Na przykład, jeśli nazwa tablicy zostanie zmieniona lub zawartość zaktualizowana, zostanie automatycznie umieszczona pod prawną blokadą danych. Dodatkowo, własność tablicy i tworzenie tablic są wstrzymane.

  Kiedy tworzona jest prawna blokada danych, ma ona zastosowanie do tablic, które opiekunowie utworzyli, są ich właścicielami lub współwłaścicielami w momencie blokady. Ponadto, wszelkie tablice, do których opiekunowie uzyskują dostęp i które modyfikują po nałożeniu blokady, są również uwzględnione. Historia dostępu do tablicy i szczegóły aktualizacji nie są dostępne w tej wersji.
- **Działania użytkownika i usuwanie tablic:** Podczas gdy użytkownicy końcowi mogą usuwać tablice, te tablice są zachowane, jeśli nałożona jest prawna blokada danych. Pozostają niedostępne dla użytkownika końcowego, ale są przechowywane do celów prawnych i administracyjnych.
- **Kontrola administracyjna:** Administratorzy eDiscovery mogą tworzyć i usuwać prawne blokady danych w sekcji eDiscovery w ustawieniach. Prawna blokada danych może być zastosowana do wszystkich tablic utworzonych, będących własnością, współwłasnością, edytowanych lub do których uzyskano dostęp przez użytkownika. Aby zarządzać wieloma prawnymi blokadami danych, administratorzy mogą najpierw utworzyć sprawę, w ramach której te blokady będą pogrupowane.
- **Usunięcie zespołu:** Jeśli tablica objęta prawną blokadą danych istnieje w zespole, ten zespół nie może być trwale usunięty, dopóki blokada nie zostanie zwolniona. To zapobiega niezamierzonej utracie danych, zapewniając, że cała istotna zawartość zostanie zachowana. W przypadkach, gdy zespół zostanie usunięty, ale zawiera tablicę objętą prawną blokadą danych, zespół ten zostanie oznaczony jako zachowany na stronie usuniętych zespołów, a jego trwałe usunięcie zostanie wyłączone do czasu zwolnienia prawnej blokady danych.
- **Perspektywa administratora i eDiscovery:** Podczas gdy użytkownicy końcowi nie mają dostępu do usuniętej tablicy, która jest wstrzymana, administratorzy i zespoły eDiscovery mogą nadal z nią współpracować. Tablica jest zachowana do momentu zamknięcia sprawy, po czym prawna blokada danych może zostać zniesiona, a tablica trwale usunięta.
- **Funkcjonalność eksportu tablicy:** Tablice objęte prawną blokadą danych wciąż można eksportować za pomocą funkcji eksportu tablicy, co umożliwia łatwe zebranie istotnych danych do spraw prawnych.
- **Przenoszenie tablic:** Tablice objęte prawną blokadą danych nie mogą być przenoszone poza organizację. Jeśli tablica jest objęta prawną blokadą danych, zespoły zewnętrzne są automatycznie filtrowane z listy zespołów, do których tablica może zostać przeniesiona.
