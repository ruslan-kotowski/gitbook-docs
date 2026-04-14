---
title: "Ustawienia zaprosze\u0144 w wersji Enterprise"
article_id: 4412315533842
translation_id: 4412315533842
locale: pl-pl
sidebar_position: 3
created_at: '2021-12-13T04:56:26Z'
updated_at: '2026-02-19T10:56:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: invitations
---

Skonfiguruj ustawienia zaproszeń w wersji Enterprise, aby zarządzać, kto może zapraszać nowych użytkowników do dołączenia do Twojego abonamentu. Możesz dostosować ustawienia zaproszeń do wymagań swoich zespołów i całej firmy.

> **Dostępne dla:** wersji Enterprise
> **Kto może to zrobić:** administratorzy firmy

:::tip
Jeśli jesteś nowym użytkownikiem Miro, dowiedz się więcej o [ustawieniach zespołu i firmy](../../administration/get-started-as-a-miro-admin/01-i-am-a-new-miro-admin.-where-to-start.md).
:::

## Ustawienia zaproszeń do zespołu

Dla sprawniejszej współpracy, pozwól **wszystkim członkom zespołu** zapraszać nowych członków do zespołu. Jeśli wolisz mieć większą kontrolę nad zaproszeniami, możesz ograniczyć tę opcję do administratorów firmy i/lub zespołu, tak aby wszystkie prośby o zaproszenie były wysyłane za pośrednictwem [zarządzania prośbami](09-request-management-on-enterprise-plan.md). Możesz również kontrolować, czy użytkownicy mogą zapraszać [gości](../../using-miro/sharing-boards/07-collaboration-with-guests.md) do zespołów.

### Jak skonfigurować ustawienia zaproszeń do zespołu

Aby zarządzać ustawieniami zaproszeń do zespołu, w konsoli administracyjnej przejdź do **Zespoły** i wybierz swój zespół. Otworzy się panel zespołu. W sekcji **Zaproszenia** wybierz jedną z następujących opcji:

- **Tylko administratorzy firmy**
  Tylko administratorzy firmy mogą dodawać nowych członków do zespołu.
- **Administratorzy firmy i zespołu**
  Administratorzy firmy i zespołu mogą zapraszać nowych członków do zespołu.
- **Wszyscy członkowie zespołu**
  Wszyscy członkowie zespołu mogą zapraszać nowych członków do zespołu.

