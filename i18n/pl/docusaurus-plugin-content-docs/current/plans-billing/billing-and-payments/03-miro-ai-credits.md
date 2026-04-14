---
title: Tokeny na Miro AI
article_id: 19756209116178
translation_id: 19756209116178
locale: pl-pl
sidebar_position: 3
created_at: '2024-06-25T21:32:21Z'
updated_at: '2026-03-04T08:31:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Kto może to zrobić: Wszyscy użytkownicy, administratorzy rozliczeń, administratorzy
    firm Jakie abonamenty: Free, Starter, Business, Enterprise Na jakich platformach:
    Przeglądarka, komputer, urządzenia mobilne'
---

Tokeny na AI umożliwiają korzystanie z funkcji AI w Miro. Za każdą czynność AI, którą wykonasz, zużywasz tokeny na AI.

Miro przydziela określoną liczbę tokenów na AI na Twoje konto co miesiąc. Saldo [zależy od Twojego abonamentu](#ai-credits-per-plan).

Dla abonamentów Enterprise i Free Twoje saldo resetuje się w pierwszym dniu każdego miesiąca kalendarzowego. Dla abonamentów Starter i Business Twoje saldo resetuje się co miesiąc w dniu odnowienia abonamentu. Na przykład, jeśli masz roczną subskrypcję, a data odnowienia przypada na 3 marca, saldo resetuje się trzeciego dnia każdego miesiąca podczas Twojej subskrypcji.

**Więcej informacji:** Zobacz [tokeny na AI według abonamentu](#ai-credits-per-plan).

Gdy na koncie zabraknie tokenów na AI, w Miro otwiera się okno modalne, które pokazuje opcje dodatkowych tokenów na AI, w tym płatny [dodatek tokenów na Miro AI](../../using-miro/miro-ai/17-miro-ai-credits-add-on.md).

Każdy członek zespołu może zużywać tokeny na AI, wykonując akcje AI. Goście i odwiedzający nie mogą wykonywać akcji AI i nie zużywają tokenów na AI.

> **Wskazówka:** W płatnych abonamentach można sprawdzić [saldo tokenów na AI](#check-ai-credit).

## Zużycie tokenów na Miro AI

Każda akcja AI zużywa token na AI z Twojej miesięcznej puli. Na przykład, [dodatek Miro Prototypes](../../using-miro/miroverse/prototyping/07-miro-prototypes-add-on.md) zużywa pięć (5) tokenów na AI generowany ekran, a każde AI generowane zdjęcie zużywa trzy (3).

Poniższa tabela pokazuje zużycie tokenów dla generowanych przez AI wyników:

| Wynik AI według funkcji | Zużyte token(y) |
| --- | --- |
| Wyszukiwanie AI | 0 tokenów |
| Nowości | 1 token |
| Diagramy | 5 tokenów |
| Dokument | 2 tokeny |
| Obraz | 3 tokeny |
| Prototypy | 5 tokenów na ekran |
| Usuń tło | 1 token |
| Sidekicks | 2 tokeny |
| Slajdy | 5 tokenów na slajd |
| Karteczka | 1 token |
| Tabele | 5 tokenów |
| Tekst | 1 token na AI |

> **UWAGA:** Współpracownik AI zużywa 2 tokeny na AI za każdym razem, gdy wykonasz prompt. Upewnij się, że Twoje prośby są jak najbardziej szczegółowe, aby zmniejszyć liczbę wykonanych poleceń potrzebnych do osiągnięcia wyniku.

> **UWAGA:** Jeśli Miro AI nie jest w stanie wygenerować wyniku i wyświetli komunikat o błędzie, nie zużywa tokenu na AI.

> **UWAGA:** Funkcje dostępności, takie jak generowanie tekstu alternatywnego dla obrazu, nie zużywają tokenów na AI.

### Przykładowe scenariusze zużycia tokenów na AI

#### Generowanie prototypu dla przepływu UX

Używasz dodatku Miro Prototypes, aby wygenerować 6 ekranów dla przepływu wdrażania.

Na podstawie Twojego promptu, Miro AI generuje 6 indywidualnych ekranów prototypu, które możesz edytować.

- **Przybliżone zużycie tokenów:** 30 tokenów na AI.
- **Podział zużycia:** 5 tokenów na AI na ekran dla 6 ekranów (5*6) = 30 tokenów na AI zużytych.

#### Utwórz i rozwijaj prezentację slajdów

Generujesz zestaw slajdów ze strategią na podstawie notatek na tablicy, a następnie rozwijasz określone slajdy.

Miro AI skanuje Twoją tablicę w poszukiwaniu kontekstu i tworzy uporządkowaną prezentację slajdów składającą się z 10 slajdów, każdy z rozmieszczeniem, tekstem i wizualizacjami.

Następnie zlecasz Miro AI przepisanie slajdu "Podsumowanie wykonawcze" oraz dodanie jednego nowego slajdu o nazwie "Następne kroki".

- **Przybliżone zużycie tokenów:** 60 tokenów na AI.
- **Analiza zużycia:**
  - 5 tokenów na AI za każdy z 10 slajdów (5*10) = 50 tokenów na AI.
  - Dodatkowo 5 tokenów na AI za iterację slajdu 'Podsumowanie Wykonawcze'.
  - Dodatkowo 5 tokenów na AI za wygenerowanie dodatkowego slajdu 'Następne kroki'.

> **Wskazówka:** Twórz każde polecenie tak szczegółowe, jak to możliwe, aby użyć jak najmniejszej liczby tokenów na generację.

## Tokeny na AI na abonament

Poniższa tabela pokazuje, ile tokenów przydzielanych jest miesięcznie na każdy abonament.

| Abonament | Tokeny na AI |
| --- | --- |
| Free | 10 tokenów/miesiąc |
| Starter | 25 tokenów/licencja/miesiąc |
| Business | 50 tokenów/licencja/miesiąc |
| Enterprise | Zmienny w zależności od poziomu licencji. Zobacz Tokeny na AI dla Enterprise. |
| Education | 100 tokenów/miesiąc |

:::note
[Dodatek Miro Prototypes](../../using-miro/miroverse/prototyping/07-miro-prototypes-add-on.md) zawiera co najmniej 350 dodatkowych tokenów na Miro AI dla organizacji miesięcznie. Administratorzy firmy (Enterprise) mogą określić wyższą liczbę ze swoim administratorem konta Miro.
:::

Dla Twojej organizacji Miro wykorzystuje tokeny na licencję do obliczenia miesięcznej puli tokenów na AI. Każda akcja AI przeprowadzona w organizacji zużywa token z tej puli.

Jeśli dodasz lub usuniesz użytkowników w trakcie cyklu rozliczeniowego, Miro dynamicznie dostosowuje przydział tokenów. Twój przydział tokenów na AI jest aktualizowany, aby pasować do nowej wielkości zespołu na kolejnej dacie rozliczenia.

(Enterprise, Free) Miesięczna pula tokenów na Miro AI resetuje się pierwszego dnia każdego miesiąca kalendarzowego.

(Business, Starter) Miesięczna pula tokenów na Miro AI resetuje się w dniu odnowienia abonamentu.

:::tip
Aby zwiększyć saldo swoich tokenów na AI, subskrypcje Starter, Business i Enterprise kwalifikują się do zakupu [dodatku tokeny na Miro AI](../../using-miro/miro-ai/17-miro-ai-credits-add-on.md).
:::

### Tokeny na Miro AI dla Enterprise

W subskrypcji Enterprise liczba tokenów przydzielanych na licencję na miesiąc zależy od [poziomu licencji](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md). Administratorzy firmy mogą monitorować przydział i zużycie tokenów na AI w konsoli administracyjnej.

W **konsoli administracyjnej** przejdź do **Rozliczenia** > **Subskrypcja**.

> **UWAGA:** (Enterprise) Warstwy licencji mogą ulec zmianie. Więcej informacji o przydziałach na każdy poziom Enterprise znajdziesz w artykule [Tokeny na Miro AI dla wersji Enterprise](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/03-miro-ai-credits-for-enterprise-plans.md).

## Sprawdź saldo tokenów na AI

W ramach płatnej subskrypcji Miro administratorzy rozliczeń oraz administratorzy firmy mogą w każdej chwili sprawdzić saldo tokenów na AI dla swojej organizacji. Saldo tokenów nie jest wyświetlane w wersji Free.

### Plany Starter i Business

Przejdź do **Konsola administracyjna** > **Rozliczenia**. W widoku **Rozliczenia** pokazane jest użycie tokenów na AI oraz pozostałe saldo.

### Plany Enterprise

Przejdź do **Konsoli administracyjnej** > **Rozliczenia** > **Subskrypcja**. Widok **Subskrypcji** pokazuje zużycie tokenów na AI i pozostały stan konta.

## Dodatek tokenów na Miro AI

Dodatek tokenów na AI to płatna subskrypcja, która zwiększa Twój miesięczny limit tokenów na AI.

**Więcej informacji:** Zobacz [dodatek tokenów na Miro AI](../../using-miro/miro-ai/17-miro-ai-credits-add-on.md).
