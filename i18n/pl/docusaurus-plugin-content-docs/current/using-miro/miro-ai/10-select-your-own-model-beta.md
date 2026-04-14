---
title: Wybierz własny model (wersja beta)
article_id: 29484232754578
translation_id: 29484232754578
locale: pl-pl
sidebar_position: 10
created_at: '2025-09-15T12:50:30Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-sidekicks
availability:
  notes: 'Kto może to zrobić: Członkowie zespołu Które abonamenty: Free, Starter,
    Business, Enterprise Na których platformach: Przeglądarka, Desktop, Mobile'
---

Podczas wykonywania działań AI z przepływami Miro [Flows](04-flows-overview.md) i współpracownikami AI, opcja Select Your Own Model pozwala Ci określić najbardziej odpowiedni model dużego języka (LLM) dla zadania.

Na przykład, w przypadku generowania obrazów możesz zdecydować, czy użyć Stable Diffusion 3.5 Large lub Gemini 2.5 Flash Image (Nano Banana).

Twój wybór może zależeć od złożoności lub specyfiki zadania.

:::tip
Miro Flows i współpracownicy AI mają domyślnie wybrane LLM dla każdego zadania. Gdy nie jesteś pewien, jaki model wybrać, najlepszym rozwiązaniem jest użycie domyślnego modelu. Domyślny model jest oznaczony etykietą Polecany.
:::

Wybór modelu jest dostępny tylko w ramach przepływów i współpracowników AI dla następujących elementów:

- Dokumenty i formaty obrazów we współpracownikach AI i przepływach
- Główna logika współpracowników AI
- Blok instrukcji w przepływach

Ten artykuł wyjaśnia, jak wybrać własny model dla przepływów i współpracowników AI oraz dostarcza informacji, które pomogą Ci wybrać LLM do wspólnych zadań.

## Wybór własnego modelu

### Przepływy

Dokumenty, obrazy oraz Bloki Instrukcji w Przepływie posiadają pole prompt, w którym możesz wybrać własny model.

Postępuj zgodnie z poniższymi krokami:

1. Dodaj Dokument, obraz lub Blok Instrukcji na planszę.
2. Aby uzyskać dostęp do listy dostępnych modeli, kliknij nazwę domyślnego modelu w prawym górnym rogu pola prompt. Na przykład: `AWS | Claude 3.5`.
3. Wybierz model.

Aby dowiedzieć się więcej o tworzeniu Przepływów i interfejsu użytkownika Przepływów, zobacz [Przepływy](05-flows.md).

### Współpracownicy AI

Podczas tworzenia lub edycji współpracowników AI, zobaczysz sekcję **Model (zaawansowany)**, gdzie możesz wybrać, który model chcesz użyć do przetwarzania współpracownika AI, generacji obrazów i dokumentów.

Aby dowiedzieć się więcej o współpracownikach AI, zobacz [dokumentację współpracowników AI](08-ai-sidekicks.md).

## Jak różnią się modele

Duży model językowy (LLM) to zazwyczaj członek rodziny modeli, która obejmuje modele o wysokiej wydajności, modele optymalne oraz najszybsze, ale mniej wydajne modele.

Na przykład, rodzina GPT-5 zawiera GPT-5, GPT-5-mini i GPT-5-nano.

Najszybsze, ale najmniej wydajne modele są idealne dla niskiej latencji.

### Wnioskowanie i brak wnioskowania

Głównym wyróżnikiem między LLM-ami są modele z rozumowaniem i bez niego.

*Rozumowanie* oznacza, że model potrzebuje więcej czasu, aby dostarczyć odpowiedź wyższej jakości.

:::note
*Rozumowanie* nie zawsze oznacza najdokładniejszy wynik. Jeśli potrzebujesz wielu iteracji wyjścia, wysokie rozumowanie może nie być najefektywniejsze.
:::

Dla złożonych zadań, takich jak tworzenie dokumentów skierowanych do klientów, priorytetyzacja i zadania wymagające przetwarzania dużej ilości informacji, model z rozumowaniem jest najlepszym wyborem.

Dla prostych zadań, takich jak sprawdzanie gramatyki, tłumaczenie czy formatowanie tekstu, model bez rozumowania jest najefektywniejszym wyborem.

