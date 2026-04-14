---
title: "Usu\u0144 zasad\u0119 retencji"
article_id: 19205219887762
translation_id: 19205219887762
locale: pl-pl
sidebar_position: 12
created_at: '2024-05-28T18:02:52Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

Usunięcie zasady retencji powoduje zwolnienie tablic powiązanych z tą zasadą retencji. Te tablice mogą teraz zostać trwale usunięte bez ograniczeń.

:::note
Aby usunąć zasady retencji, musisz mieć [Data Governance Admin role](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Aby zażądać roli administratora zarządzania danymi, skontaktuj się z administratorem firmy.
:::

Aby usunąć zasadę retencji, wykonaj następujące kroki:

1. Przejdź do [ustawień Miro](https://miro.com/app/settings).
2. W panelu po lewej stronie, pod **Enterprise Guard,** kliknij **Cykl życia treści**.
3. Kliknij kartę **Retencja**.
4. Na stronie **zasady** **retencji** kliknij zasadę retencji, którą chcesz usunąć.
   Strona wyświetlająca informacje związane z zasadą pojawia się.
5. Kliknij **Usuń** w prawym górnym rogu strony.
6. Przeanalizuj wpływ usunięcia zasady retencji. Strona oceny wpływu dostarcza następujące informacje:
   - **Podsumowanie:** konfiguracja zasady retencji, taka jak nazwa zasady, okres retencji i zakres.
   - **Wpływ zasad:** liczba tablic, które zostaną zwolnione z retencji i będzie można je trwale usunąć bez żadnych ograniczeń. Zasada retencji ma również zastosowanie do tablic w koszu i są one uwzględniane w obliczeniach wpływu przeglądu.
7. Aby usunąć zasadę retencji, kliknij **Usuń zasadę**.

:::note
Utworzenie, aktualizacja lub usunięcie zasady uruchamia proces zasad retencji, który może potrwać do 24 godzin. Jednak aktualizacja nazwy lub opisu zasady następuje natychmiast, ponieważ te działania nie uruchamiają procesu zasad retencji.
:::
