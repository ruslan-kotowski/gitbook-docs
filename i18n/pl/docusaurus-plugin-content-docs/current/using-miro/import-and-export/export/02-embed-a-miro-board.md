---
title: Osadzenie tablicy Miro
article_id: 360016335640
translation_id: 360016335640
locale: pl-pl
sidebar_position: 2
created_at: '2020-09-09T07:54:13Z'
updated_at: '2025-09-19T09:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Lista osób: edytujący tablic Abonamenty: wszystkie abonamenty Platformy:
    internetowa, komputerowa, mobilna'
---

Możesz osadzić dowolną tablicę Miro lub konkretny element (ramkę lub format) z tablicy w obsługiwanych aplikacjach i witrynach, aby Twoi współpracownicy mogli pracować w kontekście bez zmieniania narzędzi.

Osadzone elementy dziedziczą [ustawienia udostępniania](../../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) tablicy:

- **Publiczny link włączony** — każdy z linkiem może wyświetlać (lub, w płatnych i Education, komentować lub edytować).
- **Publiczny link wyłączony** — tylko zaproszeni współpracownicy mogą otworzyć osadzenie po zalogowaniu się.

[Administratorzy Enterprise](../../../plans-billing/miro-plans/04-enterprise-plan.md) mogą zarządzać dostępnością publicznego linku w [ustawieniach bezpieczeństwa](../../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Wybierz metodę osadzania

Miro oferuje dwie metody osadzania tablic:

- **Korzystając z obsługiwanych aplikacji**:

  - Praca na platformach takich jak Zoom, Teams, Confluence, Jira czy Notion.
  - Chęć korzystania z funkcji natywnej integracji i bezproblemowego przepływu pracy.
  - Użytkownicy będą głównie korzystać z tej konkretnej platformy.
  - Potrzebujesz najprostszego procesu konfiguracji.
- **Za pomocą kodu do osadzenia**:

  - Osadzenie w witrynach internetowych, blogach lub platformach niestandardowych.
  - Praca z WordPress, Webflow lub innymi kreatorami stron internetowych.
  - Potrzebujesz większej kontroli nad rozmiarem i wyglądem.
  - Platforma obsługuje iFrames, ale nie ma natywnej integracji z Miro.

## Osadź tablicę w obsługiwanych aplikacjach

Miro oferuje szereg aplikacji obsługiwanych, w których możesz łatwo udostępniać swoje tablice Miro. Do obsługiwanych aplikacji należą:

- [Zoom](../../../integrations-apps/zoom/02-miro-app-for-zoom-user-guide.md)
- [Webex](../../../integrations-apps/more-integrations/10-miro-for-webex.md)
- [Microsoft Teams](../../../integrations-apps/microsoft/microsoft-teams/02-miro-for-microsoft-teams-user-guide.md)
- [Jira](../../../integrations-apps/atlassian/02-miro-for-jira-cloud.md)
- [Confluence](../../../integrations-apps/atlassian/01-miro-for-confluence.md)
- [Notion](https://miro.com/marketplace/notion-embed/)
- [Coda](https://miro.com/marketplace/coda-embed/)
- [Productboard](https://miro.com/marketplace/productboard-embed/)
- Medium

Kiedy osadzasz tablicę Miro w innej aplikacji, możesz ustawiać prawa dostępu specyficzne dla użytkowników tej aplikacji, umożliwiając im wyświetlanie, komentowanie lub edytowanie tablicy bezpośrednio z poziomu aplikacji. Dostęp do tablicy po stronie Miro nie zostanie zmieniony. Dowiedz się, jak działają [udostępnianie i uprawnienia dla osadzonych tablic](../../../integrations-apps/integrate-miro-with-other-apps/01-user-permissions-for-boards-embedded-in-third-party-apps.md).

Aby osadzić tablicę w jednej z obsługiwanych aplikacji:

1. W docelowej aplikacji wpisz **/miro** lub wybierz **Miro** z menu wstawiania.
2. Wybierz tablicę.
3. Wybierz **początkowe wyświetlanie**:
   - **Cała tablica** — cała plansza.
   - **Specyficzny element**, taki jak ramka lub format (Dokument, Diagram, Tabela, Oś czasu lub Slajdy).
4. Włącz **tryb skupienia**, aby stworzyć osadzenie bez rozpraszaczy. Pozostaw wyłączony, aby umożliwić pełną interakcję.
5. Wybierz **ustawienia dostępu** dla wszystkich odwiedzających:
   - **Może wyświetlać** — każdy odwiedzający osadzoną zawartość może wyświetlać tablicę.
   - **Wymagany dostęp** — każdy odwiedzający osadzoną zawartość musi mieć dostęp do wyświetlania, komentowania lub edytowania tablicy.
6. Wybierz **Osadź tablicę**.

Osadzenie respektuje ustawienia udostępniania tablicy. Na urządzeniach mobilnych wszystkie osadzenia są tylko do odczytu.

## Osadź tablicę za pomocą kodu osadzania

Użyj tej opcji dla każdej platformy, która obsługuje iFrame, such as **WordPress** lub **Webflow**.

1. Otwórz panel **Udostępnij** używając jednej z tych metod:
   - W prawym górnym rogu wybierz **Udostępnij** > **Osadź**, lub
   - W głównym menu tablicy wybierz **Tablica** > **Eksportuj** > **Osadź**, lub
   - Na planszy wybierz element, który chcesz osadzić (ramka lub format). Na przykład, dokument. Otwórz menu kontekstowe z trzema kropkami i wybierz **Osadź ten dokument**.
2. Wybierz **Początkowe wyświetlanie**:
   - **Tablica** — cała plansza.
   - **Specyficzny element**, taki jak ramka lub format (dokument, diagram, tabela, oś czasu lub slajdy).
3. (Opcjonalnie) **Ustaw obszar początkowy** — przeciągnij, aby zaznaczyć dokładny obszar tablicy.
4. Zdecyduj o interakcji:
   - Zaznacz **Tylko wyświetlanie**, aby zablokować widok.
   - Odznacz **Tylko wyświetlanie**, aby umożliwić wyświetlającym przesuwanie, powiększanie, komentowanie lub edytowanie (jeśli mają uprawnienia).
5. Wybierz **Kopiuj kod** i wklej go tam, gdzie jest potrzebny.
   Jeśli docelowe miejsce obsługuje tylko adresy URL, wybierz zamiast tego **Kopiuj link**.

Możesz utworzyć wiele osadzeń dla tej samej tablicy, każde z własnym początkowym widokiem, obszarem początkowym lub obiektem do skupienia.

### Autoodtwarzanie slajdów

Aby autoodtwarzać osadzony Slajd, ustaw **Interwał autoodtwarzania slajdów** od 1 do 30 sekund w zakładce **Osadzenie**. Autoodtwarzanie jest ignorowane, gdy osadzasz tablicę w innej tablicy.

## Jak wyglądają osadzenia

- Nazwa tablicy nie jest klikalna.
- Mapa, [notatki](../../essential-tools/17-visual-notes.md) i popupy są domyślnie zamknięte.
- Niektóre opcje menu, takie jak **Ustaw widok początkowy**, są ukryte.
- Wszystkie osadzenia są tylko do odczytu na urządzeniach mobilnych.
- Blokery ciasteczek stron trzecich mogą uniemożliwić prawidłowe ładowanie osadzeń.

## Często zadawane pytania

**Jaka jest różnica między widokiem początkowym a trybem skupienia?**
Widok początkowy ustawia pozycję startową, ale wyświetlający mogą nadal eksplorować tablicę. Tryb skupienia ukrywa wszystko poza wybranym obiektem i zawsze jest w trybie tylko do odczytu.

**Czy mogę zrobić, aby osadzenie w trybie skupienia było edytowalne?**
Nie. Aby umożliwić współpracę, usuń zaznaczenie **Tylko do odczytu** i przyznaj prawa do edycji w ustawieniach udostępnienia tablicy.

**Jakie widgety są obsługiwane?**
Dokumenty, Diagramy, Tabele, Oś czasu, Slajdy i dowolna ramka.

**Czy mogę usunąć logo Miro?**
Nie. Usunięcie znaków firmowych nie jest dostępne.

**Czy mogę osadzić tablicę w innej tablicy?**
Tak. Skopiuj kod osadzenia i wklej go do docelowej tablicy za pomocą **Wklej kod iFrame**.
