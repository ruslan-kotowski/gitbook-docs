---
title: Przewodnik importu z Mural do Miro – PDF
article_id: 22856050009362
translation_id: 22856050009362
locale: pl-pl
sidebar_position: 2
created_at: '2024-11-25T14:36:20Z'
updated_at: '2026-01-19T14:43:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Osoby: Użytkownicy z dostępem do edycji Plany: Business, Education, Enterprise,
    Starter Platformy: Przeglądarka, Pulpit'
---

Możesz zaimportować istniejące tablice Mural do Miro, eksportując je z Mural jako pliki PDF, a następnie importując te pliki PDF do Miro. Ten artykuł dostarcza wskazówek dotyczących osiągania najlepszych wyników przy imporcie PDF, wyjaśnia procedurę importu oraz opisuje, czego możesz oczekiwać, gdy różne elementy Mural są importowane do Miro przy użyciu tej metody.

Metoda importu PDF jest szczególnie skuteczna w przypadku treści, które mogą nie być dobrze przenoszone za pomocą kopiowania-wklejania lub importów opartych na API. Importer PDF w Miro analizuje kształty i ich współrzędne w pliku PDF Mural i próbuję odtworzyć oryginalny układ. Na przykład, może interpretować przecinające się linie jako strukturę tabeli.

Należy pamiętać, że niektóre obiekty mogą wyglądać inaczej w Miro po imporcie, a precyzyjne stylizowanie lub układ mogą wymagać ręcznych dostosowań lub odtworzenia w Miro. Ogólnie rzecz biorąc, prostsze treści z mniej skomplikowanym stylizowaniem zazwyczaj pozwalają na uzyskanie bardziej dokładnych wyników importu.

## Wytyczne dotyczące importu z Mural

Aby osiągnąć najlepsze wyniki podczas importowania treści Mural jako PDF, warto zrozumieć, jak działa importer oraz które treści najlepiej się przenoszą. Importer PDF przede wszystkim dopasowuje podstawowe kształty i linie.

:::note
**Notatka:** Aby zaimportować treści do Miro, Twoje treści Mural muszą być objęte pełną lub bezpłatną ograniczoną licencją w Mural.
:::

Przejrzyste odstępy między elementami w Muralu pozwalają importerowi Miro dokładniej analizować treści. Tablica Mural z wieloma elementami tłoczonymi blisko siebie może dać mieszane lub mniej precyzyjne wyniki importu.

Aby uzyskać najwyższą wierność importu, upewnij się, że Twoje treści w Muralu **nie** zawierają następujących atrybutów, ponieważ mogą się one źle przenosić poprzez PDF:

- Niestandardowe czcionki
- Złożone stylizacje, które przekształcają podstawowe kształty (np. mocno zaokrąglone rogi w prostokątach, unikalnie wygięte strzałki)
- Liczne nakładające się kształty i linie
- Obrócone elementy

:::tip
**Wskazówka:** Jeśli potrzebujesz zachować dokładne stylizacje, złożone układy lub precyzyjne współrzędne swoich treści w Muralu, najbardziej niezawodną metodą jest eksport treści z Murala jako statyczny obraz (np. PNG, JPG) i następnie import tego obrazu do swojej tablicy w Miro.
:::

## Importuj tablice z Mural do Miro jako pliki PDF

Ta sekcja wyjaśnia, jak zaimportować zawartość z Mural do Miro, korzystając z funkcji importu PDF.

### Wymagania wstępne do importu PDF

Przed rozpoczęciem procesu importu upewnij się, że spełniasz następujące wymagania wstępne:

- Musisz mieć uprawnienia do edycji tablicy źródłowej w Mural (aby ją eksportować jako PDF).
- Musisz mieć uprawnienia do edycji tablicy docelowej w Miro, na którą zamierzasz zaimportować zawartość.
- Musisz mieć już pobrane tablice z Mural jako pliki PDF.

