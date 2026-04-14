---
title: Przenoszenie danych między regionami – Automatyczna migracja
article_id: 24866660560402
translation_id: 24866660560402
locale: pl-pl
sidebar_position: 5
created_at: '2025-02-24T08:47:08Z'
updated_at: '2025-10-29T14:40:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Kto może to zrobić: Administratorzy firmy Które plany: Enterprise Na których
    platformach: Przeglądarka, Desktop'
---

:::note
Automatyczna migracja to płatna usługa współpracy z działem usług profesjonalnych. Aby uzyskać wycenę, skontaktuj się z dedykowanym opiekunem klienta w Miro.
:::

Artykuł ten wyjaśnia automatyczną migrację danych. Aby dowiedzieć się więcej o innych opcjach przenoszenia danych między regionami, zobacz [Przenoszenie danych między regionami](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Dane uwzględnione w automatycznej migracji między regionami

Poniższa lista pokazuje, jakie dane są uwzględnione w automatycznej migracji między regionami:

- Tablice, treść tablic oraz ustawienia udostępniania tablic
- Hierarchia treści, w tym zespoły, przestrzenie i sekcje przestrzeni
- Organizacja, ustawienia zespołów i tablic
- Użytkownicy, profile użytkowników oraz ustawienia użytkowników, w tym goście
- Dzienniki audytu, klasyfikacja danych i ustawienia bezpieczeństwa treści

## Przygotowanie do migracji danych między regionami

Aby przygotować się do migracji danych między regionami, wykonaj te kroki:

1. Aby móc zarządzać wszystkimi użytkownikami w swojej domenie, zweryfikuj wszystkie domeny, które posiadasz, używając weryfikacji DNS.
2. Włącz zasadę zarządzania domeną **Blokuj własne subskrypcje**, która zapewnia, że użytkownicy nie będą przypadkowo tworzyć darmowych subskrypcji Miro w swoim starym regionie.
3. Skoordynuj zespoły i/lub organizacje w jedną organizację z jedną subskrypcją.
4. Przeprowadź audyt integracji używanych przez Twoją organizację i potrzebnych w nowym regionie, a następnie zaplanuj oś czasu na ponowną konfigurację każdej integracji w nowym regionie.

## Jak działa migracja danych między regionami i jak długo trwa

Migracja między regionami obejmuje następujące pięć kroków:

- **Przygotowanie**
  Przeważnie 4-8 tygodni. Administrator firmy, wspierany przez Miro, przygotowuje swoją organizację do migracji, planuje czas przestoju oraz komunikuje zmiany użytkownikom końcowym
- **Migracja**
  Zazwyczaj mniej niż 8 godzin przestoju. Organizacja i jej dane są migrowane do nowego regionu.

  > ✏️ Zespół Miro koordynuje się z Tobą w celu wyboru daty migracji. Jeśli migracja zakończy się niepowodzeniem z jakiegokolwiek powodu, dostęp do Twojego źródłowego regionu zostanie przywrócony, a Miro skoordynuje nową datę migracji, aby ponownie przeprowadzić proces.
- **Weryfikacja i konfiguracja**
  Typowo 2-3 tygodnie. Administrator musi ponownie skonfigurować niektóre integracje, takie jak SSO, w nowym regionie. Administrator i użytkownicy muszą zweryfikować, czy ich tablice i dane znalazły się w nowym regionie zgodnie z oczekiwaniami.
- **Szkolenie**
  Typowo 2-3 tygodnie. Użytkownicy są szkoleni w zakresie dostępu do nowej organizacji Miro.
- **Zgodność**
  W ciągu 120 dni od daty migracji – Miro weryfikuje, czy dane organizacji zostały usunięte z pierwotnego regionu.

## Co zrobić po migracji danych między regionami

Po migracji danych między regionami upewnij się, że wykonasz następujące czynności:

- Natychmiast ponownie skonfiguruj pojedyncze logowanie (SSO), jeśli dotyczy, dla nowych subdomen regionalnych. Na przykład, au.miro.com.

  > ✏️ Użytkownicy nie mogą się zalogować do nowego regionu, dopóki SSO nie zostanie ponownie skonfigurowane po stronie dostawcy tożsamości (IdP).
- Ponownie skonfiguruj SCIM dla nowych subdomen regionalnych. Na przykład, au.miro.com.
- Potwierdź, że opcja **Blokuj własne subskrypcje** w ustawieniach zarządzania domeną jest włączona.
- Sprawdź ustawienia zarządzania domeną.
- Ponownie zainstaluj i skonfiguruj odpowiednie aplikacje i integracje.

## Często zadawane pytania dotyczące automatycznych migracji danych między regionami

**Co to jest migracja danych między regionami?**

Migracje danych między regionami automatyzują przenoszenie danych klienta z jednego regionu geograficznego do innego. Końcowym rezultatem migracji między regionami jest przechowywanie i przetwarzanie danych klienta Miro w nowym regionie.

**Jak to działa i ile to trwa?**

Zobacz Jak działa migracja danych między regionami i jak długo trwa.

**Kto jest uprawniony, a kto nie?**

Aby zautomatyzować migrację między regionami, musisz być klientem Enterprise. Jednak klient Enterprise korzystający z rozwiązania Enterprise Guard i zarządzania kluczami szyfrowania jest niekwalifikowany. Aby uzyskać więcej informacji, skontaktuj się ze swoim przedstawicielem Miro.

**Jakie dane są uwzględnione w zautomatyzowanej migracji między regionami?**

Aby dowiedzieć się, jakie dane są uwzględnione w zautomatyzowanej migracji między regionami, zobacz Dane uwzględnione w zautomatyzowanej migracji między regionami.

**Jakie dane nie są uwzględniane w zautomatyzowanej migracji danych między regionami?**

Zautomatyzowana migracja między regionami nie obejmuje następujących danych:

- Aplikacje i integracje, w tym SSO i SCIM, które muszą być ponownie skonfigurowane dla nowego regionu
- Nagrania Talktrack
- Powiadomienia w aplikacji są usuwane

**Czy wiąże się to z dodatkowymi kosztami?**

Tak. Zautomatyzowana migracja danych między regionami jest płatną usługą oferowaną przez Miro Services. Aby uzyskać więcej informacji, skontaktuj się z osobą kontaktową w Miro.

**Jak Miro zapewnia usunięcie danych mojej organizacji z regionu źródłowego?**

Aby usunąć dane z regionu źródłowego po migracji między regionami, Miro stosuje następujący protokół:

- Dane pozostają w regionie źródłowym przez 30 dni, co zapewnia dostępność niezawodnej kopii zapasowej w przypadku problemu z migracją.
- Po 30 dniach Miro rozpoczyna usuwanie danych z regionu źródłowego.
- Po maksymalnie 120 dniach od daty początkowej migracji, Miro usuwa wszystkie dane z regionu źródłowego.

**Co widzą użytkownicy podczas migracji między regionami?**

Aby dowiedzieć się więcej o doświadczeniu użytkowników podczas migracji, zobacz [Doświadczenie użytkowników podczas przenoszenia danych między regionami](../../canvas-25-admin-features/data-residency/04-user-experience-while-moving-data-between-regions.md).

**Co się dzieje, jeśli migracja się nie powiedzie?**

Jeśli migracja nie powiedzie się z jakiegokolwiek powodu, Miro przywraca dostęp do Twojego źródłowego regionu i koordynuje nową datę na ponowienie migracji.
