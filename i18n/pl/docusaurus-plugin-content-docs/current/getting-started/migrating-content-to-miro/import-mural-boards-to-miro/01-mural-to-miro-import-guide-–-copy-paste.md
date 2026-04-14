---
title: Przewodnik importu z Mural do Miro – Kopiuj-wklej
article_id: 22957521683986
translation_id: 22957521683986
locale: pl-pl
sidebar_position: 1
created_at: '2024-11-29T13:36:36Z'
updated_at: '2025-11-25T15:49:05Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Lista osób: Użytkownicy z uprawnieniami do edycji Abonamenty: Bezpłatna
    wersja, Starter, Business, Enterprise, Education Platformy: Przeglądarka, aplikacja
    komputerowa, urządzenia mobilne.'
---

Możesz przenieść treści z tablic Mural do Miro, używając metody kopiuj-wklej. Ten przewodnik dostarcza najlepsze praktyki dla tej metody importu, wyjaśnia proces krok po kroku i szczegółowo opisuje, czego możesz się spodziewać w zakresie wyglądu i zachowania różnych obiektów po ich wklejeniu do Miro.

## Wytyczne dotyczące importu z Mural

Stosowanie się do tych wytycznych pomoże Ci osiągnąć najlepsze wyniki podczas przenoszenia treści z Mural do Miro.

W przypadku ustrukturyzowanych danych, takich jak mapy myśli Mural Mind, metoda kopiuj-wklej jest zazwyczaj najlepszym podejściem, aby uniknąć zrywania połączeń między elementami.

:::note
Aby zaimportować treści do Miro za pomocą tej metody, treści w Mural muszą być objęte licencją pełną lub bezpłatną ograniczoną w Mural.
:::

Metoda kopiuj-wklej jest również zalecana do importowania pojedynczych widżetów, które nie są obsługiwane przez [przewodnik importu Mural do Miro (PDF)](02-mural-to-miro-import-guide-–-pdf.md), lub dla widżetów, które nie są importowane z wysoką wiernością przy użyciu metody PDF.

Zwróć uwagę na pewne ograniczenia metody kopiuj-wklej: niektóre atrybuty stylowania oraz obrazy, które zostały pierwotnie przesłane do Mural (a nie połączone przez URL), nie zostaną skopiowane do schowka, a zatem nie zostaną przeniesione do Miro.

## Skopiuj i wklej zawartość Mural do Miro

Poniższa procedura wyjaśnia, jak skopiować zawartość z tablicy Mural i wkleić ją na tablicę Miro.

**Wymagania wstępne**

Upewnij się, że masz uprawnienia do edycji zarówno na tablicy źródłowej w Mural, jak i na tablicy docelowej w Miro.

Aby skopiować zawartość z tablicy Mural i wkleić ją na tablicę Miro:

1. W Muralu wybierz obiekty, które chcesz skopiować.
   > 💡 Aby zaznaczyć wszystkie obiekty na tablicy Mural, użyj skrótu klawiszowego **Ctrl+A** (Windows) lub **Cmd+A** (Mac).
2. Aby skopiować wybrane obiekty, użyj skrótu klawiaturowego **Ctrl+C** (Windows) lub **Cmd+C** (Mac).
   Obiekty Mural zostały teraz skopiowane do schowka.
3. W Miro otwórz tablicę, na którą chcesz wkleić zawartość. Użyj skrótu klawiaturowego **Ctrl+V** (Windows) lub **Cmd+V** (Mac), aby wkleić.

   Pomyślnie skopiowano i wklejono treść z Mural do Miro.
   > ✏️ Treści wklejone z Mural mogą wymagać ręcznego dostosowania w Miro. Niektóre aspekty stylizacji i formatowania mogą wyglądać inaczej po wklejeniu.

## Wygląd obiektu po wklejeniu

Obiekty z Mural zazwyczaj można kopiować i wklejać do Miro z pewnymi różnicami w stosunku do ich pierwotnego stanu. Ta sekcja opisuje oczekiwane wyniki dla niektórych powszechnych obiektów i dostarcza najlepsze praktyki tam, gdzie to możliwe.

### Obszary

Obszary z Mural kopiuj-wklej jako ramki i kształty Miro.

Obszar Mural o 100% przezroczystości pokaże przezroczystą, ale widoczną krawędź po wklejeniu do Miro. Jeśli obszar Mural ma tytuł, to ten tytuł pojawia się i zachowuje w Miro jako tytuł ramki.

