---
title: Importuj tablice Lucidspark do Miro
article_id: 9549014537490
translation_id: 9549014537490
locale: pl-pl
sidebar_position: 7
created_at: '2023-01-12T09:05:07Z'
updated_at: '2026-01-19T14:30:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: backup-restore-board
availability:
  notes: 'Osoby: Każdy użytkownik z uprawnieniami do edycji zarówno tablic Lucidspark,
    jak i Miro Plany: Free, Starter, Business, Education i Enterprise Platformy: Przeglądarka,
    Desktop'
---

Migruj swoje treści z Lucidspark do Miro, aby wzmocnić doświadczenie współpracy. Ten przewodnik wyjaśnia, jak zaimportować swoje tablice i czego się spodziewać w trakcie tego procesu.

> **Ostrzeżenie:** Edytowanie zaimportowanej treści jest jednokierunkowe. Zmiany wprowadzone w Miro nie będą synchronizowane z Lucidspark.

> **Uwaga:** Tablice Lucidspark z planami Free lub Restricted można migrować.

## Jak zaimportować tablice Lucidspark za pomocą eksportu do PDF

Postępuj zgodnie z poniższymi krokami, aby zaimportować tablice Lucidspark do Miro metodą eksportu PDF:

1. Upewnij się, że eksportujesz treści **Lucidspark**, które chcesz zaimportować do Miro jako PDF.
2. Na pulpicie **Home** w Miro kliknij **+ Utwórz nowy**.
3. Wybierz **Importuj**, a następnie **Importuj z Lucidspark**.
   Otworzy się **okno modalne Importuj z Lucidspark**. Możesz zbiorczo zaimportować kilka plików PDF Lucidspark.
4. Postępuj zgodnie z instrukcjami wyświetlanymi na ekranie w oknie modalnym.
5. Wybierz **Importuj tablice**.
6. Przejrzyj zaimportowaną zawartość i wprowadź niezbędne poprawki. Mimo że Lucidspark i Miro mają podobne funkcje, mogą występować różnice w opcjach stylizacji i formatowania. Zapoznaj się z [Jak obiekty Lucidspark są odwzorowywane w Miro (Metoda zbiorczego importu PDF)](#lucidspark-object-mapping-bulk-import), aby uzyskać wskazówki dotyczące tego, jak obiekty są tłumaczone.

## Metoda alternatywna: Kopiowanie i wklejanie zawartości

Jako szybszą alternatywę do przenoszenia mniejszych ilości zawartości, możesz bezpośrednio kopiować elementy z otwartej tablicy Lucidspark i wklejać je na tablicę Miro.

> **Uwaga:** Każdy użytkownik z uprawnieniami do edycji zarówno tablic Lucidspark, jak i Miro, powinien być w stanie kopiować treści z Lucidspark i wklejać je do Miro. Aby uzyskać szczegóły dotyczące tego, jak obiekty są tłumaczone przy użyciu tej metody, zobacz [Jak obiekty Lucidspark pojawiają się w Miro (Metoda kopiuj/wklej)](#lucidspark-object-mapping-copy-paste).

## Jak obiekty Lucidspark pojawiają się w Miro (Metoda kopiuj/wklej)

Ta tabela zapewnia kompleksowe porównanie, jak obiekty są tłumaczone, gdy kopiujesz treści bezpośrednio z Lucidspark i wklejasz je do Miro.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Karty Azure | Karty Azure są migrowane jako Karty Miro: 1. Skonfiguruj integrację Azure w Miro. 2. Przekształć Karty Miro na [Karty Azure](../../integrations-apps/microsoft/03-azure-cards.md). |
| Współpracownicy i udostępnianie | 🟠 Można odtworzyć ręcznie |
| Komentarze | 🟠 Można odtworzyć ręcznie |
| Łączniki i rozdzielniki | Łączniki |
| Kontenery | Kształty |
| Dokumenty z plików i adresów URL | 🟠 Mogą być odtworzone ręcznie |
| Dokumenty URL (PDF) | Osadzone dokumenty |
| Rysunki | Obrazy |
| Dynamiczne tabele | Tabele |
| Emoji | Obrazy |
| Ramki | Ramki |
| GIF-y z paska narzędzi | Obrazy |
| GIF-y z plików | Obrazy |
| GIF-y z URL | GIF-y |
| Obrazy | Obrazy |
| Karty Jira | Karty Jira migrują się jako Karty Miro:  1. Skonfiguruj integrację z Jira w Miro 2. Przekonwertuj Karty Miro na [Karty Jira](../../integrations-apps/atlassian/03-jira-cards.md). |
| Karty Lucid | Karty |
| Mapa myśli | Mapa myśli |
| Kształty | Kształty |
| Karteczka | Karteczki |
| Tabele | Tabele |
| Tekst | Tekst |
| Oś czasu | 🟠 Można odtworzyć ręcznie |
| Wideo i inne adresy URL | Podglądy |

## Jak obiekty Lucidspark pojawiają się w Miro (Zbiorcza metoda importu PDF)

Ta tabela przedstawia szczegółowe porównanie obiektów pomiędzy Lucidspark i Miro po zbiorczym imporcie treści przez PDF.

|  |  |
| --- | --- |
| **Lucidspark** | **Miro** |
| Karty Azure | Obrazy |
| Współpracownicy i udostępnianie | 🟠 Można odtworzyć ręcznie |
| Komentarze | 🟠 Można odtworzyć ręcznie |
| Łączniki i podziałki | Łączniki |
| Kontenery | Kształty |
| Dokumenty | 🟠 Można odtworzyć ręcznie |
| Rysuj | Linie |
| Tabele dynamiczne | Kształty i łączniki |
| Emoji | Obrazy |
| Ramki | Ramki i kształty |
| GIF-y | Obrazy |
| Obrazy | Obrazy |
| Karty Jira | Kształty |
| Karty Lucid | Kształty |
| Mapa myśli | Kształty i łączniki |
| Kształty | Kształty |
| Karteczka | Karteczki |
| Tabele | Tabele/Kształty i łączniki |
| Tekst | Tekst |
| Oś czasu | Kształty i łączniki |
| Wideo i inne adresy URL | 🟠 Można odtworzyć ręcznie |

## Ograniczenia importu

Chociaż Lucidspark i Miro oferują podobne funkcjonalności, bądź świadomy następujących różnic i ograniczeń przy imporcie zawartości:

- Pola tekstowe Miro mogą pomieścić do 6000 znaków, wliczając spacje. Dodatkowy tekst zostanie przycięty.
- Kolory i style są dopasowywane do najbliższych odpowiedników w Miro.
- Wartości przezroczystości z Lucidspark nie są dokładnie odwzorowywane podczas importu.
- Karteczki Miro nie obsługują obrotu, dostosowywania palety kolorów ani wypunktowania tekstu, które mogły być użyte w Lucidspark.

## Uzyskiwanie pomocy

> **Uwaga:** W razie dalszych pytań i potrzeby wsparcia dotyczącego migracji z Lucidspark skontaktuj się z [zespołem wsparcia Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md) lub bezpośrednio z Twoim managerem ds. sukcesu klienta w Miro.
