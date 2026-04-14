---
title: Przepływy
article_id: 29687970855442
translation_id: 29687970855442
locale: pl-pl
sidebar_position: 5
created_at: '2025-09-23T12:18:02Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: template-picker
availability:
  notes: 'Kto może to zrobić: Członkowie zespołu Które abonamenty: Free, Starter,
    Business, Enterprise, Education Na których platformach: Przeglądarka, Aplikacja
    desktopowa, Mobilna'
---

Przepływy umożliwiają łączenie formatów na planszy w celu tworzenia przepływów pracy zasilanych przez AI. Każdy format działa jako dane wejściowe dla następnego, przekształcając złożone, wieloetapowe procesy, takie jak planowanie sprintu, pisanie briefów czy wykorzystanie danych klientów, w zautomatyzowane przepływy.

Aby dowiedzieć się, które formaty wspierają przepływy, zobacz Wsparte formaty.

Ten artykuł wyjaśnia, jak używać przepływów. Aby uzyskać ogólne informacje o przepływach, zobacz [Przegląd przepływów](04-flows-overview.md).

:::tip
Znajdź gotowe szablony przepływów w [selektorze szablonów](../../getting-started/start-here/your-first-board/04-templates.md).
:::

## Tworzenie i uruchamianie przepływu

Poniższa procedura wykorzystuje podstawowe elementy UX przepływów do stworzenia przepływu od podstaw. Aby rozpocząć tworzenie przepływów szybciej, zobacz elementy UX przepływów.

Postępuj zgodnie z tymi krokami:

1. Dodaj obsługiwany format lub blok instrukcji AI na planszy.
2. (Opcjonalnie) Połącz dowolny istniejący format lub blok instrukcji z formatem, który właśnie dodałeś. Użyj diamentowych łączników AI, aby połączyć swój przepływ.
3. Nad formatem kliknij pasek **TASK**.
   Pasek **TASK** rozwinie się do pola, w którym możesz określić prompt dla tej pozycji w swoim przepływie.
4. W polu **TASK** dodaj swój prompt. Na przykład w dokumencie możesz wygenerować Dokument Wymagań Produktu (PRD). Możesz użyć wyników z dowolnego połączonego formatu lub bloku instrukcji AI.

   > 💡 Pole **TASK** umożliwia wybranie dużego modelu językowego (LLM), dostawcy wiedzy lub wyszukiwania w internecie. W lewym dolnym rogu wybierz model AI, bazę wiedzy lub przeszukaj sieć. Opcje różnią się w zależności od formatu.
5. (Opcjonalnie) Aby utworzyć nowy wynik, kliknij po prawej stronie diamentowy łącznik AI.
   Otworzy się menu **Utwórz nowy wynik**.
6. (Opcjonalnie) Aby dodać nowe wejście, po lewej stronie kliknij diamentowy łącznik Miro AI.
   Otworzy się menu **Utwórz nowe wejście**.
7. Aby ukończyć przepływ, powtórz kroki 1-6 w razie potrzeby.
8. Aby uruchomić przepływ, w pasku **TASK** kliknij **Uruchom**.
   ![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)*Menu kontekstowe **Wybrany przepływ** pokazuje, ile kroków zawiera przepływ.*

## Użyj wiedzy z przepływami

Wiedza integruje się z dostawcami takimi jak Glean, wyszukiwarka internetowa i Miro Insights, aby pobrać wszystko, co Twoja firma wie, korzystając z wewnętrznych i zewnętrznych źródeł.

Dla dowolnego formatu w Twoim przepływie kliknij pasek **TASK**. Pasek **TASK** się rozwinie. W lewym dolnym rogu wybierz i połącz swoją bazę wiedzy.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Określ wewnętrzną bazę wiedzy dla swojego przepływu*

Możesz przekształcać dane z własnych zasobów wiedzy w formaty takie jak dokumenty, tabele, karteczki i slajdy. Następnie połącz każdy format, aby użyć swoich danych jako wejścia lub wyjścia przepływu.

**Więcej informacji:** Zobacz [Wiedza](09-knowledge.md).

## Cofnięcie wyniku w przepływie