:::note
W [programie elastycznych licencji (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) opcje zapraszania członków zespołu są uzupełnione przez ustawienia zapraszania firmowego.
:::

### Jak skonfigurować zapraszanie gości

Administratorzy firmy mogą pozwolić członkom na zapraszanie [gości](../../using-miro/sharing-boards/07-collaboration-with-guests.md) lub ograniczyć tę opcję. Goście mogą uzyskać dostęp tylko do tablic, na które zostali zaproszeni i nie potrzebują licencji.

Zaktualizuj ustawienia zapraszania gości w **Zespoły** > wybierz swój zespół > **Ustawienia** > **Zezwól gościom na dołączenie do zespołu [Name].**

:::note
Administratorzy firmy mogą włączyć automatyczną dezaktywację gości po 30 dniach nieaktywności.
:::

## Scenariusze zaproszeń

:::tip
W zależności od [ustawień zarządzania prośbami](09-request-management-on-enterprise-plan.md) prośby o udostępnienie tablicy lub zaproszenie użytkownika do zespołu mogą być wysyłane bezpośrednio do administratorów firmy, do konkretnych osób poprzez e-mail lub poprzez utworzenie zgłoszenia w serwisie pomocy.
:::

**Zapraszanie nowych członków do zespołu**

Jeśli goście nie są dozwoleni, a członkowie nie mogą zapraszać nowych członków, gdy próbują udostępnić tablicę, zobaczą poniższe powiadomienie i będą musieli złożyć prośbę.

**Nadawanie roli właściciela lub współwłaściciela**

Jeśli członkom nie wolno zapraszać nowych członków i próbują przydzielić rolę właściciela lub współwłaściciela gościowi lub [Free Restricted](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) członkowi na konkretnej tablicy, zobaczą poniższe powiadomienie i będą musieli złożyć prośbę.

**Zapraszanie zewnętrznego użytkownika lub gościa do edycji tablicy**

:::note
Zewnętrzni goście to goście spoza domeny Twojej firmy. Będą posiadać e-mail z zewnętrzną domeną firmy.
:::

Jeśli członkom zespołu nie wolno zapraszać nowych członków do zespołu i jeśli nie włączono uprawnień do edycji dla gości w zespole, to próba zaproszenia zewnętrznego użytkownika do edycji tablicy spowoduje wyświetlenie poniższej notyfikacji i konieczność złożenia prośby. Po złożeniu prośby, zapraszana osoba zostanie dodana do tablicy z uprawnieniami do komentowania, co umożliwi jej dodawanie komentarzy na tablicy, ale bez możliwości edycji jej treści.

## Ustawienia zaproszeń do firmy

Ustawienia zaproszeń firmy kontrolują, kto może zapraszać nowych Członków do Twojej subskrypcji Enterprise. Wszyscy nowi Członkowie otrzymują licencję Advanced, Standard, Full (legacy), Free, Free Restricted w zależności od [modelu licencjonowania](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md) i [domyślnej licencji](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

### Jak skonfigurować ustawienia zaproszeń firmy

> **Dostępne dla**: [program elastycznych licencji (FLP)](../enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md)

Aby zarządzać ustawieniami zaproszeń firmy, przejdź do **Ustawienia firmy** > **Bezpieczeństwo** > **Udostępnianie** > **Zaproszenie** i wybierz jedną z poniższych opcji:

**Tylko administratorzy firmy**
Jedynie administratorzy firmy mogą przyznawać licencje nowym członkom. Administratorzy zespołów i członkowie mogą tylko zapraszać istniejących członków firmy do swoich zespołów i nie mogą aktywować nowych licencji.

**Administratorzy firmy i administratorzy zespołów**
Administratorzy firmy i administratorzy zespołów mogą zapraszać nowych członków i dodawać nowe licencje. Administratorzy zespołów mogą zapraszać nowych członków tylko do zespołów, w których są administratorami.

**Wszyscy członkowie**
Każdy członek subskrypcji Enterprise może dodawać nowe licencje, zapraszając osoby do swojego zespołu, o ile zaproszenia są dozwolone dla **wszystkich członków zespołu** w ustawieniach zaproszeń zespołu.

## Jak działają ustawienia Firmy i Zespołu razem

Ustawienia firmy uzupełniają ustawienia zaproszeń zespołu. Administratorzy firmy mogą konfigurować, kto może zapraszać użytkowników do konkretnego zespołu w ustawieniach zespołu. Oznacza to, że administratorzy firmy mogą pozwolić członkom zespołu i administratorom zespołów na zarządzanie własnymi zaproszeniami i współpracą w zespole, ale licencje nadal są kontrolowane przez administratorów firmy w ustawieniach firmy.

## Automatyczna dezaktywacja Gości

Skonfiguruj automatyczną dezaktywację gości po 30 dniach braku aktywności. Użyj tej funkcji, aby usunąć gości i zwiększyć bezpieczeństwo swojej subskrypcji.

Po włączeniu funkcji, wszyscy goście (niezależnie od ich domeny), którzy nie byli aktywni w zespołach Enterprise przez 30 dni, zostaną automatycznie dezaktywowany. Nie ma możliwości dostosowania okresu 30 dni.

To ustawienie dotyczy wszystkich zespołów w ramach organizacji.

Przejdź do **Ustawień firmy** > **Bezpieczeństwo** > **Udostępnianie** i włącz **Automatyczne dezaktywowanie gości**.

:::tip
Gdy tylko ustawienie zostanie włączone, działanie zostanie zapisane w [dziennikach audytu](../security-integrations/security-management/01-audit-logs.md) jako **Włączone/wyłączone ustawienie wygaśnięcia użytkowników zewnętrznych**. Zdarzenia dezaktywacji będą również logowane w [dziennikach audytu](../security-integrations/security-management/01-audit-logs.md). Użytkownik zostanie wyświetlony jako **Miro Automation**.
:::
