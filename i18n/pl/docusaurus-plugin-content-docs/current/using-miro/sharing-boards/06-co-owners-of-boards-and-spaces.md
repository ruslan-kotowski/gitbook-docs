---
title: Współwłaściciele tablic i przestrzeni
article_id: 360021580759
translation_id: 360021580759
locale: pl-pl
sidebar_position: 6
created_at: '2021-05-12T07:36:28Z'
updated_at: '2026-01-06T19:03:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: board-roles-and-permissions
availability:
  notes: 'Kto może to zrobić: Właściciele tablic, współwłaściciele tablic, właściciele
    przestrzeni, współwłaściciele przestrzeni, administratorzy zespołu, administratorzy
    firmy Które abonamenty: Business, Enterprise Na jakich platformach: Przeglądarka,
    komputeroway, urządzenie mobilne.'
---

Rola współwłaściciela wzmacnia współpracę, umożliwiając właścicielom tablic delegowanie obowiązków związanych z przygotowaniem i ułatwianiem pracy na tablicy, niezależnie od tego, czy jest to sesja na żywo, czy asynchroniczna.

Współwłaściciel zapewnia płynny przepływ pracy, nawet gdy główny właściciel tablicy jest niedostępny, ponieważ może wykonywać prawie wszystkie działania na poziomie właściciela, od zarządzania ustawieniami tablicy po kontrolowanie widoczności treści. Współwłaściciel pomaga rozdzielać obciążenie pracą i zapewnia niezawodne wsparcie w zarządzaniu tablicą.

Aby dowiedzieć się, jakie uprawnienia ma współwłaściciel tablicy lub przestrzeni, zobacz Dokumentację współwłaścicieli.

## Włączyć rolę współwłaściciela dla organizacji

Jako administrator firmy wykonaj następujące czynności:

1. Na pulpicie Miro kliknij swój awatar w prawym górnym rogu i wybierz **Konsolę administratora**.
2. Przejdź do **Bezpieczeństwo** > **Udostępnianie** > **Role i uprawnienia**.
3. Przełącz **Zezwalaj na rolę współwłaściciela** w pozycję włączoną.

Administratorzy mogą teraz włączyć rolę współwłaściciela dla swoich zespołów.

## Włącz rolę współwłaściciela w zespole

Jako administrator firmy lub administrator zespołu, wykonaj te kroki:

1. Na pulpicie Miro kliknij swój awatar w prawym górnym rogu i wybierz **Konsola administratora** | **Ustawienia**.
2. Przejdź do **Zespoły** > **\{team name\}** > **Ustawienia**.
3. W sekcji **ustawienia współpracy** przełącz **włącz rolę współwłaściciela na tablicach i w przestrzeniach** na włączoną pozycję.

## Dodaj współwłaścicieli do tablic

Jako właściciel tablicy lub istniejący współwłaściciel, wykonaj następujące kroki:

1. Z pulpitu Miro wykonaj jedną z następujących czynności:
   1. Aby przejść do tablicy, kliknij menu z 3 kropkami (**...**) i wybierz **Udostępnij**.
   2. Otwórz tablicę, a następnie kliknij **Udostępnij** w prawym górnym rogu.
2. Wprowadź adres e-mail użytkowników, których chcesz dodać jako współwłaścicieli.
3. Aby zmienić ich prawa dostępu, kliknij **Jest współwłaścicielem**.
4. (Opcjonalnie) Dodaj niestandardową wiadomość.
5. Kliknij **Wyślij zaproszenia**.

> Możesz przypisać rolę współwłaściciela tylko uczestnikom zespołu. Aby dodać współwłaściciela spoza zespołu, najpierw zaproś go do zespołu.

## Dodaj współwłaścicieli do przestrzeni

Jako właściciel przestrzeni lub istniejący współwłaściciel wykonaj następujące czynności:

1. Z pulpitu nawigacyjnego Miro wykonaj jedną z następujących czynności:
   1. Dla przestrzeni w pasku bocznym kliknij menu z 3 kropkami (**...**) i kliknij **Udostępnij**.
   2. Otwórz przestrzeń, a następnie kliknij etykietę u góry, która pokazuje liczbę uczestników.
2. Kliknij **Zarządzaj dostępem**.
3. Dla członka przestrzeni, zaktualizuj jego uprawnienia do **współwłaściciela.**