Możesz cofnąć wynik dla dowolnego formatu w swoim przepływie. Na przykład, przypadkowo uruchamiasz przepływ i nadpisujesz dokument.

Aby przywrócić Format w swoim przepływie do wcześniejszego stanu, kliknij na pasku **TASK**. Pasek **TASK** rozwinie się. Na dole po prawej stronie, kliknij ikonę w lewo. Wybierz dowolną wersję z ostatnich 24 godzin, aby ją przywrócić.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Funkcja przywracania pozwala na odtworzenie dowolnej wersji swojego Formatu z ostatnich 24 godzin.*

## Elementy UX przepływów

Zrozumienie poniższych elementów UX przepływów pomoże Ci szybciej rozpocząć tworzenie przepływów.

### Konektor Miro AI

Obsługiwane formaty i bloki instrukcji mają diamentowy łącznik Miro AI z lewej strony, który umożliwia podłączenie wejścia, oraz z prawej strony, które łączy wyjście.

Kliknij łącznik Miro AI po dowolnej stronie, aby otworzyć menu **Utwórz nowe wejście** lub **Utwórz nowe wyjście**.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)

*Kliknij łącznik Miro AI, aby otworzyć menu wejścia i wyjścia.*

:::tip
Możesz także przeciągnąć łącznik Miro AI do istniejącej zawartości.
:::

### Inteligentne podświetlanie łączników

Kliknij dowolny obiekt w swoim przepływie, aby zobaczyć tylko te połączenia.

### Ukryj łączniki przepływu

W przypadku złożonych przepływów z wieloma połączeniami możesz ukryć wszystkie łączniki przepływów, aby uprościć widok.

Na pasku [Tablica](../working-on-the-board/02-miro's-new-simplified-user-interface.md) kliknij pionowe trzy kropki. Następnie wybierz **Wyświetlanie**. Przełącz **Pokaż/Ukryj łączniki przepływów** w pozycję wyłączone. Aby pokazać wszystkie łączniki przepływów, przełącz na włączone.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Pokaż lub ukryj wszystkie łączniki przepływów na swojej tablicy.*

:::note
**Pokaż/Ukryj łączniki przepływów** wpływa tylko na wyświetlanie twojej tablicy. Współpracownicy mogą zmieniać swoje własne ustawienia.
:::

### Prompt na Format

Możesz wywołać dowolny format lub blok instrukcji w swoim przepływie, co zapewnia, że każdy format w łańcuchu może wykonywać wyspecjalizowane zadanie w ramach przepływu.

Kliknij pasek **TASK** nad dowolnym formatem w swoim przepływie. Pasek **TASK** się rozwinie. Dodaj swój prompt i opisz, jak chcesz, aby format czytał treść wejściową lub dowolną treść na tablicy, oraz określ zasady i rezultat dla następnego formatu w przepływie.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Pole prompt on-Format pojawia się w pasku **TASK** nad każdym formatem w przepływie.*

### Blok instrukcji dla AI

Możesz wybrać model dużego języka (LLM) lub dowolnego dostępnego [dostawcę wiedzy](09-knowledge.md), aby uruchomić prompt w osobnym bloku, w dowolnym miejscu w Twoim przepływie.

Dla danego formatu kliknij diamentowy konektor Miro AI. W menu wejścia lub wyjścia wybierz **AI** **Instrukcję**.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Bloki instrukcji umożliwiają łańcuchowe łączenie instrukcji, przyjmowanie wejścia i przekazywanie wyjścia do następnego formatu.*

### Globalny przycisk uruchamiania

Możesz rozpocząć swoją pracę z dowolnego Formatu lub bloku instrukcji AI w przepływie. Kliknij, aby wybrać Format lub blok. Pojawi się menu kontekstowe **Przepływ wybrany** obok paska Współpracy.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Menu kontekstowe Przepływ wybrany*

Menu **Przepływ wybrany** pokazuje, ile kroków pozostało do wykonania. Aby uruchomić przepływ, kliknij **Uruchom**.

## Obsługiwane formaty

Przepływy obsługują następujące formaty Miro.

- Diagramy
- Dokumenty
- Obrazy
- Osadzanie kodu iFrame
- Kanban
- Prototypy
- Slajdy
- Tabele
- Oś czasu
