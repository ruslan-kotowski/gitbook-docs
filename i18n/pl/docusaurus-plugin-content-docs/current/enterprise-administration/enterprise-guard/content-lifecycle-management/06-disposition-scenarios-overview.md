---
title: "Przegl\u0105d scenariuszy usuwania"
article_id: 19596032332434
translation_id: 19596032332434
locale: pl-pl
sidebar_position: 6
created_at: '2024-06-17T17:24:29Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## Automatyczne przenoszenie tablic do kosza

Tablice są automatycznie przenoszone do kosza w wyznaczonym terminie usuwania. Jeśli na tablicę nie ma wpływu żadna aktywna zasada retencji, jej trwałe usunięcie zostanie określone przez zasady kosza.
![disposition1.png](images/27613208637202_disposition1.png)

Na przykład rozważmy projektową tablicę, która ma być przeniesiona do kosza 1 lipca 2025 roku zgodnie z zasadą usuwania i nie ma na nią wpływu żadna zasada retencji. Tablica zostanie automatycznie przeniesiona do kosza 1 lipca 2025 roku, a następnie trwale usunięta 29 września 2025 roku zgodnie z 90-dniową zasadą kosza.

:::note
Obowiązująca zasada retencji ma pierwszeństwo przed zasadą kosza. Dlatego data trwałego usunięcia tablicy będzie zgodna z obowiązującą zasadą retencji.
:::

Jeśli powiadomienia o usuwaniu są włączone dla zasady, użytkownicy otrzymają powiadomienie zgodnie z ustaloną liczbą dni przed planowanym przeniesieniem tablicy do kosza.

Powiadomienie pojawia się w Aktualnościach Miro i prowadzi bezpośrednio do tablicy. Baner jest również wyświetlany na górze tablicy, ostrzegając użytkownika o nadchodzącej akcji przeniesienia do kosza. właściciele i współwłaściciele tablic mają możliwość zachowania tablicy.

## Usunięcie tablicy zainicjowane przez użytkownika

Gdy właściciel tablicy przenosi tablicę do kosza, zasada usuwania nie wpływa już na cykl życia tablicy. Jeśli żadna aktywna zasada retencji nie dotyczy tablicy, jej trwałe usunięcie będzie zgodne z zasadą kosza.

![disposition2.png](images/27613208640914_disposition2.png)

Na przykład, rozważ plan operacyjny tablicy zaplanowany do usunięcia na 13 października 2024 roku. Jeśli właściciel tablicy z wyprzedzeniem przeniesie tablicę do kosza 15 maja 2024 roku i na tablicę nie mają wpływu aktywne zasady retencji, będzie ona podlegać zasadzie kosza. Tablica zostanie trwale usunięta 13 sierpnia 2024 roku, zgodnie z 90-dniową zasadą kosza.

:::note
Jeśli na tablicę wpływa aktywna zasada retencji, zasada ta zastąpi zasadę kosza, ustalając datę trwałego usunięcia zgodnie z zasadą retencji.
:::

## Przywracanie tablicy zainicjowane przez użytkownika

Gdy użytkownik przywraca tablicę z kosza, każda odpowiednia zasada usuwania zostaje automatycznie ponownie zastosowana. Zapewnia to, że tablica ponownie wchodzi w cykl życia z przywróconymi wszystkimi oryginalnymi ustawieniami zasad.

![disposition3.png](images/27613208646418_disposition3.png)

Na przykład, jeśli użytkownik przywróci tablicę ze strategią marketingową z kosza 20 czerwca 2024 roku, która wcześniej miała zastosowaną zasadę usuwania na 1 rok, ta zasada zostanie automatycznie ponownie zastosowana po przywróceniu. Nowa data usunięcia tablicy zostanie ponownie obliczona od daty przywrócenia, ustalając zaktualizowaną datę usunięcia na 20 czerwca 2025 roku lub rok od daty, kiedy ta tablica była ostatnio modyfikowana po przywróceniu.

## Powiadomienia o usuwaniu

Powiadomienia o usuwaniu ostrzegają użytkowników z wyprzedzeniem, gdy tablica jest zaplanowana do automatycznego przeniesienia do kosza z powodu braku aktywności, zgodnie z aktywną zasadą usuwania.

- Administratorzy mogą włączyć powiadomienia podczas publikowania zasady.
- Harmonogram powiadomień można konfigurować od 1 do 30 dni przed planowaną datą przeniesienia.
- Powiadomienia są wysyłane zgodnie z ustawioną liczbą dni, kiedy powiadomienie o usuwaniu musi być wysłane przed datą umieszczenia w koszu.

Kiedy tablica wchodzi w okres inspekcji:

- Powiadomienie pojawia się w aktualnościach użytkownika.
- Kliknięcie jej otwiera tablicę z górnym banerem ostrzegającym o nadchodzącym przeniesieniu do kosza.
- Użytkownicy mogą zdecydować się na zachowanie tablicy, co resetuje licznik usuwania.

Ten mechanizm powiadomień dotyczy wszystkich scenariuszy, w których:

- Aktywna jest zasada usuwania z powiadomieniami.
- Tablica wchodzi w okres inspekcji (według ustawionej liczby dni przed datą usuwania).