**Więcej informacji:** Instrukcje dotyczące eksportu z Mural znajdziesz w dokumentacji Mural pod [Eksportuj i pobierz zawartość swojego muralu](https://support.mural.co/s/article/export-and-download-your-mural-s-content) (zewnętrzny link).

### Importuj plik PDF

Postępuj zgodnie z tymi krokami, aby zaimportować pliki PDF z Muralu do Miro:

1. Na swoim pulpicie Miro kliknij przycisk **+ Utwórz nowy**.
2. Z menu rozwijanego wybierz **Importuj**, a następnie wybierz **Importuj z Muralu**.
   Pojawi się okno **Importuj tablice z Muralu**.
3. Postępuj zgodnie z instrukcjami wyświetlanymi w oknie modalnym. Zostaniesz poproszony o przesłanie plików PDF z Mural.
   Możesz opcjonalnie wybrać dodanie zaimportowanej zawartości do danej przestrzeni w Miro. Jeśli nie określisz przestrzeni, importowana zawartość zostanie dodana do głównego obszaru zespołu.
4. Po przesłaniu plików i skonfigurowaniu opcji wybierz **Importuj tablice**.
   Proces importu rozpocznie się. Otrzymasz powiadomienie e-mail od Miro, gdy import zostanie ukończony.

Gratulacje! Udało Ci się zaimportować zawartość z Mural do Miro za pomocą PDF.

## Oczekiwane wyniki

Podczas importowania obiektów z Mural do Miro przez PDF, można spodziewać się pewnych różnic w stylizacji i formatowaniu ze względu na różnice między platformami oraz naturę konwersji do PDF. Ta sekcja opisuje typowe wyniki importu dla powszechnych obiektów z Mural oraz oferuje kilka najlepszych praktyk.

### Obszary

Zewnętrzny obszar w eksporcie Mural zazwyczaj jest importowany jako ramka Miro. Inne, wewnętrzne obszary są zwykle importowane jako zwykłe kształty w Miro.

:::note
**Uwaga:** Zagnieżdżone obszary (obszary w obrębie obszarów) mogą czasami być błędnie zidentyfikowane lub zbudowane podczas importu. Importer PDF opiera się na wizualnych współrzędnych do określania relacji element nadrzędny-element podrzędny widżetów, co może być niejasne przy skomplikowanym zagnieżdżaniu.
:::

### Łączniki

Importowanie PDF głównie rozpoznaje i odtwarza łączniki z solidnymi liniami. Łączniki z kropkowanymi lub przerywanymi liniami mogą nie zostać poprawnie zaimportowane.

Jeśli łącznik w Mural zawiera tekst osadzony bezpośrednio na linii, importer PDF może zinterpretować to jako dwie oddzielne linie z obiektem tekstowym w pobliżu, zamiast jako pojedynczy łącznik z tekstem.

![A connector with text that the PDF importer breaks into two lines.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Łącznik z tekstem, który importer PDF „rozbija” na dwie linie.*

### Rysunki

Elementy rysowane ręcznie z Mural są zazwyczaj importowane jako zestaw linii lub krzywych w Miro.

W przypadku skomplikowanych rysunków, importer PDF może czasami błędnie powiązać części rysunku z nakładającymi się lub pobliskimi obiektami, interpretując je jako konektory, gdy nie było takiego zamierzenia.

![A drawing may import as linked to a nearby or overlapping object.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Rysunek może zostać zaimportowany jako powiązany z pobliskim lub nakładającym się obiektem.*

### GIF-y

Importer PDF rozpoznaje GIF-y z Mural, ale zaimportuje je jako statyczne obrazy (zwykle pierwsza klatka GIF-a).

:::note
**Uwaga:** Sam format pliku PDF nie obsługuje animowanych GIF-ów. To jest ograniczenie PDF, a nie importera Miro.
:::

### Obrazy

Obrazy z Twojej tablicy Mural zostaną zaimportowane jako obrazy w Miro. Jednak ich dokładna pozycja na tablicy może nieznacznie się zmienić z powodu różnic w systemach współrzędnych między Mural a Miro oraz procesem konwersji do PDF.

### Listy

Listy (zarówno numerowane, jak i wypunktowane) z Mural zazwyczaj są importowane jako listy w Miro. Aby uzyskać najlepsze rezultaty, upewnij się, że Twoje listy w Mural używają domyślnych znaczników (standardowych numerów dla list uporządkowanych oraz podstawowych punktorów dla list nieuporządkowanych).

![A numbered list, and a bulleted list, with default markers, numerals and bullets respectively.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Numeryczna lista i wypunktowana lista z domyślnymi znacznikami, numerami i punktorami.*

### Mapy myśli

Metoda importu przez PDF najlepiej działa dla map myśli w Muralu, które mają pojedynczy węzeł główny i widoczne ramki na wszystkich węzłach. Złożone mapy myśli z wieloma węzłami głównymi lub ukrytymi ramkami mogą nie zostać prawidłowo zaimportowane.

![A basic Mind map is easier to import as PDF.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Podstawowa mapa myśli jest łatwiejsza do importu jako PDF*

Importer PDF może mieć trudności z dokładnym przetworzeniem map myśli, ponieważ często zawierają one wiele linii i obiektów umieszczonych blisko siebie. Jeśli Twoja mapa myśli w formacie PDF została źle zaimportowana, rozważ skopiowanie i wklejenie zawartości mapy myśli bezpośrednio z Mural do Miro. Chociaż metoda kopiuj-wklej może wymagać ręcznych dostosowań stylu i skali w Miro, ogólna zgodność strukturalna może być wyższa dla niektórych map myśli.

### Kształty

Importer PDF został zaprojektowany do importowania podstawowych kształtów z Mural (np. prostokąty, owale, trójkąty) jako edytowalne kształty w Miro.

![Only basic shapes import as editable content.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Tylko podstawowe kształty importują się jako edytowalne treści*

Bardziej zaawansowane, niestandardowe lub silnie wystylizowane kształty z Mural, jak również obrócone kształty, mogą być importowane jako statyczne obrazy, a nie edytowalne kształty Miro.

### Karteczki

Standardowe karteczki Mural zazwyczaj importują się jako karteczki Miro. Dla największej zgodności używaj karteczek Mural z domyślnymi proporcjami (np. popularne rozmiary 3x3 lub 5x3).

![Sticky notes with the default size can be easily imported.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Karteczki z domyślnym rozmiarem można łatwo importować*

:::note
**Uwaga:** Okrągłe karteczki z Mural będą importowane jako zwykłe kształty w Miro, ponieważ w Miro nie ma natywnego okrągłego obiektu typu karteczka.
:::

Nakładające się lub obrócone karteczki mogą nie importować się z wysoką wiernością i mogą wymagać ręcznego przesunięcia lub dostosowania w Miro.

![Import results vary for rotated sticky notes, and sticky notes that overlap.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Wyniki importu różnią się dla obróconych karteczek i karteczek, które się nakładają.*

### Tabele

Proste tabele z Mural z wyraźnymi liniami siatki zazwyczaj importują się z wysoką wiernością jako tabele Miro lub zbiór kształtów i linii tworzących strukturę tabeli.

Tabele o złożonej geometrii mogą być zaimportowane jako seria niepołączonych linii i pól tekstowych. Aby uzyskać najlepsze wyniki przy imporcie tabel, upewnij się, że tabele w twoim eksporcie z Mural **nie** mają następujących cech:

- Złączone komórki
- Niewidoczne lub ukryte granice
- Zaokrąglone rogi komórek lub obramowania tabeli

![Complex tables do not import with high fidelity.](../../../../../../../docs/getting-started/migrating-content-to-miro/import-mural-boards-to-miro/images/22923959796242_image.png)

*Złożone tabele nie są importowane z wysoką dokładnością.*

### Tekst

Obiekty tekstowe z Muralu są zazwyczaj importowane jako edytowalny tekst w Miro, często w pojedynczym bloku tekstowym lub kształcie odpowiadającym oryginalnemu polu tekstowemu Muralu.

Aby uzyskać jak najwyższą wierność importu tekstu, używaj domyślnych czcionek i standardowych marginesów w Muralu.

:::note
**Uwaga:** Rozmiar czcionki może się różnić po imporcie i może być konieczne ręczne dostosowanie go w Miro.
:::

Importowane PDF-y mogą rozdzielać tekst, który używa niestandardowych czcionek lub ma złożone formatowanie (np. wiele stylów w jednym polu tekstowym), na kilka mniejszych bloków tekstu.
