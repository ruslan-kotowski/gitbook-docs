---
title: "Po\u0142\u0105cz narz\u0119dzia z Zapier"
article_id: 30124629305106
translation_id: 30124629305106
locale: pl-pl
sidebar_position: 2
created_at: '2025-10-10T11:48:03Z'
updated_at: '2025-10-14T12:37:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Połącz Miro Insights z setkami narzędzi przez [Zapier](http://zapier.com/), aby automatycznie przechwytywać opinie i dane z źródeł, które nie mają bezpośrednich integracji. Umożliwia to centralizację obserwacji klientów z całego Twojego stosu technologicznego.

Integracja z Zapier pozwala na:

- Automatyczne tworzenie opinii z biletów wsparcia klienta, ankiet lub rozmów czatowych.
- Przechwytywanie danych z każdego narzędzia obsługiwanego przez Zapier, nawet jeśli Miro Insights nie ma bezpośredniej integracji.
- Zmniejszenie ręcznego wprowadzania danych poprzez skonfigurowanie zautomatyzowanych przepływów pracy.

## Tworzenie opinii

Zapier oferuje dwie główne akcje do tworzenia elementów opinii w Miro Insights.

### Tworzenie opinii

Standardowa akcja do tworzenia ogólnych elementów opinii w Miro Insights z następującymi polami:

- **Tytuł opinii**: Krótkie podsumowanie opinii.
- **Treść**: Szczegółowa zawartość lub opis opinii.
- **Nazwa zgłaszającego**: Imię i nazwisko osoby zgłaszającej opinię.
- **E-mail zgłaszającego**: Adres e-mail osoby zgłaszającej opinię.
- **E-mail właściciela**: Wewnętrzny właściciel lub przypisany do opinii.
- **Podana data i godzina**: Kiedy opinia została pierwotnie przesłana.
- **URL źródła**: Link do oryginalnego źródła (zgłoszenie, odpowiedź na ankietę itp.).
- **Nazwa firmy**: Organizacja, z którą związana jest opinia.
- **Domena firmy**: Domena strony internetowej firmy.

### Tworzenie opinii (Rozmowa)

Specjalne działanie przeznaczone do zbierania opinii z rozmów telefonicznych i konwersacji przy użyciu następujących pól:

- **Tytuł rozmowy**: Tytuł lub temat rozmowy.
- **Transkrypcja rozmowy**: Pełna transkrypcja lub notatki z rozmowy.
- **Źródłowy URL**: Link do nagrania rozmowy lub szczegółów spotkania.
- **Uczestnicy**: Informacje o uczestnikach rozmowy.
  - **E-mail**: Adres e-mail uczestnika.
  - **Nazwa**: Imię uczestnika.
- **Adres e-mail właściciela**: Wewnętrzny właściciel lub osoba odpowiedzialna za opinię z rozmowy.
- **Data i godzina rozpoczęcia**: Kiedy odbyła się rozmowa.
- **Nazwa firmy**: Organizacja związana z rozmową.
- **Domena firmy**: Domena strony internetowej firmy.

## Konfigurowanie integracji z ZAPIER

Aby rozpocząć pracę z ZAPIER i Miro Insights, wykonaj te kroki.

### Wymagania wstępne

- Aktywne konto Miro Insights
- Konto ZAPIER (Free lub płatne)
- Dostęp do narzędzia źródłowego, które chcesz połączyć

### Szybki start od szablonów

Miro Insights oferuje wstępnie przygotowane szablony Zapier dla popularnych narzędzi do analizy rozmów, takich jak Grain, Fathom i Fireflies.

Aby skonfigurować Zapa za pomocą szablonu:

1. Przejdź do ustawień Miro Insights > sekcja **Integracje & Automatyzacje**.
2. Wybierz swoje narzędzie do analizy rozmów. Na przykład Grain.
3. Zaloguj się do Zapier, jeśli konieczne.
4. Podłącz swoje konto Grain.
5. Przeprowadź mapowanie pól z Grain do pól Miro Insights.
6. Przetestuj i aktywuj wstępnie skonfigurowaną integrację.

Szablony zapewniają szybszą konfigurację dzięki optymalnym odpowiednikom pola dla każdego konkretnego narzędzia, co ułatwia rozpoczęcie zbierania feedbacku od klientów z nagranych rozmów.

### Konfiguracja podstawowa

1. **Utwórz nowy Zap** w swoim pulpicie Zapier.
2. Wybierz swoją **aplikację wyzwalającą**. Narzędzie, z którego pochodzi feedback.
3. Wybierz **Miro Insights** jako swoją aplikację akcji.
4. Wybierz swoje **zdarzenie akcji**:
   - **"Stwórz Opinię"** dla ogólnych elementów feedbacku.
   - **"Stwórz Opinię (Rozmowa)"** dla feedbacku specyficznego dla rozmowy.
5. Połącz swoje **konto Miro Insights** gdy pojawi się monit.
6. **Mapuj pola** z aplikacji wyzwalającej do pól Miro Insights.
7. Przetestuj integrację, aby upewnić się, że dane przepływają poprawnie.
8. **Aktywuj Zap** aby rozpocząć automatyczne zbieranie danych.

### Najlepsze praktyki mapowania pól

Podczas mapowania pól z Twojego narzędzia źródłowego do Miro Insights, weź pod uwagę następujące najlepsze praktyki, aby zapewnić wysoką jakość przechwytywania danych.

**Wymagane pola:**

- **Tytuł feedbacku**: Użyj jasnych, opisowych tytułów z danych źródłowych.
- **Treść**: Zamapuj główną treść feedbacku lub połącz kilka pól.

**Zalecane pola:**

- **Informacje o zgłaszającym**: Zbierz dane kontaktowe klienta, jeśli są dostępne.
- **Dane firmy**: Niezbędne do zarządzania produktem w oparciu o konto.
- **Źródłowy URL**: Zachowaj śledzenie do oryginalnych źródeł.
- **Podana data**: Użyj rzeczywistej daty opinii, a nie daty przetwarzania.

**Wskazówki dotyczące mapowania pól:**

- Użyj narzędzi formatujących Zapier, aby połączyć wiele pól źródłowych.
- Dla przejrzystości dołącz nazwę narzędzia źródłowego w tytule lub treści.
- Stosuj spójne formaty dla dat, nazw firm i kategorii.
- Ustaw domyślne wartości dla opcjonalnych pól.