![Obszar Muralu z tytułem, oraz całkowicie przezroczystym tłem i obramowaniem.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Obszar swobodnej formy Mural z tytułem, 100% przezroczystym tłem i obramowaniem*

![Wklejony obszar z Mural do Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Wklejony obszar z Mural do Miro*

### Łączniki

Łączniki z Mural kopiuj-wklej jako łączniki Miro.

Etykiety łączników, pozycje pionowe i poziome będą wklejane do Miro jako wyśrodkowane. Miro obsługuje tylko etykiety łączników wyśrodkowane.

Jeśli chodzi o rodzaje łączników, Miro obsługuje linie *ciągłe*, *kropkowane* i *przerywane*. Mural dodatkowo zawiera typ łącznika *z luźnymi kreskami*. Miro mapuje typy konektorów wklejone z Mural w następujący sposób: *solid* mapuje do *solid*, a typ *loosely dashed* z Mural mapuje do typu *dashed* w Miro. Inne bezpośrednie dopasowania (jak kreskowane do kreskowane) są również zachowane.

Miro obsługuje każdy typ krzywej łącznika Mural, chociaż ich wygląd w Miro może się nieznacznie różnić.

![Krzywa połączeniowa Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Krzywa łącząca Mural*

![Krzywa łącznika Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Krzywa łącznika Miro*

### GIF-y i obrazy

GIF-y i obrazy, które pierwotnie dodano do Mural z adresu URL, można kopiować i wklejać do Miro.

> GIF lub obraz w Mural przesłany bezpośrednio z urządzenia lub dodany z paska narzędzi Mural nie może być kopiowany i wklejany do Miro za pomocą tej metody.

### Mapy myśli

Mapy myśli z Mural kopiowane jako mapy myśli Miro, w tym węzeł główny, każdy węzeł podrzędny i ich tekst.

Stylizacja dla węzła głównego jest w większości zachowana. Jednak promień kształtu może się różnić, a rozmiar czcionki tekstu nie jest zachowywany podczas przenoszenia z Mural do Miro.

Węzły podrzędne z Mural są wklejane jako węzły tekstowe w Miro, a ich formatowanie nie jest zachowane.

Kolor i grubość łącznika w mapie myśli mogą się również różnić.

![Mapa myśli skopiowana w Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)
*Mapa myśli skopiowana w Mural*

![Mapa myśli skopiowana z Mural do Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa myśli skopiowana do Miro*

W przypadku map myśli w Mural, które mają wiele poziomów węzłów, kolejność węzłów może się zmienić po wklejeniu do Miro.

![Mapa myśli w Mural z wieloma poziomami węzłów.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa myśli w Mural z wieloma poziomami węzłów*

![Mapa myśli z wieloma poziomami węzłów skopiowana z Mural do Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Mapa myśli z wieloma poziomami węzłów skopiowana z Mural do Miro*

:::tip
Mapy myśli kopiowane z Mural do Miro mogą utracić swoją oryginalną skalę. Aby zmienić rozmiar mapy myśli po wklejeniu, możesz ją ręcznie rozciągnąć na tablicy Miro.
:::

### Kształty

Kształty z Mural są ogólnie wklejane jako kształty Miro. Miro obsługuje większość kształtów Mural bezpośrednio.

Jednak Mural zawiera 16 specyficznych kształtów, które nie mają bezpośredniego odpowiednika w Miro. Te kształty zostaną wklejone do Miro jako prostokąty.

![Wszystkie 16 kształtów, które kopiują się z Murala do Miro jako prostokąty.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Te 16 kształtów, które po skopiowaniu z Mural do Miro zmieniają się w prostokąty*

### Karteczki

Karteczki z Mural wklejane jako karteczki Miro.

Miro przyporządkuje kolor i poziom krycia karteczki do najbliższych dostępnych odpowiedników w Miro.

Następujące różnice mogą również wystąpić, gdy kopiujesz i wklejasz karteczki z Mural do Miro:

- Okrągłe karteczki z Mural zostaną wklejone do Miro jako kwadratowe karteczki.
- Listy w karteczkach Miro nie są zachowane jako interaktywne listy, chociaż poszczególne elementy linii będą wyświetlane na oddzielnych liniach w karteczce Miro.
- Rozmiar czcionki tekstu nie jest zachowywany, ponieważ karteczki Miro automatycznie dostosowują rozmiar czcionki w oparciu o zawartość i rozmiar karteczki.
- Rotacja zastosowana do karteczek w Muralu nie jest zachowywana po wklejeniu.

![Karteczki skopiowane w Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Karteczki skopiowane w Mural*

![Karteczki skopiowane z Mural do Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Karteczki skopiowane do Miro*

### Tabele

Tabele z Mural wklejają się jako tabele Miro.

Mogą pojawić się następujące różnice podczas kopiowania i wklejania tabel z Mural do Miro. Dla każdego z tych elementów możesz zazwyczaj przywrócić swoje preferencje ręcznie w Miro po wklejeniu:

- Tabele umieszczone na innych obiektach w Mural (jak obszary, kształty lub obrazy) mogą być częściowo ukryte za tymi obiektami po wklejeniu do Miro. Może być konieczne dostosowanie ich warstwowania (przenieść na wierzch).
- Kolor obramowania jest ignorowany; obramowania zostaną wklejone jako szare.
- Przezroczystość tła jest ignorowana. Przezroczyste komórki w Mural zostaną wklejone jako białe komórki w Miro. Jednak sam kolor tła (jeśli nie jest przezroczysty) jest zazwyczaj zachowany.
- Rodzina czcionek tekstu jest ignorowana; tekst zostanie wklejony z domyślną czcionką tabeli Miro (RobertPro).
- Formatowanie tekstu, takie jak pogrubienie i kursywa, jest ignorowane w komórkach tabeli.

![Tabela z mieszanym formatowaniem skopiowana w Mural.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tablica ze zróżnicowanym formatowaniem skopiowana do Mural*

![Tabela z mieszanym formatowaniem skopiowana z Mural do Miro.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tablica z mieszanym formatowaniem kopiowana do Miro*

### Tekst

Obiekty tekstowe z Mural wklejane jako obiekty tekstowe w Miro. Oryginalne rodziny czcionek Mural nie są zachowane. Miro odwzorowuje rodzinę czcionek Mural na najbliżej pasującą czcionkę dostępną w Miro i skalują wklejony tekst dla najlepszych wyników na tablicy Miro.
