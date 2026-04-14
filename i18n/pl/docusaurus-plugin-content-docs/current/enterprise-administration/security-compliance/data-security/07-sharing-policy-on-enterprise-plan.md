---
title: Zasady udostępniania w wersji Enterprise
article_id: 360017730133
translation_id: 360017730133
locale: pl-pl
sidebar_position: 7
created_at: '2019-02-11T10:09:02Z'
updated_at: '2025-11-25T16:00:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Dostępne w wersjach: Wersja Enterprise Wymagana rola: Administrator firmy'
---

Bezpieczeństwo danych i poufność to istotne kwestie dla większości przedsiębiorstw. Dlatego nasza wersja Enterprise dostarcza egzekwowane narzędzia do kontrolowania ryzyk związanych z bezpieczeństwem informacji. Obejmują one bezpieczniejsze zarządzanie dostępem z opcją jednokrotnego logowania opartego na SAML oraz lepszą kontrolę praw i uprawnień użytkowników dzięki rozszerzonym możliwościom administracyjnym. Dodatkowo wprowadzamy opcjonalne ograniczenia: udostępnianie poza dozwolonymi domenami i udostępnianie za pomocą publicznego linku.

:::note
Ustawienia zasad udostępniania wpływają również na dostępne ustawienia dostępu podczas osadzania tablic w konkretnej aplikacji. Dowiedz się więcej: [Zarządzanie zasadami udostępniania Enterprise dla integracji osadzania](../../managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

## Ogranicz udostępnianie poza dozwolone domeny

Na poziomie firmy Na poziomie zespołu

Gdy już ustawisz dozwolone domeny na poziomie firmy, opcja udostępniania tablic poza tymi domenami zostanie ograniczona dla wszystkich członków firmy i zespołów.

1. Przejdź do **ustawień firmy** > **bezpieczeństwa** > **udostępniania**.
2. Włącz **Ogranicz dozwolone domeny**.
3. Dodaj listę zaufanych domen używanych w ramach Twojej wersji Enterprise.

Aby włączyć udostępnianie [współpracownikom-gościom](../../../using-miro/sharing-boards/07-collaboration-with-guests.md) i ominąć listę dozwolonych, zaznacz pole **Zezwalaj na udostępnianie gościom poza tymi domenami**.

Kiedy **Zezwalaj na udostępnianie gościom poza tymi domenami** jest włączona, użytkownicy z domenami spoza listy dozwolonych mogą mieć udostępniane tablice, ale nadal nie będą mogli znaleźć zespołów pod [odkrywalnością zespołu.](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)

![sharing-allowed-domains.png](https://help.miro.com/hc/article_attachments/26575879408786)
*Lista zaufanych domen i opcja udostępniania gościom spoza tych domen*

Wszyscy użytkownicy zaproszeni do subskrypcji przed włączeniem ustawienia pozostaną w Twojej wersji i zachowają dostęp do udostępnionej zawartości. Jednak nie będzie możliwe udostępnianie im innej zawartości.

Dodatkowo możesz **zweryfikować wszystkich użytkowników względem listy dozwolonych** w przypadku, gdy istnieją użytkownicy, których domena nie jest dozwolona. Możesz usunąć ich w następującym wyskakującym okienku:

![validate_against_the_allowlist.jpg](https://help.miro.com/hc/article_attachments/26575879410066)*Użytkownicy, których adresy e-mail nie są zgodne z listą dozwolonych*

Ograniczając dostęp na poziomie zespołu, użytkownicy spoza dozwolonych domen nie będą mogli uzyskać dostępu ani nie zostaną zaproszeni do zespołu ani do tablic w nim. Opcja pozwala włączyć ustawienia dla konkretnego zespołu bez ograniczania zasad udostępniania dla wszystkich użytkowników Enterprise. Daje ci to również możliwość zezwolenia na konkretną domenę dla zespołu bez konieczności zezwalania na nią dla całej firmy.

:::note
Jeśli domeny na liście dozwolonych nie są skonfigurowane na poziomie zespołu, obowiązują ustawienia firmy. Jeśli lista dozwolonych na poziomie zespołu jest skonfigurowana, nadpisuje ona ograniczenia na poziomie firmy. Na przykład, jeśli **domena 1** znajduje się na liście dozwolonych na poziomie firmy, a **domena 2** jest na liście dozwolonych na poziomie zespołu, **domena 1** nie będzie dozwolona na poziomie zespołu, chyba że zostanie dodana do listy dozwolonych na poziomie zespołu.
:::

Aby skonfigurować dozwolone domeny dla konkretnego zespołu:

1. Przejdź do **Zespoły** i wybierz zespół, który chcesz skonfigurować.
2. Przejdź do **Ustawienia** i przewiń w dół do **Dozwolone domeny dla zespołu**.
3. Włącz przełącznik **Ogranicz dozwolone domeny**.
4. Wprowadź swoje dozwolone domeny i kliknij **Dodaj**.
   Aby umożliwić udostępnianie gościom spoza domen, zaznacz pole **Włącz udostępnianie gościom spoza dozwolonych domen**.

![sharing-team-allowed-domains.png](https://help.miro.com/hc/article_attachments/26575887748370)
*Opcja ograniczenia dozwolonych domen dla konkretnego zespołu w ramach subskrypcji Enterprise*

Gdy ograniczysz udostępnianie poza dozwolone domeny, użytkownicy firmowi będą mogli udostępniać swoje tablice tylko użytkownikom z określonych domen. Jeśli to ustawienie jest włączone, a użytkownik firmy spróbuje udostępnić swoją tablicę do domeny, która nie jest dozwolona, otrzyma następujący komunikat:

![can_t_share_outside_the_allowlist.jpg](https://help.miro.com/hc/article_attachments/26575887749010)*Tablica nie może być udostępniona użytkownikowi, którego domena nie jest na liście dozwolonych*

:::note
Jeśli udostępnianie za pomocą linku publicznego jest dozwolone w Twojej firmie, [tablice publiczne](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#udostepnianie-tablic-za-pomoca-linku-publicznego) mogą być nadal dostępne dla *każdego, kto posiada link do tablicy* (oraz hasło, jeśli zostało ustawione).
:::

## Ogranicz udostępnianie przez link publiczny

Administratorzy firmy mogą ograniczyć wszystkich użytkowników firmy lub członków konkretnego zespołu od [publicznego udostępniania tablic firmowych](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#udostepnianie-tablic-za-pomoca-linku-publicznego). Kiedy to ustawienie jest wyłączone, opcja **Kto ma link** znika z menu Udostępnianie tablic w firmie lub zespole.

Na poziomie firmy Na poziomie zespołu

Aby ograniczyć udostępnianie publiczne dla wszystkich użytkowników firmy:

1. Przejdź do **firmy** **Ustawienia >** **Bezpieczeństwo > Udostępnianie**.
2. Wyłącz **Tablice mogą być udostępniane publicznie**.

Wykonanie tej czynności usunie opcję "Każdy, kto ma link" z menu Udostępnianie tablicy. Oznacza to również, że wszystkie tablice, które zostały wcześniej udostępnione przez link publiczny lub osadzone na stronach, staną się niedostępne dla użytkowników publicznych, a ich aktywne sesje na tablicach zostaną zamknięte.

Jeśli administratorzy ponownie włączą możliwość publicznego udostępniania tablic, użytkownicy będą musieli ręcznie reaktywować publiczne udostępnianie dla każdej tablicy.

Jeśli chcesz zezwolić na edycję publicznie udostępnionych tablic, zaznacz opcję **Zezwalaj na edycję tablic dostępnych publicznie***.* Jeśli *odznaczysz pole wyboru,* dostęp publiczny do wszystkich tablic wcześniej udostępnionych do edycji publicznej będzie ograniczony.

:::note
Udostępnianie za pomocą linku publicznego jest domyślnie włączone na poziomie zespołu i ustawione jako „Każdy może wyświetlać i komentować” dla nowo utworzonych zespołów. Jednak jeśli jest to **wyłączone** na poziomie firmy, zespoły nie mogą udostępniać tablic publicznie, nawet jeśli jest to dozwolone na poziomie zespołu.
:::

Aby ograniczyć publiczne udostępnianie tablic dla konkretnego zespołu:

1. Przejdź do **zespołów** i wybierz zespół, który chcesz skonfigurować.
2. Przejdź do **Ustawienia** i przewiń w dół do **Ustawienia udostępniania**.
3. W sekcji **Udostępnianie tablic** > **Za pomocą linku publicznego**, zobaczysz trzy opcje: możesz zdecydować, czy zezwolić na publiczne udostępnianie tylko do wyświetlania i komentowania, do wyświetlania, komentowania i edycji, czy też ograniczyć publiczne udostępnianie dla zespołu.

![sharing-public-link.png](https://help.miro.com/hc/article_attachments/26575879424402)
*Opcja konfiguracji udostępniania poprzez link publiczny dla zespołu w ramach subskrypcji Enterprise*

**Wygaśnięcie linku publicznego (poziom firmy)**

Aby zwiększyć bezpieczeństwo publicznie udostępnianych tablic, włącz wygaśnięcie linku publicznego. Oznacza to, że wszelkie linki do tablicy udostępnione odwiedzającym przestaną działać po upływie określonego czasu, jeśli tablica nie zostanie otwarta. Dotyczy to wszystkich tablic, gdy wygaśnięcie linku publicznego zostanie włączone w ustawieniach firmy.

Aby włączyć wygaśnięcie linku publicznego:

1. Przejdź do **Ustawienia firmy > Bezpieczeństwo > Udostępnianie**.
2. Przewiń w dół do sekcji **Zawartość**.
3. Zaznacz pole wyboru dla **Wygasa link do udostępniania publicznego**.
4. Ustaw liczbę dni, po których nieaktywne linki wygasają. Możesz wybrać od 30 do 999 dni.

:::warning
Jeśli hasło na tablicy zostanie zresetowane, data wygaśnięcia tablicy również zostanie zresetowana.
:::

## Wymagaj haseł dla publicznych tablic (poziom firmy)

Możesz także egzekwować obowiązkowe hasła dla wszystkich tablic udostępnianych publicznie przez link.

1. Przejdź do **Ustawienia firmy > Bezpieczeństwo > Udostępnianie**.
2. Przewiń w dół do sekcji **Zawartość**.
3. Zaznacz pole **Wymagaj haseł dla publicznie udostępnianych tablic**.

Po zaznaczeniu tej funkcji, zostanie to natychmiast zastosowane do tablic wcześniej dostępnych z publicznym linkiem, a wszystkie tablice w przyszłości nie będą mogły być dostępne publicznie bez hasła.

- *W przypadku tablic wcześniej dostępnych za pomocą* [*publicznego linku*](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#udostepnianie-tablic-za-pomoca-linku-publicznego) *bez haseł:*
  Jeśli tablice były wcześniej dostępne za pomocą publicznego linku bez haseł, otwarte sesje zostaną unieważnione, a odwiedzający zostaną poproszeni o wprowadzenie hasła, jeśli spróbują uzyskać dostęp do wcześniej dostępnego linku.
- *We wszystkich tablicach:*
  Aby tablica była publicznie dostępna przez link, jej właściciel lub [administrator treści](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) musi ustawić hasło. Jeśli hasło zostanie usunięte, opcja **Każdy, kto ma link** w menu Udostępnianie tablicy zostanie zmieniona na **Brak dostępu**. Członkowie zespołu z uprawnieniami do edycji mogą udostępniać tablicę za pomocą publicznego linku, jeśli hasło zostało już ustawione, w przeciwnym razie muszą skontaktować się z właścicielem tablicy, aby ustawić hasło.
- Gdy opcja "*Dezaktywuj link, jeśli tablica była nieaktywna przez 'x' dni*" jest ustawiona, w oknie dialogowym Udostępnianie pojawi się ikona zegara z informacją, że publiczny dostęp zniknie po określonej liczbie dni.
  ![1-2.png](https://help.miro.com/hc/article_attachments/26575887758738)
*Opcja udostępniania publicznego w wersji Enterprise z obowiązkowymi hasłami*

Możesz również wymagać skomplikowanych haseł i określić, jakie wymagania muszą one spełniać. Mogą obejmować:

- Minimalna długość hasła (od 6-14 znaków; domyślnie 8).
- Wielkie i małe litery.
- Liczby.
- Znaki specjalne.

![complex-board-password.png](https://help.miro.com/hc/article_attachments/26575887760786)
*Ustawienia dla złożonych haseł do tablic*

## Ogranicz udostępnianie na poziomie zespołu i firmy (poziom zespołu)

:::note
Udostępnianie w zakresie zespołu i firmy jest włączone domyślnie, jeśli ustawienia nie zostały dostosowane przez administratora firmy.
:::

Administratorzy firmy Enterprise mogą również włączyć/wyłączyć udostępnianie w zakresie całej firmy lub zespołu.

1. Przejdź do **Zespoły** i wybierz zespół, który chcesz skonfigurować.
2. Przejdź do **Ustawienia** i przewiń w dół do **Ustawień udostępniania**.
3. W **udostępnianiu tablic**, wybierz, czy udostępnianie zespołowi jest dozwolone czy nie. Dla ustawień obejmujących całą firmę, wybierz, czy firma może wyświetlać i komentować udostępnione tablice, wyświetlać/komentować/edytować, czy udostępnianie nie jest dozwolone.![sharing-board-sharing.png](https://help.miro.com/hc/article_attachments/26575879435538)*Ustawienia udostępniania tablic w wersji Enterprise*

Włączenie udostępniania tablic zespołowi pozwala członkom zespołu łatwo udostępniać swoje tablice i projekty całemu zespołowi.

Wyłączenie tej opcji usunie ją z menu Udostępnianie tablic i projektów zespołu. Wcześniej udostępnione tablice i projekty nie będą już dostępne dla użytkowników zespołu, chyba że zostaną udostępnione innymi sposobami.

Jeśli administrator ponownie włączy możliwość udostępniania zespołowi, wcześniej udostępnione tablice i projekty nie będą automatycznie udostępniane zespołowi i użytkownicy będą musieli ponownie je udostępnić ręcznie.

![1-3.png](https://help.miro.com/hc/article_attachments/26575887765394)
*Opcja udostępniania tablicy zespołowi może być ukryta w menu Udostępnianie*

Użytkownicy w wersjach Enterprise z wyłączoną [ochroną prywatności zespołu](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) mogą również [udostępniać swoje tablice całej firmie do przeglądania, komentowania lub edycji jednym kliknięciem](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md). Możesz zablokować tę opcję dla konkretnego zespołu, wybierając **Niedozwolone** w ustawieniach **Dla całej firmy**. Lub możesz zezwolić na udostępnianie wyłącznie do wyświetlania i komentowania albo również do edycji.

Należy pamiętać, że jeśli [ochrona prywatności zespołu](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) jest włączona w Twojej firmie, opcja udostępniania tablic całej firmie nie będzie dostępna, nawet jeśli jest to dozwolone na poziomie zespołu.

![1-4.png](https://help.miro.com/hc/article_attachments/26575879443730)
*Opcja udostępniania tablicy całej firmie może być ukryta w menu Udostępnianie*

## Ogranicz możliwość przenoszenia tablic do innych zespołów (poziom zespołu)

:::note
Możliwość przenoszenia tablic do innych zespołów jest domyślnie włączona, jeśli ustawienie nie zostało dostosowane przez administratora firmy.
:::

Gdy administrator firmy nie zezwala na przenoszenie tablic dla zespołu, członkowie tego zespołu nie będą mogli przenosić tablic do innych zespołów ani z tego zespołu. Ustawienie jest konfigurowane dla każdego zespołu w **Ustawienia zespołu > Uprawnienia**.

:::note
Użytkownicy niebędący administratorami nie mogą przenosić tablic do zespołu, jeśli [opcja tworzenia tablic jest dla nich ograniczona](../../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md) w docelowym zespole.
:::

![sharing-moving-boards.png](https://help.miro.com/hc/article_attachments/26575879445266)
*Opcja ograniczenia przenoszenia tablic do i z zespołu*

## Ogranicz udostępnianie niestandardowych szablonów w całej firmie

> **Dostępne w wersjach:** Wersja Enterprise
> **Kto może to zrobić:** Administratorzy firmy

Administratorzy firmy mogą zezwolić lub ograniczyć udostępnianie niestandardowych szablonów na poziomie firmy. Gdy udostępnianie jest ograniczone, członkowie zespołu nie będą mogli udostępniać niestandardowego szablonu firmie bez zgody administratora.

1. Przejdź do **ustawienia firmy** > **bezpieczeństwo** > **ustawienia**.
2. Przewiń w dół do **Ról i uprawnień**.
3. Włącz **Ogranicz udostępnianie szablonów firmowych**.

![sharing-restrict-templates.png](https://help.miro.com/hc/article_attachments/26575879446802)
*Opcja ograniczenia udostępniania szablonów firmowych*

## Często zadawane pytania

Czy uczestnicy otrzymują powiadomienia, gdy administratorzy firmy zmieniają wyżej wymienione ustawienia udostępniania na poziomie zespołu lub firmy?

Nie, nie ma powiadomień w takich przypadkach. Zasady są stosowane natychmiast.

Czy mamy pulpit, na którym możemy śledzić wszystkie tablice udostępnione za pomocą linku publicznego?

Obecnie nie ma takiego pulpitu.

Wyłączyłem opcję ograniczania dozwolonych domen, ale nadal nie możemy udostępniać tablic użytkownikom spoza dozwolonych domen. Jak mogę to naprawić?

Możliwe, że ustawienie jest nadal aktywne na poziomie firmy / zespołu. Proszę sprawdź, czy ograniczenie jest wyłączone w ustawieniach firmy lub ustawieniach zespołu.
