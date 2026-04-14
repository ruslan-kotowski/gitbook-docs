---
title: Przewodnik po promptach Miro AI
article_id: 30226743358226
translation_id: 30226743358226
locale: pl-pl
sidebar_position: 1
created_at: '2025-10-14T17:24:22Z'
updated_at: '2025-11-25T15:54:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Lepsze prompty powodują lepsze rezultaty przy pracy z dowolnym modelem AI. Bardziej szczegółowe prompty zazwyczaj tworzą wyniki bardziej zgodne z tym, co masz na myśli. Krótsze, mniej szczegółowe prompty dają modelowi AI więcej swobody w interpretacji tego, czego chcesz, co może prowadzić do zaskakujących wyników.

Ten przewodnik pomoże Ci tworzyć lepsze prompty podczas pracy z funkcjami Miro AI.

## Framework RISEN

Framework RISEN do tworzenia promptów AI to struktura zaprojektowana w celu uzyskania lepszych wyników od samego początku. Uwzględnia:

- **Rola:** Czy AI jest twórcą, doradcą, czy też rozwiązującym problemy? Czy pełni szczególną rolę w Twoim zespole? *Przykłady: „Jesteś starszym projektantem produktu tworzącym…” lub „Jesteś ekspertem pisarzem technicznym doradzającym...”*
- **Informacje wejściowe:** Tutaj dostarczasz informacji potrzebnych AI do wykonania zadania. W Miro może to obejmować informacje pisemne lub kontekst z tablicy. Na przykład przy tworzeniu prototypu możesz uwzględnić funkcje produktu lub które strony należy uwzględnić.
- **Kroki:** Tutaj określasz, co AI ma zrobić. Podawanie ogólnych instrukcji jest możliwe, ale precyzyjne wyjaśnienie, co dokładnie chcesz osiągnąć, przyniesie lepsze rezultaty. *Przykład: „1. Podsumuj materiały dostarczone w kontekście z tablicy. 2. Utwórz karteczkę dla każdego ważnego punktu z materiału. 3. Zorganizuj karteczki w kolejności ich potencjalnego wpływu.”*
- **Oczekiwania:** Jeśli nie określisz, co chcesz, aby AI wygenerowało, AI samo podejmie decyzję, co nie zawsze będzie trafne. Bądź tutaj szczegółowy; zamiast pisać „stwórz zestaw slajdów”, napisz „stwórz zestaw slajdów z dwunastoma slajdami” i opisz, jakie tematy każdy slajd ma poruszać.
- **Ograniczenie:** Jeśli są rzeczy, które *nie* powinny się znaleźć w wyniku, określ to na końcu. Na przykład możesz stworzyć prototyp AI dla procesu finalizacji zakupów online, który *nie* zawiera strony logowania w przepływie.

Definiując każdy z tych parametrów, Miro AI dokładnie będzie wiedział, czego oczekujesz od jego wyniku, co pozwoli stworzyć lepsze rezultaty ogólnie.

## Dodawanie kontekstu z tablicy Miro

Jedną z najpotężniejszych funkcji [Miro AI](../01-miro-ai-overview.md) jest możliwość dodania kontekstu z aktualnej tablicy. Pozwala to na dodanie dużej ilości informacji w zorganizowany sposób, aby poprawić wyniki AI.

Oto kilka wskazówek, jak najlepiej wykorzystać kontekst tablicy:

- **Nie wybieraj wszystkiego na tablicy.** Chociaż może się wydawać, że łatwiej jest wybrać wszystko na tablicy jako kontekst, zawężenie tego do najbardziej istotnych informacji przyniesie najlepsze rezultaty.
- **Dodaj kontekst specyficzny dla branży do tablicy.** Chociaż Miro AI jest potężne, opiera się na ogólnym dużym modelu językowym (LLM), jak większość innych modeli AI. Dodanie dokumentacji specyficznej dla branży, istotnej dla Twojego promptu, pomaga mu uzyskać lepsze wyniki za pierwszym razem. Mogą to być na przykład glosariusz terminów branżowych, przykład konkretnego wyniku, który chcesz uzyskać, lub inne informacje branżowe, które nie są raczej znane osobom spoza Twojej branży.
- **Użyj Miro AI do tworzenia kontekstu.** Jeśli potrzebujesz czegoś w rodzaju briefu projektowego na podstawie notatek ze spotkania, możesz użyć Miro AI, aby stworzyć dokument na swojej tablicy. Wprowadź niezbędne poprawki, a następnie użyj tego jako kontekstu zamiast rozproszonych notatek, które mogą być mylące.

## Miro AI - gotowe prompty startowe

Nowy w Miro AI? Jesteśmy dla Ciebie. Stworzyliśmy gotowe do użycia prompty startowe dla popularnych przepływów pracy. Po prostu zamień miejsca w nawiasach (np. [rola], [artefakt], [ton]) na swój kontekst, a następnie uruchom prompt. Odkryj nasze prompty startowe w podziale na przepływy pracy:

