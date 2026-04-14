---
title: "Importuj etykiety poufno\u015Bci Microsoft Purview"
article_id: 22161930709010
translation_id: 22161930709010
locale: pl-pl
sidebar_position: 7
created_at: '2024-10-23T15:05:49Z'
updated_at: '2025-12-01T16:32:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Dla organizacji korzystających z Microsoft Purview, utrzymanie spójnego bezpieczeństwa danych i klasyfikacji na wielu platformach jest kluczowe. Integracja Miro z Microsoft Purview umożliwia administratorom importowanie etykiet poufności bezpośrednio z Microsoft Purview do Miro, upraszczając zarządzanie schematami klasyfikacji na obu platformach.

Dzięki wykorzystaniu tej integracji, organizacje mogą zapewnić, że treść w Miro jest klasyfikowana zgodnie z ustaloną strukturą Microsoft Purview. To nie tylko redukuje obciążenie operacyjne związane z manualnym odtwarzaniem lub aktualizacją etykiet klasyfikacji, ale także wzmacnia bezpieczeństwo danych. Poprzez dostosowanie możliwości ochrony danych Miro do Microsoft Purview, administratorzy mogą z pewnością zarządzać informacjami wrażliwymi w całym swoim cyfrowym ekosystemie.

## Importowanie etykiet poufności Microsoft Purview do Miro

Jeśli w Twojej organizacji nie skonfigurowano jeszcze klasyfikacji danych w Miro, możesz łatwo założyć klasyfikację danych w Miro, importując istniejące etykiety poufności bezpośrednio z Microsoft Purview.

Jeśli masz już istniejącą konfigurację klasyfikacji danych, możesz zaimportować etykiety poufności z Microsoft Purview oraz przenieść istniejące etykiety klasyfikacji w Miro.

## Konfiguracja klasyfikacji danych przez importowanie etykiet poufności z Microsoft Purview

### Wymagania wstępne