### Scenariusz 1: Tablice zgodne z zasadą usuwania

Te tablice podlegają zasadzie i zostaną przeniesione do kosza po określonym okresie braku aktywności.

Jeśli powiadomienia o usuwaniu są włączone dla zasady, powiadomienie zostanie wysłane zgodnie z określoną liczbą dni, kiedy powiadomienie o usuwaniu musi zostać wysłane przed planowanym przeniesieniem tablicy do kosza. Tablica będzie również wyświetlać baner umożliwiający użytkownikom jej przegląd lub zachowanie.

### Scenariusz 2: Tablice z etykietą klasyfikacji dodaną po ostatniej modyfikacji tablicy.

Te tablice są retrospektywnie objęte zakresem i nadal podążają za tym samym harmonogramem usuwania, opartym na dacie ostatniej modyfikacji.

Jeśli powiadomienia o usuwaniu są włączone, użytkownicy otrzymają powiadomienie zgodnie z określoną liczbą dni, kiedy powiadomienie o usuwaniu musi zostać wysłane przed planowanym przeniesieniem do kosza, nawet jeśli etykieta została zastosowana po ostatniej edycji.

### Scenariusz 3: Tablice z etykietą klasyfikacji usuniętą przed opublikowaniem zasady.

Te tablice nie podlegają już zasadzie i są wyłączone z oceny usuwania.

Ponieważ są poza zakresem, nie zostaną wysłane żadne powiadomienia o usuwaniu.

### Scenariusz 4: Tablice niedawno zmodyfikowane i jeszcze nie podlegające progowi usuwania.

Te tablice zostały niedawno zedytowane i jeszcze nie kwalifikują się do usuwania.

Powiadomienie zostanie wysłane tylko wtedy, gdy tablica wejdzie w okres inspekcji — to znaczy zgodnie z określoną liczbą dni, kiedy powiadomienie o usuwaniu musi zostać wysłane przed datą usuwania. Do tego czasu żadne powiadomienie nie zostanie uruchomione.

### Scenariusz 5: Tablice zmodyfikowane po wejściu w inspekcję

Gdy tablica wejdzie w okres inspekcji, jej data usuwania zostaje zablokowana. Oznacza to, że chyba że właściciel tablicy wyraźnie zdecyduje się ją zachować, zostanie ona automatycznie przeniesiona do kosza w zaplanowanym terminie.

Modyfikowanie lub uzyskiwanie dostępu do tablicy w trakcie okresu inspekcji nie wpływa na harmonogram usuwania. Następujące działania nie zmienią wyniku usuwania: edycja lub wyświetlanie tablicy, zmiana jej etykiety klasyfikacyjnej lub zespołu, a nawet usunięcie powiązanej zasady.

Jeśli powiadomienia o usuwaniu są włączone, powiadomienie zostanie wysłane na podstawie skonfigurowanej liczby dni, kiedy powiadomienie o usuwaniu musi być wysłane przed zaplanowaną datą przeniesienia do kosza, a na tablicy zostanie wyświetlony baner umożliwiający użytkownikowi jej przegląd lub zachowanie.

### Scenariusz 6: Tablice, które zostały już usunięte lub ręcznie przeniesione do kosza

Te tablice zostały już usunięte z przestrzeni roboczej i nie są już zarządzane przez zasady usuwania.

Powiadomienia o usuwaniu nie są wysyłane dla tablic, które są już w koszu lub zostały trwale usunięte.

### Scenariusz 7: Tablice objęte wieloma zasadami

Tablice mogą podlegać więcej niż jednej aktywnej zasadzie usuwania jednocześnie, szczególnie jeśli wiele zasad dotyczy tej samej etykiety klasyfikacyjnej lub zespołu.

Jeśli do tablicy zastosowano więcej niż jedną zasadę z włączonymi powiadomieniami, użytkownik otrzyma tylko jedno powiadomienie, gdy tablica wejdzie w inspekcję. Powiadomienie bazuje na zasadzie z najwcześniejszą zaplanowaną datą usunięcia i jest wysyłane na określoną liczbę dni przed tą datą, zgodnie z ustawieniami.

## Scenariusz 8: Tablice już w stanie kontroli, a zasada usuwania zostaje następnie skasowana.

Jeśli tablica już weszła w okres inspekcji i powiadomienia o usuwaniu zostały wysłane (jeśli były włączone), zaplanowana data usunięcia zostaje zabezpieczona. Nawet jeśli powiązana zasada usuwania zostanie później skasowana lub zmodyfikowana, tablica zostanie automatycznie przeniesiona do kosza w oryginalnej dacie usunięcia — chyba że właściciel tablicy zdecyduje się ją zachować.

Natomiast jeśli zasada zostanie usunięta przed wejściem tablicy w okres inspekcji, tablica będzie uważana za wyłączoną z zakresu i nie zostanie przeniesiona do kosza.
Zapewnia to, że gdy użytkownicy zostaną powiadomieni, czynność usuwania pozostanie spójna i przewidywalna, niezależnie od późniejszych zmian w zasadach.
