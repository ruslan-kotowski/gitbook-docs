---
title: "Jak przenie\u015B\u0107 tablic\u0119"
article_id: 360017730093
translation_id: 21358610443410
locale: pl-pl
sidebar_position: 4
created_at: '2024-09-13T18:53:06Z'
updated_at: '2026-03-27T16:09:48Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  roles: board_owner
  notes: 'Relevant for: All plans'
backstage_link:
  entity_kind: capability
  entity_id: move-board-to-space
---

> **Kto może to zrobić:** Właściciele tablic
> **Dotyczy:** Wszystkie abonamenty

Każdy użytkownik Miro może być członkiem wielu zespołów. Twój profil Miro to Twój adres e-mail. Możesz przenieść tablicę Miro z jednego zespołu do innego lub przenieść swoją tablicę Miro na inny profil.

:::note
W wersjach Enterprise współwłaściciele tablic i administratorzy treści mogą przenosić tablice korzystając z [Miro REST API](https://developers.miro.com/reference/update-board), co celowo różni się od doświadczenia w interfejsie Miro, gdzie tylko właściciele mogą przenosić swoje tablice.
:::

:::note
Administratorzy firmy w wersji Enterprise mogą [ograniczyć opcję przenoszenia tablic do i z zespołu](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md) dla wszystkich użytkowników niebędących administratorami oraz właścicieli tablic.
:::

## Najczęstsze scenariusze

Oto kilka najczęstszych scenariuszy związanych z przenoszeniem tablic, wraz z odpowiednimi sekcjami artykułu, które wyjaśniają, jak to zrobić:

- Masz **dwa profile Miro** (adresy e-mail powiązane z Miro) i chcesz przenieść tablice z jednego profilu na drugi.
  *Postępuj zgodnie z krokami opisanymi w* [*tej sekcji*](04-how-to-move-a-board.md)*, używając zakładki **Free plan**.*
- Przeszedłeś z **bezpłatnego planu na płatny plan** i chcesz przenieść tablice do płatnego planu.
  *Postępuj zgodnie z krokami opisanymi w* [*tej sekcji*](04-how-to-move-a-board.md)*, używając zakładki **Free plan**.*
- Chcesz **przenieść tablice między dwoma płatnymi zespołami**.
  *Postępuj według kroków opisanych w* [*tej sekcji*](04-how-to-move-a-board.md)*, używając karty **Paid, Education plans**.*

## Przenoszenie tablic między zespołami

:::warning
Przeniesienie tablicy do innego zespołu spowoduje utratę [historii wersji](12-board-history-versions.md). Jeśli chcesz zachować historię wersji, zalecamy zamiast tego [skopiowanie zawartości tablicy](../working-on-the-board/09-copy-as-text-or-as-an-image.md).
:::

Aby przenieść tablicę między zespołami, musisz:

- być właścicielem tablicy
- być członkiem obu zespołów

Istnieją dwa sposoby przeniesienia tablicy do innego zespołu: z poziomu pulpitu lub bezpośrednio w tablicy.

### Jak przenieść tablicę bezpośrednio w tablicy

1. Otwórz swoją tablicę i kliknij ikonę menu z 3 kropkami (**…**) po prawej stronie nazwy tablicy (w lewym górnym rogu)
2. Przejdź do **Tablica > Przenieś do > Inny zespół![moving-board-three-dots.png](../../../../../../docs/using-miro/managing-boards/images/21537437708306_moving-board-three-dots.png)**

### Jak przenieść tablicę używając pulpitu

1. Przejdź do swojego pulpitu, aby zobaczyć wszystkie tablice w zespole.
2. Najedź kursorem na kartę tablicy, którą chcesz przenieść.
3. Kliknij menu z 3 kropkami, a następnie wybierz **Przenieś do zespołu**.
   Otworzy się okno dialogowe.
4. Wybierz organizację, do której chcesz przenieść tablicę.
5. Wybierz zespół w tej organizacji.
6. Kliknij **Przenieś**.

### Jak przenieść tablicę do innej przestrzeni

1. Otwórz swoją tablicę i kliknij ikonę menu z 3 kropkami (**...**) bezpośrednio po prawej stronie nazwy tablicy (górny lewy róg)
2. Przejdź do **Tablica > Przenieś do > Inna przestrzeń.** Możesz dodatkowo powiadomić członków zespołu, że tablica została przeniesiona do innej przestrzeni.![moving-boards-spaces.png](../../../../../../docs/using-miro/managing-boards/images/21537453797394_moving-boards-spaces.png)*Przenoszenie tablicy do innej przestrzeni*

### Odmowa dostępu użytkownikowi

Jeśli którekolwiek ze współpracowników tablicy nie są częścią zespołu, do którego przenoszona jest tablica, zobaczysz komunikat o odmowie dostępu.

Istnieją dwa sposoby, aby sprawdzić, które adresy e-mail użytkowników stracą dostęp do tablicy po jej przeniesieniu. Jeśli liczba użytkowników jest mniejsza niż 10, listę adresów e-mail można zobaczyć po kliknięciu **Zobacz adresy użytkowników** w **komunikacie o odmowie dostępu.** Jeśli liczba przekracza 10, będzie dostępny link do pobrania listy e-maili.

Aby upewnić się, że wszyscy współpracownicy zachowają dostęp do tablicy, możesz [zaprosić członków do nowego zespołu](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) przed przeniesieniem tablicy.

Możesz również wybrać **Przenieś mimo to** i ponownie dodać współpracowników do tablicy po jej przeniesieniu.

![warning when moving a board.png](../../../../../../docs/using-miro/managing-boards/images/16759524012690_warning%20when%20moving%20a%20board.png)
*Komunikat o odmowie dostępu podczas przenoszenia tablicy z jednego zespołu do drugiego*

**Jeśli przeniesiesz tablicę do zespołu Free**, będzie ona udostępniona wszystkim członkom zespołu.

![private boards are not available in free teams.png](../../../../../../docs/using-miro/managing-boards/images/16759539790738_private%20boards%20are%20not%20available%20in%20free%20teams.png)
*Prywatne tablice nie są dostępne w zespołach Free*

## Przenoszenie tablic między profilami

Twój profil w Miro to adres e-mail, z którym się zarejestrowano. Jeśli zarejestrowałeś(-aś) się z dwoma różnymi adresami e-mail, oznacza to, że masz dwa profile. Możesz przenieść tablicę z jednego profilu na drugi.

### Jak przenieść tablice między profilami

Płatne, Education wersje Wersja Free

Jeśli tablica znajduje się w płatnym zespole lub zespole Education i chcesz przenieść ją do innego płatnego zespołu lub zespołu Education, po prostu zapisz kopię zapasową tablicy i prześlij ją do tego zespołu.

1. Otwórz swój pulpit.
2. Najedź myszką na kartę tablicy, którą chcesz przenieść.
3. Kliknij menu z 3 kropkami.
4. Kliknij **Pobierz kopię zapasową tablicy**.
5. Plik .rtb zostanie zapisany na Twoim urządzeniu.

   ![board-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136352530_board-backup.png)
6. Zaloguj się na swój drugi profil Miro.
7. Przełącz się na zespół, do którego chcesz przenieść tablicę.
8. Kliknij **+ Utwórz nowe** > **Importuj** > **Importuj kopię zapasową**.
9. Zostanie otwarty selektor plików.
10. Wybierz uprzednio zapisaną kopię zapasową pliku .rtb i kliknij **Otwórz**. Tablica będzie wtedy dostępna z twojego pulpitu.

    ![board-import-backup.png](../../../../../../docs/using-miro/managing-boards/images/23122136353682_board-import-backup.png)

Postępuj zgodnie z poniższymi krokami, jeśli Twoja tablica znajduje się w free zespole lub musisz przenieść tablicę do free zespołu.

1. Zaloguj się do Miro za pomocą profilu #1.
2. Udostępnij tablicę profilowi #2. Kliknij **Udostępnij**.
   ![free-sharing-board.png](../../../../../../docs/using-miro/managing-boards/images/23122136354066_free-sharing-board.png)
3. Wpisz e-mail dla profilu #2 > kliknij **Wyślij zaproszenia**.

   ![free-sharing-board-dialog.png](../../../../../../docs/using-miro/managing-boards/images/23122136354706_free-sharing-board-dialog.png)
4. Przenieś własność tablicy z profilu #1 do profilu #2. Kliknij przycisk **Udostępnij** > **Ustawienia udostępniania** > wybierz profil #2 > wybierz **Właściciel** z menu rozwijanego.
5. Zaloguj się do Miro na profil #2, gdzie zobaczysz tablicę.
6. Przenieś tablicę do innego zespołu.

:::warning
Jeśli Twój drugi profil jest na abonamencie Free, a zapraszasz swój darmowy profil do płatnego profilu, zajmujesz jedno miejsce (licencję) w swoim płatnym abonamencie. Jeśli to przekroczy liczbę miejsc w Twoim abonamencie, możesz zostać obciążony(a) opłatą za dodatkowe miejsce (licencję).
:::

## Często zadawane pytania

**Dlaczego nie widzę opcji przeniesienia do zespołu w menu mojej tablicy?**

Tylko właściciele tablic, którzy są członkami kilku zespołów, mogą przenosić tablice między nimi. Jeśli nie jesteś właścicielem tablicy, możesz [duplikować tablicę](03-how-to-duplicate-a-board.md) (jeśli jest to dozwolone w [ustawieniach zawartości tablicy](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md)) i przenieść kopię tablicy.

Opcja przenoszenia tablic może być również ograniczona przez administratorów firmy w wersji Enterprise.

**Jak mogę przekazać własność mojej tablicy innemu użytkownikowi?**

Dowiedz się, jak [przenieść własność tablicy na innego współpracownika](05-how-to-transfer-board-ownership.md).

**Czy link do tablicy zmienia się, gdy przenoszę tablicę do innego zespołu?**

Nie, adres URL tablicy nie zmienia się.

**Czy mogę przenieść szablonową tablicę do zespołu innego użytkownika?**

Tak, możesz poprosić tego użytkownika, aby zaprosił Cię do swojego zespołu, a następnie przenieść tablicę, lub [udostępnij tablicę](../sharing-boards/03-sharing-boards-and-inviting-collaborators.md) i pozwól mu [zduplikować Twoją tablicę](03-how-to-duplicate-a-board.md) w [ustawieniach zawartości tablicy](../sharing-boards/14-how-to-allow-or-restrict-copying-and-exporting-boards-and-content.md).

**Czy mogę przenosić przestrzenie między zespołami?**

Nie, możesz przenosić tylko pojedyncze tablice.

**Czy mogę przenieść kilka tablic jednocześnie?**

Nie, ta funkcja nie jest obecnie obsługiwana.

**Próbuję przenieść moją tablicę i nic się nie dzieje lub pojawia się komunikat o błędzie - co mam zrobić?**

Spróbuj przenieść tablicę w innej przeglądarce lub w trybie incognito. Możesz także spróbować przełączyć się na inną sieć lub urządzenie.

Inną opcją jest [duplikowanie tablicy](03-how-to-duplicate-a-board.md) i przeniesienie kopii tablicy. Jeśli to nie pomoże, [zgłoś problem do Pomocy Miro](../tools/troubleshooting/06-contacting-miro-support.md).