- [Początkowe prompty do generowania i tworzenia pomysłów](02-content-generation-and-ideation-starter-prompts.md)
- [Początkowe prompty do analizy i organizacji treści](03-content-analysis-and-organization-starter-prompts.md)
- [Początkowe prompty do optymalizacji pracy](04-workflow-optimization-starter-prompts.md)

## Wskazówki dotyczące promptów specyficznych dla funkcji

Miro AI oferuje ogólne i specjalistyczne współpracowniki AI, tryb AI, przepływy i narzędzia AI specyficzne dla formatu, aby lepiej skupić się na żądanym wyniku. Jeśli próbujesz stworzyć prototyp, otwórz Miro Prototypes zamiast próbować utworzyć go za pomocą ogólnych współpracowników AI.

### Miro Prototypes

[Miro Prototypes](../../miroverse/prototyping/07-miro-prototypes-add-on.md) pozwala na tworzenie przepływów prototypów jedno- lub wieloekranowych z AI. Skorzystaj z tych wskazówek, aby uzyskać lepsze wyniki przy tworzeniu prototypów:

- Określ ekrany, które ma zawierać prototyp, zwłaszcza jeśli którykolwiek z nich wykracza poza typowy wzorzec UX dla projektowanej ścieżki użytkownika.
- Jeśli masz jakiekolwiek wymagania dotyczące produktu lub projektu (np. kody heksadecymalne dla określonych kolorów), uwzględnij to jako kontekst na swojej tablicy.
- Dołącz zrzuty ekranu podobnych stron lub projektów, które chcesz użyć jako inspirację i umieść je na swojej tablicy.
- Uwzględnij informacje o swoim docelowym użytkowniku w promcie (np. „studenci college'u” lub „liderzy zespołów projektowych”).

### Slajdy Miro

Użyj AI, aby tworzyć [Slajdy](../../formats/02-create-miro-slides-with-ai.md) i przyspieszyć przygotowanie prezentacji. Oto kilka wskazówek, jak tworzyć lepsze zestawy slajdów:

- Zdefiniuj paletę kolorów lub inne kwestie stylu w swoim promcie. Jeśli określiłeś paletę kolorów w Centrum marki Miro, uwzględnij ją w promcie.
- Dodaj treść dla konkretnych slajdów jako dokumenty lub karteczki jako kontekst na tablicy.
- Określ, kto jest Twoją publicznością w promcie (np. „członkowie zarządu” lub „inwestorzy venture capital”).

### Obrazy

Użyj Miro AI do tworzenia obrazów na swoich tablicach. Oto kilka wskazówek, jak tworzyć lepsze obrazy:

- Określ styl obrazu (np. „fotorealistyczny”, „digital painting”, „impresjonistyczny”).
- Uwzględnij istotny kontekst z tablicy, na przykład opis tego, co obraz powinien zawierać (możesz też zawrzeć to w polu promptu, ale jeśli już istnieje na tablicy, uwzględnij to jako kontekst).
- Uwzględnij wszelkie szczegóły, które obraz powinien zawierać (np. „osoba niesie laptopa” lub „na biurku jest stos książek”).
- Im bardziej szczegółowy będzie Twój prompt, tym lepsze będą Twoje początkowe wyniki.

## Edycja i iteracja z Miro AI

Miro AI jest narzędziem wspierającym Twoją pracę, a nie zastępnikiem ludzkich obserwacji i wiedzy. Edycja i iteracja jest ważnym krokiem w tworzeniu lepszych rezultatów, zarówno z użyciem AI, jak i manualnie.

Podczas tworzenia formatów za pomocą Miro AI masz możliwość wprowadzenia edycji przed dodaniem treści do tablicy. W Miro Prototypes i Slajdach Miro możesz edytować jeden ekran lub slajd naraz, ale możesz wykonywać tyle rund edycji, ile potrzebujesz. Możesz również cofnąć się do wcześniejszych wersji w dowolnym momencie przed dodaniem treści do tablicy.

Oto kilka wskazówek dotyczących edytowania z Miro AI:

- Wprowadzaj jedną zmianę na raz podczas dostrajania wyników. Wprowadzanie zbyt wielu instrukcji naraz może skutkować nieoczekiwanymi rezultatami.
- Skup się na treści, a nie na stylu, ponieważ możesz edytować tylko jeden ekran lub slajd naraz.
- Spróbuj użyć różnych sformułowań lub słów kluczowych, jeśli wynik nie jest zgodny z oczekiwaniami.

Jeśli utworzyłeś Format, który chcesz iterować, ale już dodałeś go do tablicy, możesz użyć tego obiektu jako kontekstu do kolejnej iteracji. To dobre rozwiązanie, jeśli chcesz zrobić coś tak prostego, jak zmiana stylu zestawu slajdów, lub jeśli chcesz dodać dodatkowe ekrany w przepływie prototypu.

:::note
Choć wykorzystywanie wcześniejszych prac generowanych przez AI jako kontekstu do tworzenia nowych wersji jest dobrym punktem wyjścia, AI może zmieniać aspekty pracy w oparciu o inne elementy prompta lub dodatkowy kontekst. Upewnij się, że sprawdzasz wszystkie wyniki.
:::
