---
title: "Przegl\u0105daj tablice z poufnymi informacjami biznesowymi i niestandardowymi\
  \ poufnymi informacjami biznesowymi (wersja beta)"
article_id: 24090123693586
translation_id: 24090123693586
locale: pl-pl
sidebar_position: 13
created_at: '2025-01-21T15:10:56Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: data-discovery
---

Eksplorator treści pozwala [administratorom treści wrażliwych](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) przeglądać przypadki dopasowań poufnych lub niestandardowych poufnych danych biznesowych.

:::note
- Aby przeglądać tablice z dopasowaniami zawierającymi poufne informacje biznesowe lub niestandardowe poufne informacje biznesowe, musisz mieć [rolę administratora treści wrażliwych](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). W celu ubiegania się o rolę administratora treści wrażliwych skontaktuj się z administratorem firmy.
- Dopasowania zawierające poufne informacje biznesowe są oznaczone jako CUSTOMER, TECH lub STRATEGY, a wyniki są wyświetlane na początku listy wyników.

- Dopasowania do danych poufnych biznesowo są oznaczone odpowiednimi niestandardowymi etykietami.
:::

Aby sprawdzić tablicę z danymi poufnymi biznesowo lub niestandardowymi dopasowaniami danych poufnych biznesowo, wykonaj poniższe kroki:

1. Jeśli znajdujesz się na stronie **Eksplorator treści**, przejdź do kroku 2.
   Jeśli nie znajdujesz się na stronie **Eksplorator treści**:
   a. Przejdź do swoich [ustawień Miro](https://miro.com/app/settings).
   b. W lewym panelu, pod **Enterprise Guard**, kliknij **Eksplorator treści**.
   c. Kliknij **Odkrywanie danych**.
2. Na stronie **Content explorer/Wykrywanie danych** kliknij tablicę, którą chcesz przejrzeć.
   Po prawej stronie ekranu pojawia się panel wysuwany.
3. W panelu wysuwanym możesz wykonać następujące czynności:

   - Tylko dla niestandardowych wyników dotyczących poufnych danych biznesowych: **Pokaż lub ukryj** **poufne informacje biznesowe**
   Domyślnie niestandardowe poufne informacje biznesowe są zaczernione. Jeśli chcesz wyświetlić informacje o niestandardowych poufnych danych biznesowych, kliknij przełącznik **Pokaż poufne informacje**, aby go włączyć.
   Kiedy niestandardowe poufne informacje biznesowe są widoczne, możesz je ukryć, klikając przełącznik **Pokaż wrażliwe informacje** , aby go wyłączyć.

   > ✏️ - Dopasowania poufnych informacji biznesowych są oznaczane jako KLIENT, TECH lub STRATEGIA, a wyniki są wymienione na początku listy wyników.
   > - Dopasowania niestandardowych poufnych informacji biznesowych są oznaczane odpowiednimi niestandardowymi etykietami.

   - Zarówno dla dopasowań dotyczących poufnych informacji biznesowych, jak i niestandardowych poufnych informacji biznesowych: **Filtruj informacje według kategorii poufnych informacji biznesowych**
   Aby wyświetlić poufne informacje biznesowe należące do określonej kategorii, kliknij kartę **Poufne informacje biznesowe** , a następnie kliknij odpowiedni przycisk filtru poniżej karty.

   -Tylko dla dopasowań do poufnych informacji biznesowych: **Wyklucz przypadki fałszywych pozytywnych**
   Podczas wykrywania poufnych informacji biznesowych możesz napotkać sytuacje, w których system generuje dopasowania, które, mimo że technicznie poprawne, mogą nie być istotne lub uznawane za dane wrażliwe wg różnych zasad bezpieczeństwa i specyficznych potrzeb organizacji. Wykluczanie dopasowania, które nie stanowi zagrożenia dla bezpieczeństwa czy działalności biznesowej, staje się kluczowe dla dostosowania procesu wykrywania danych do szczególnych wymagań bezpieczeństwa i potrzeb biznesowych organizacji.

   Może się również zdarzyć, że system błędnie oznaczy dane na Twoich tablicach jako prawdopodobnie wrażliwe (fałszywy alarm). Do takich sytuacji mogą przyczyniać się różne czynniki, w tym bliskość powiązanych terminów czy formatowanie danych biznesowych. Możesz również wyciszać niepoprawne zgodności.

   Kiedy wyciszasz zgodność, aktualizacje zachodzą w czasie rzeczywistym. Klasyfikacja tablicy i zastosowane zabezpieczenia są również aktualizowane zgodnie z konfiguracją Autoklasyfikacji i Inteligentnych Zabezpieczeń.

   Aby zablokować fałszywie pozytywny wynik, kliknij wielokropek obok dopasowania poufnych informacji biznesowych, które chcesz ukryć, a następnie wybierz **Ukryj dopasowanie**. Pamiętaj, że aktualizacje odbywają się w czasie rzeczywistym. Klasyfikacja tablicy i zastosowane zabezpieczenia są również aktualizowane zgodnie z konfiguracją Autoklasyfikacji i Inteligentnych Zabezpieczeń.
4. Kliknij następną tablicę, z którą chcesz pracować, na liście wyników Eksploratora Treści i wykonaj niezbędne czynności, lub zamknij panel przesuwany, klikając przycisk **Zamknij** w prawym górnym rogu panelu.