- Upewnij się, że masz niezbędne role lub uprawnienia do pracy z etykietami poufności w Microsoft Purview.
- Musisz znać szczegóły poziomów klasyfikacji tablic, które chcesz skonfigurować zgodnie z wymaganiami dotyczącymi bezpieczeństwa i zarządzania.
- Musisz mieć [rolę administratora treści wrażliwych](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby złożyć prośbę o rolę administratora treści wrażliwych, skontaktuj się z administratorem firmy.

:::note
Notatki:
- Zgodnie z dokumentacją Microsoftu, aktualizacje etykiet poufności w Microsoft Purview mogą zająć do 24 godzin, zanim zostaną zreplikowane we wszystkich aplikacjach i usługach. Prosimy o odczekanie odpowiedniego czasu na wprowadzenie zmian, a następnie zaimportowanie etykiet poufności. Jeśli aktualizacje wprowadzone w Microsoft Purview nie zostaną zreplikowane po 24 godzinach, prosimy o kontakt z zespołem wsparcia Microsoft Purview.
- Możesz zaimportować maksymalnie 50 etykiet poufności z Microsoft Purview do Miro.
- Jeśli masz już istniejącą konfigurację klasyfikacji danych, możesz zaimportować etykiety poufności z Microsoft Purview i przenieść istniejące etykiety klasyfikacyjne w Miro. Aby uzyskać więcej informacji, zobacz [Importuj etykiety poufności z Microsoft Purview do istniejącej konfiguracji klasyfikacji danych w Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Aby zaimportować etykiety poufności z Microsoft Purview i skonfigurować klasyfikację danych w Miro, wykonaj następujące kroki:

1. Przejdź do [ustawień Miro](https://miro.com/app/settings).
2. W lewym panelu, w sekcji **Enterprise Guard**, kliknij **Klasyfikacja danych**.
3. Na stronie **Klasyfikacja**, na dole ekranu, kliknij **Rozpocznij**.
4. W oknie **Import z Microsoft Purview**, kliknij **Zaloguj się**.
5. Na stronie **Logowanie do Microsoft**, która otwiera się w nowej karcie, wprowadź swoje dane dostępowe Microsoft i zaloguj się. Po zalogowaniu się na swoje konto Microsoft, karta zamyka się automatycznie.
6. Na stronie **Klasyfikacja**, w polu **Importuj z Microsoft Purview**, kliknij **Importuj**.
   Pojawi się strona **Importuj klasyfikację z Microsoft Purview**.
7. Zaznacz pole wyboru dla etykiet poufności Microsoft Purview, które chcesz użyć jako poziomy klasyfikacji w Miro, a następnie kliknij **Dalej**.

   > ✏️ Zgodnie z dokumentacją Microsoftu, aktualizacje etykiet poufności w Microsoft Purview mogą zająć do 24 godzin, aby zostać zreplikowane we wszystkich aplikacjach i usługach. Pozwól na odpowiedni czas na wprowadzenie zmian, a następnie zaimportuj etykiety poufności. Jeśli aktualizacje wprowadzone w MS Purview nie zostały zreplikowane po upływie 24 godzin, skontaktuj się z zespołem pomocy Microsoft Purview.
8. Na stronie **Zdefiniuj poziomy klasyfikacji** możesz edytować poziomy klasyfikacji, aby przypisać domyślny poziom klasyfikacji lub dodać link do wytycznych. Poniższa tabela wymienia każde pole i jego opis.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | **Link do wytycznych** | URL, który zapewnia więcej informacji na temat zasad lub instrukcji odnoszących się do tego poziomu klasyfikacji. Może to być strona, która dostarcza więcej informacji dla użytkowników w twojej organizacji, aby dowiedzieć się więcej o poziomach klasyfikacji tablic i jak z nimi pracować. Musisz podać URL w następującym formacie: `http://www.example.com`  Kiedy użytkownik klika ikonę **Dowiedz się więcej** (ikona z pytajnikiem) obok odznaki klasyfikacji tablicy, ten URL jest ładowany w nowej karcie przeglądarki. |
   | **Ustaw jako domyślny poziom dla nowych tablic** | Zaznacz to pole wyboru, aby ustawić ten poziom klasyfikacji jako domyślny dla wszystkich nowych tablic. |
   | **Podgląd** | Wyświetla podgląd odznaki klasyfikacji tablicy z jej opisem i ikonką „dowiedz się więcej”. Podgląd pokazuje dokładnie, jak odznaka klasyfikacyjna pojawia się dla użytkowników na tablicy. |
9. Aby zapisać konfigurację poziomu klasyfikacji, kliknij **Zrobione**.
10. Kliknij **Dalej**. Twoja konfiguracja jest zapisana, ale zacznie obowiązywać dopiero po kliknięciu **Publikuj** na stronie [**Sprawdź wpływ**](https://help.miro.com/hc/articles/16494764223378).

    Możesz teraz kontynuować z jednym z następujących kroków:

    - [Zdefiniuj automatyczną klasyfikację](09-define-auto-classification.md). To jest opcjonalne. Jeśli chcesz zdefiniować automatyczną klasyfikację później, kliknij **Dalej**.
    - [Zdefiniuj zabezpieczenia](05-define-guardrails.md). To jest opcjonalne. Jeśli chcesz zdefiniować zabezpieczenia później, kliknij **Dalej**.
    - [Przejrzyj wpływ](https://help.miro.com/hc/articles/16494764223378). To jest ostatni krok w przepływie pracy i jest obowiązkowy.

## Import etykiet poufności z Microsoft Purview do istniejącej konfiguracji klasyfikacji danych w Miro

### **Wymagania wstępne**

- Upewnij się, że masz niezbędne role lub uprawnienia do pracy z etykietami poufności w Microsoft Purview.
- Musisz znać szczegóły poziomów klasyfikacji tablic, które chcesz skonfigurować na podstawie swoich wymagań dotyczących bezpieczeństwa i zarządzania.
- Musisz mieć [rolę administratora treści wrażliwych](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby zażądać roli administratora treści wrażliwych, skontaktuj się z administratorem firmy.

:::note
Notatki:
- Zgodnie z dokumentacją Microsoft, aktualizacje etykiet poufności w Microsoft Purview mogą zająć do 24 godzin, aby zostać zreplikowane do wszystkich aplikacji i usług. Prosimy o umożliwienie wystarczającej ilości czasu na wprowadzenie zmian, a następnie importowanie etykiet poufności. Jeśli aktualizacje dokonane w MS Purview nie zostaną zreplikowane po 24 godzinach, skontaktuj się z zespołem pomocy Microsoft Purview.
- Możesz importować do 50 etykiet poufności z Microsoft Purview do Miro.
- Nie możesz przenieść poziomów klasyfikacji, które są używane w zasadach retencji. Musisz upewnić się, że poziomy klasyfikacji nie są używane w żadnych zasadach retencji przed kontynuacją. Więcej informacji znajdziesz w [edycja zasady retencji](../content-lifecycle-management/11-edit-retention-policy.md).
:::

Aby zaimportować etykiety poufności z Microsoft Purview i przyporządkować/przenieść do istniejących etykiet klasyfikacji w Miro, wykonaj następujące kroki:

1. Przejdź do [ustawień Miro](https://miro.com/app/settings).
2. W lewym panelu, w sekcji **Enterprise Guard**, kliknij **Klasyfikacja danych**.
3. Na stronie **Klasyfikacja** na górze ekranu kliknij **Importuj**.
4. Jeśli jesteś już zalogowany do Microsoft, pomiń ten krok i przejdź do następnego kroku.
   Jeśli nie jesteś zalogowany do Microsoft, kliknij **Zaloguj się**. Na stronie **Logowanie do Microsoft**, która pojawi się w nowej karcie, wprowadź swoje dane dostępowe Microsoft i zaloguj się. Po zalogowaniu karta zostanie automatycznie zamknięta.
5. W sekcji **Importuj z Microsoft Purview** kliknij **Importuj** obok Import etykiet poufności do Miro. Pojawi się strona **Importuj klasyfikację z Microsoft Purview**.
6. Na stronie **Importuj poziomy**, zaznacz pole wyboru dla etykiet poufności Microsoft Purview, które chcesz użyć jako poziomy klasyfikacji w Miro, a następnie kliknij **Dalej**. Pojawi się strona **Przenieś istniejące poziomy**.

   > ✏️ Według dokumentacji Microsoftu, aktualizacje etykiet poufności w Microsoft Purview mogą zająć do 24 godzin, zanim zostaną zreplikowane do wszystkich aplikacji i usług. Proszę odczekać odpowiednią ilość czasu na wprowadzenie zmian, a następnie zaimportować etykiety poufności. Jeśli po 24 godzinach aktualizacje, które wprowadziłeś w MS Purview, nie zostaną zreplikowane, skontaktuj się z zespołem pomocy Microsoft Purview.
7. Aby zapewnić prawidłową klasyfikację treści, musisz przenieść istniejące poziomy klasyfikacji Miro do nowo zaimportowanych poziomów etykiet poufności z Microsoft Purview. Poziomy wymienione po lewej stronie to istniejące poziomy klasyfikacji Miro, a te wymienione w rozwijanej liście po prawej to zaimportowane etykiety poufności z Microsoft Purview. Po zakończeniu kliknij **Dalej**.
8. Na stronie **Zdefiniuj poziomy klasyfikacji** możesz edytować poziomy klasyfikacji, aby przypisać domyślny poziom klasyfikacji lub dodać link do wytycznych. Poniższa tabela wymienia każde pole oraz jego opis.

   |  |  |
   | --- | --- |
   | **Pole** | **Opis** |
   | **Link do wytycznych** | URL, który dostarcza więcej informacji na temat zasad lub wytycznych stosowanych dla tego poziomu klasyfikacji. Może to być strona, która dostarcza więcej informacji użytkownikom w Twojej organizacji na temat poziomów klasyfikacji tablic i jak z nimi pracować. Musisz podać URL w następującym formacie: `http://www.example.com`  Kiedy użytkownik kliknie ikonę **Dowiedz się więcej** (ikona znaku zapytania) obok odznaki klasyfikacji tablicy, ten URL jest otwierany w nowej karcie przeglądarki. |
   | **Ustaw jako domyślny poziom dla nowych tablic** | Zaznacz to pole wyboru, aby ustawić ten poziom klasyfikacji jako domyślną klasyfikację dla wszystkich nowych tablic. |
   | **Podgląd** | Wyświetla podgląd odznaki klasyfikacji tablicy wraz z jej opisem i ikoną „dowiedz się więcej”. Podgląd pokazuje dokładnie, jak odznaka klasyfikacji wygląda dla użytkowników na tablicy. |

   Aby zapisać konfigurację poziomu klasyfikacji, kliknij **Gotowe**.
9. Kliknij **Dalej**. Twoja konfiguracja zostanie zapisana, jednak wejdzie w życie dopiero po kliknięciu **Opublikuj** na stronie [**Przegląd wpływu**](https://help.miro.com/hc/articles/16494764223378).

   Możesz teraz przejść do jednej z poniższych opcji:

   - [Zdefiniuj auto-klasyfikację](09-define-auto-classification.md). To jest opcjonalne. Jeśli chcesz zdefiniować auto-klasyfikację później, kliknij **Dalej**.
   - [Zdefiniuj zabezpieczenia](05-define-guardrails.md). To jest opcjonalne. Jeśli chcesz zdefiniować zabezpieczenia w późniejszym czasie, kliknij **Dalej**.
   - [Przeanalizuj wpływ](https://help.miro.com/hc/articles/16494764223378). To jest ostatni krok przepływu pracy i jest obowiązkowy.

## Odłączenie od Microsoft Purview

Po połączeniu z Purview nie można dodawać ani edytować nazw klasyfikacji, aktualizować poziomów klasyfikacji itp. Aby wykonać te czynności, musisz odłączyć się od Microsoft Purview. Nie można importować aktualizacji z Microsoft Purview do Miro po odłączeniu od Purview.

Aby odłączyć się od Microsoft Purview, wykonaj następujące kroki:

1. Przejdź do [ustawień Miro](https://miro.com/app/settings).
2. W lewym panelu, w sekcji **Enterprise Guard**, kliknij **Klasyfikacja danych**.
3. Na stronie **Klasyfikacja**, na górze ekranu, kliknij przycisk **Ostatni import**, a następnie kliknij **Odłącz od Purview**.