> Możesz przypisać rolę współwłaściciela tylko członkom przestrzeni. Aby dodać współwłaściciela spoza przestrzeni, najpierw zaproś go do przestrzeni.

> Współwłaściciel przestrzeni ma uprawnienia edytora do całej zawartości w tej przestrzeni.

## Referencja współwłaścicieli

### Uprawnienia współwłaściciela tablicy

Oprócz wszystkich uprawnień edytującego współwłaściciel tablicy ma następujące uprawnienia:

- **Zarządzaj ustawieniami zawartości tablicy i ustawieniami narzędzi do współpracy**
  Kontroluj, kto może kopiować zawartość tablicy i zarządzać narzędziami, takimi jak timer, głosowanie, czat wideo, udostępnianie ekranu i zarządzanie uwagą.
- **Ukryj i odsłoń ramki**
  Kontroluj widoczność zawartości ramki podczas prezentacji lub warsztatów.
- **Dodaj blokadę chronioną**
  Zapobiegaj przypadkowemu przenoszeniu lub usuwaniu treści podczas współpracy.
- **Dodaj hasło do tablicy**
  Zabezpiecz tablice publiczne, wymagając hasła do uzyskania dostępu.
- **Pobierz kopię zapasową tablicy**
  Twórz zarchiwizowane kopie tablic. Współwłaściciele mogą również przywracać tablice z kopii zapasowych.
- **Dodaj współwłaścicieli**
  Nadaj status współwłaściciela innym użytkownikom.
- **Zmień szczegóły tablicy**
  Zmień okładkę i zmień nazwę tablicy
- **Udostępnij tablicę**
  Modyfikuj uprawnienia dostępu dla zespołu i innych użytkowników na tablicy
- **Skonfiguruj zaawansowane uprawnienia do udostępniania tablicy**
  Określ, czy tablica może być udostępniona poza zespół lub organizację.

:::note
W abonamencie Enterprise, współwłaściciele tablic i administratorzy treści mogą przenosić tablice za pomocą [Miro REST API](https://developers.miro.com/reference/update-board), co różni się celowo od doświadczenia w interfejsie Miro, gdzie tylko właściciele mogą przenosić swoje tablice.
:::

Współwłaściciel tablicy nie może wykonywać następujących operacji:

- Usuń tablicę
- Przenieś tablicę do innego zespołu
- Zmień właściciela tablicy

### Uprawnienia współwłaściciela przestrzeni

Oprócz wszystkich uprawnień edytującego, współwłaściciel przestrzeni ma następujące uprawnienia:

- Zmień nazwę przestrzeni
- Udostępnij przestrzeń
- Modyfikuj uprawnienia dostępu dla zespołu i innych użytkowników w przestrzeni
- Dodaj współwłaścicieli do przestrzeni

Współwłaściciel przestrzeni nie może wykonać następujących operacji:

- Usuń przestrzeń
- Zmień właściciela przestrzeni

## FAQ

**Nie mam opcji przypisania współwłaściciela. Dlaczego?**

Funkcja współwłaściciela jest dostępna w wersjach Business i Enterprise. Administrator firmy musi aktywować tę funkcję w ustawieniach zespołu lub firmy. Tylko obecni uczestnicy zespołu mogą być promowani na współwłaścicieli. Upewnij się, że użytkownik został zaproszony do tablicy za pośrednictwem poczty e-mail, zanim spróbujesz przypisać mu rolę współwłaściciela.

**Jestem administratorem z włączonymi uprawnieniami administratora treści. Dlaczego nie mogę dodać współwłaścicieli tablicy?**

Administratorzy z uprawnieniami administratora treści (CAP) muszą najpierw dodać siebie jako właściciela do określonej tablicy. Po zostaniu właścicielem tablicy, będziesz mógł przypisać współwłaścicieli.

**Czy powinienem dodatkowo płacić za współwłaścicieli zaproszonych do moich tablic?**

Tylko istniejący uczestnicy zespołu mogą być wyznaczeni jako współwłaściciele. Jeśli użytkownik, którego chcesz uczynić współwłaścicielem, nie jest jeszcze częścią twojego zespołu, najpierw będziesz musiał(a) go zaprosić do zespołu, co może wiązać się z zakupem dodatkowej licencji, w zależności od twojego abonamentu i obecnej liczby użytkowników. Po tym, jak zostaną członkiem zespołu, możesz przypisać im rolę współwłaściciela.