Poniższa tabela pokazuje kilka modeli z rozumowaniem i bez rozumowania.

| Zdolność do rozumowania | Modele |
| --- | --- |
| Rozumowanie | GPT-5, GPT-5-mini, GPT-5-nano, Claude Sonnet 4, Claude Sonnet 4.5, Gemini 2.5, Gemini 2.5 Flash, o3, o4-mini |
| Brak rozumowania | GPT 4o, GPT-4o-mini, GPT-4.1, GPT-4.1-mini, Claude Sonnet 3.7, Claude Sonnet 3.5, Gemini 2.5 Flash Lite |

### Styl

Każdy LLM ma unikalny "styl". Eksperymentując z różnymi modelami, możesz zauważyć, że określony styl wyników spełnia Twoje wymagania, czy to pod kątem marki, klimatu, czy preferencji.

:::tip
Starsze modele charakteryzują się bardziej wyrazistym stylem, szczególnie pod kątem twórczego i nietuzinkowego podejścia.
:::

## Wybór modelu AI w zależności od zadania

| Zadanie | Modele | Opis |
| --- | --- | --- |
| Burza mózgów | GPT-4o, o3, o4-mini, Sonnet 3.7 | Świetne do myślenia dywergentnego, wybuchów pomysłów na funkcje, o zabawnym tonie i "kreatywnym zacięciu." Używaj do generowania tekstu, na przykład alternatywnych nagłówków i wariantów mikrotreści. |
| Priorytetyzacja i punktacja | GPT-5, Claude Sonnet 4.5, Gemini 2.5 | Najlepsze modele wnioskowania dla spójnej punktacji i przejrzystych uzasadnień. Na przykład RICE/MoSCoW na backlog, pisma dotyczące kompromisów i poziomy roadmapy. |
| Synteza i badania | GPT-5, GPT-5-mini, Claude Sonnet 4.5, GPT-4.1, Claude Sonnet 3.7, Gemini 2.5 Flash | Użyj do zadań o średniej do wysokiej złożoności. Na przykład do tworzenia osobowości z notatek i wyciągania wniosków z danych i baz wiedzy. |
| Schemat & tranformacja | GPT-5-mini, GPT-5-nano, GPT-4.1, Sonnet 3.7, Gemini 2.5 Flash, Gemini 2.5 Flash Lite | Zmiana formatu zazwyczaj nie wymaga złożonego rozumowania, więc zoptymalizowane wersje przyniosą szybsze wyniki, ale trzymaj się nowszych rodzin modeli, aby zapewnić spójność przy pracy z dużymi kontekstami. notatki → dokumenty, dokument → tabela, specyfikacja → diagram) |
| Szybkie edycje tekstu | GPT-4o-mini, Gemini 2.5 Flash Lite, GPT-5-nano, Claude 3.7 | Najbardziej konkurencyjne opcje. Najlepsze do prostych edycji tekstu, takich jak poprawa gramatyki, tłumaczenie i przepisywanie dla lepszej klarowności. |

## Wybieranie modeli do generowania obrazów

Wszystkie duże modele językowe (LLM) wspierane przez Miro mogą przetwarzać tekst i obrazy. Jednak większość z nich nie jest w stanie generować obrazów.

Do generowania obrazów doskonale nadaje się Gemini 2.5 Flash Image (Nano Banana), który skutecznie przekształca Twoje ogólne instrukcje w obraz.

Większość LLM oczekuje opisu obrazu, a nie konkretnych instrukcji. Na przykład: "obraz psa w zabawnym kapeluszu" jako opis w przeciwieństwie do "stwórz zabawny obraz psa" jako instrukcji. Nano Banana potrafi generować obrazy na podstawie konkretnych instrukcji.

:::note
Używaj Nano Banana do ukierunkowanych edycji istniejącego obrazu. Inne modele mogą używać istniejącego obrazu jako odniesienia stylu.
:::

Pod względem szybkości czy jakości wyników, różnice między LLM są niewielkie. Jak w każdym przypadku użycia, możesz eksperymentować z różnymi modelami, aby znaleźć ten, który najlepiej odpowiada Twoim preferencjom.
