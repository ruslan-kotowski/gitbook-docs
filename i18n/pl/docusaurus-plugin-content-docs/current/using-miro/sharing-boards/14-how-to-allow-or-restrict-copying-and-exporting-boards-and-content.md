---
title: Jak zezwolić lub ograniczyć kopiowanie i eksportowanie tablic oraz ich zawartości
article_id: 360018350399
translation_id: 360018350399
locale: pl-pl
sidebar_position: 14
created_at: '2020-12-14T06:10:03Z'
updated_at: '2026-01-22T14:23:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: export-pdf-canvas
availability:
  notes: 'Kto może to zrobić: Członkowie zespołu, administratorzy zespołu (Setup),
    administratorzy firmy (Setup) Plany: Starter, Business, Enterprise, Education
    Platformy: Przeglądarka, Komputer stacjonarny, Mobilne'
---

Administratorzy firmy i administratorzy zespołu mogą określić, czy członkowie zespołu i osoby spoza zespołu mogą kopiować treści z tablic, oraz ustawić domyślną opcję kopiowania dla nowych tablic.

Właściciele tablic i współwłaściciele tablic mogą określić ustawienia kopiowania dla innych członków zespołu na danej tablicy. Jeśli administratorzy zezwolą osobom spoza zespołu na kopiowanie tablic, co obejmuje odwiedzających i gości, właściciele tablic i współwłaściciele mogą również zezwolić na kopiowanie osobom spoza zespołu.

Jeśli administratorzy nie zezwolą osobom spoza zespołu na kopiowanie treści, opcja tablicowa umożliwiająca kopiowanie przez osoby spoza zespołu zostanie usunięta.

:::note
W wersji Free kopiowanie tablic jest domyślnie włączone i nie można tego zmienić.
:::

## Jak ustawić uprawnienia do kopiowania tablic dla zespołu

Dla danego zespołu, administrator firmy lub administrator zespołu mogą określić, czy osoby spoza zespołu mogą kopiować i eksportować tablice i zawartość oraz ustawić domyślne uprawnienia do kopiowania dla nowo utworzonych tablic.

Postępuj zgodnie z tymi krokami:

1. Przejdź do **Admin Console**.
2. Kliknij **Zespoły**.
3. Kliknij w wiersz **\{Team name\}**.
   Otworzy się panel **\{Team name\}**.
4. Kliknij, aby otworzyć kartę **Ustawienia**.
5. Przewiń do sekcji **Bezpieczeństwo treści**.
6. Dla opcji **Kopiowanie treści**, określ, czy tylko członkowie zespołu, czy wszyscy w organizacji mogą kopiować treści tablic.
7. Określ **Domyślne ustawienie kopiowania treści**. Właściciele tablic mogą zmieniać to ustawienie dla poszczególnych tablic.
   Twoje ustawienia są zapisywane automatycznie.

:::note
Jeśli kopiowanie treści tablic nie jest dozwolone dla osób spoza zespołu, opcja **Każdy z dostępem do tablicy** jest usuwana z ustawień tablicy. Na przykład odwiedzający i goście mają zakaz kopiowania treści.
:::

:::note
Kopiowanie obrazów między prywatnymi tablicami połączonymi z różnymi zespołami jest niemożliwe. Porozmawiaj ze swoim administratorem firmy Miro o uzyskaniu pozwolenia na dostęp do innej tablicy w celu kopiowania obrazów.
:::

## Jak ustawić pozwolenia na kopiowanie dla tablicy

Dla danej tablicy właściciel lub współwłaściciel tablicy mogą określić, kto może kopiować tablicę.

Postępuj zgodnie z tymi krokami:

1. Na tablicy, którą posiadasz, współposiadasz lub stworzyłeś, kliknij **Udostępnij** w prawym górnym rogu.
   Otworzy się okno modalne udostępniania.
2. W prawym dolnym rogu kliknij **Ustawienia udostępniania**.
3. W sekcji **Kto może kopiować zawartość tablicy**, określ jedną opcję.

   > ✏️ Jeśli administrator firmy lub administrator zespołu wyłączy opcję **Każdy z dostępem do tablicy**, to wtedy ta opcja nie jest dostępna.
4. Kliknij **Gotowe**.
   Twoje zmiany są zapisywane automatycznie i dotyczą wszystkich, którzy mają dostęp do tablicy.

## Opcje kopiowania tablicy w zależności od typu użytkownika

Zakładając, że **każda osoba z dostępem do tablicy** może kopiować jej zawartość, poniższa tabela pokazuje uprawnienia dla poszczególnych typów użytkowników.

|  | Zapisz tablicę jako szablon | Kopiuj zawartość tablicy | Eksportuj | Duplikuj | Pobierz pliki z tablicy |
| --- | --- | --- | --- | --- | --- |
| Członkowie zespołu | ✔ | ✔ | ✔ | ✔ | ✔ |
| Goście | ✘ | ✔ | ✔ | ✔ | ✔ |
| Odwiedzający z kontem Miro | ✘ | ✔ | ✔ | ✔ | ✔ |
| Odwiedzający bez konta Miro | ✘ | (Z uprawnieniami do edycji) ✔ | ✘ | ✘ | ✔ |

:::note
(Enterprise) Jeśli [przenoszenie tablic między zespołami jest niedozwolone](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md), opcja duplikowania tablicy jest niedostępna.
:::

:::note
Niektóre opcje nie są dostępne dla pewnych kategorii użytkowników, nawet jeśli właściciel tablicy umożliwia każdemu z linkiem kopiowanie zawartości tablicy
:::

## FAQ

*Dlaczego nie mogę kopiować i wklejać treści na tablicy Miro?*

Właściciel lub współwłaściciel tablicy może nie pozwolić na kopiowanie w Twojej roli. Możesz sprawdzić swoją rolę na pasku współpracy, w prawym górnym rogu tablicy Miro. Skontaktuj się z właścicielem lub współwłaścicielem tablicy, aby poprosić o uprawnienia do kopiowania dla swojej roli.

Warto również upewnić się, że jesteś zalogowany do Miro. Jeśli Twoja rola ma uprawnienia do kopiowania, a jesteś zalogowany, zaloguj się i otwórz tablicę w innej przeglądarce, a następnie spróbuj ponownie skopiować.

*Dlaczego opcja **Każdy, kto ma dostęp do tablicy** nie jest dla mnie dostępna?*

Administrator(zy) firmy lub administrator(zy) zespołu wyłączył(li) tę opcję. Jeśli jesteś administratorem firmy lub zespołu, zobacz jak ustawić uprawnienia do kopiowania tablicy dla zespołu.

*Jak umożliwić odwiedzającym pobieranie plików, jednocześnie ograniczając możliwość kopiowania lub duplikowania tablicy?*

Stwórz osobną tablicę zawierającą tylko pliki, po czym włącz kopiowanie zawartości tablicy dla każdego, kto ma link do tablicy. Udostępnij link do tej tablicy odwiedzającym.

Alternatywnie, możesz osadzić nową tablicę z plikami, z włączoną opcją kopiowania dla każdego mającego link, w oryginalnej tablicy. Więcej informacji na temat osadzania znajdziesz w artykule [Osadzanie tablicy Miro](../import-and-export/export/02-embed-a-miro-board.md).

*Dlaczego nie mogę znaleźć **Uprawnień** w menu **Udostępniania** tablicy?*

(Płatny) Tylko właściciel i współwłaściciel tablicy mogą określać uprawnienia do treści. (Free) Uprawnień do treści nie można zmienić z ich domyślnej wartości, która umożliwia kopiowanie wszystkim użytkownikom.

*Czy mogę określić, kto może przesyłać treści na moją tablicę?*

Każdy, kto ma prawa **Może edytować**, może przesyłać treści na Twoją tablicę.
