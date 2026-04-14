---
title: "Obs\u0142uga administracyjna u\u017Cytkownik\xF3w w wersji Enterprise"
article_id: 4403139914130
translation_id: 4403139914130
locale: pl-pl
sidebar_position: 13
created_at: '2021-07-01T07:59:23Z'
updated_at: '2025-11-25T16:05:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: scim
---

Dzięki automatycznemu przypisywaniu, wszyscy nowi użytkownicy wewnątrz Twoich domen firmowych są kierowani do Twojej subskrypcji Enterprise i uzyskują dostęp do zasobów Twojej firmy.

Miro Enterprise oferuje kilka opcji przypisywania użytkowników: zaproszenia, Just-in-Time provisioning (JIT), System for Cross-domain Identity Management (SCIM) i zarządzanie domeną.

> **Dostępne dla:** Wersja Enterprise

## Zaproszenia

Możesz zapraszać użytkowników do swojej subskrypcji za pomocą przycisku **Zapraszaj członków** na swoim pulpicie. Zaproszenia są wysyłane natychmiast i nie wymagają dodatkowej konfiguracji.

Dowiedz się więcej o tym, jak możesz udostępnić swoją pracę i współpracować w Miro, odwiedzając strony [Zarządzanie zaproszeniami w wersji Enterprise](05-manage-user-invitations-on-enterprise-plan.md) oraz [Udostępnianie tablic i zapraszanie współpracowników](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

![invite_members_button.jpg](../../../../../../docs/enterprise-administration/user-management/images/21017653284754_invite%20members%20button.jpg)*Opcja zapraszania członków na pulpicie Miro*

## Obsługa administracyjna JIT (just-in-time)

JIT provisioning, zintegrowane z [SSO (pojedyncze logowanie)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), automatycznie dodaje wszystkich nowych użytkowników zarejestrowanych pod Twoimi domenami SSO do konkretnego zespołu w abonamencie Enterprise.
JIT provisioning można łatwo włączyć w ustawieniach SSO Miro. Dowiedz się, [jak skonfigurować SSO](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

![user_provisioning_jit_provisioning.png](../../../../../../docs/enterprise-administration/user-management/images/21017682931730_user_provisioning_jit_provisioning.png)*Włączanie Just-in-Time (JIT) provisioning w ustawieniach SSO*

## System zarządzania tożsamością międzydomenową (SCIM)

SCIM, zintegrowany z [SSO](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), umożliwia automatyczne tworzenie i zarządzanie użytkownikami w Twoim abonamencie Enterprise za pośrednictwem wybranego dostawcy tożsamości (IdP).

Gdy SCIM jest włączony, możesz dodawać użytkowników do określonych zespołów, aktualizować ich dane i adresy e-mail oraz zarządzać ich statusem aktywacji bezpośrednio w ramach wybranego dostawcy tożsamości. Ta funkcja automatyzuje wymianę informacji o użytkownikach między Twoim kontem Miro a IdP.

SCIM automatyzuje wymianę informacji o użytkownikach między Miro a Twoim IdP, pozwalając na centralne zarządzanie dostępem pracowników do abonamentu Enterprise z poziomu IdP.

Dowiedz się więcej o [funkcjach SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) i zapoznaj się z krokami konfiguracji dla [Entra ID](../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md), [OKTA](../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md) lub [OneLogin](../security-integrations/system-for-cross-domain-identity-management-scim/06-setting-up-automated-provisioning-with-onelogin.md).

## Zarządzanie domeną

[Zarządzanie domeną](../canvas-25-admin-features/domain-control/01-domain-control.md) umożliwia automatyczne dodawanie nowych użytkowników do Twojej subskrypcji Enterprise, ograniczanie możliwości tworzenia przez użytkowników korporacyjnych osobnych subskrypcji Miro oraz monitorowanie aktywności użytkowników w Twojej domenie.

Dzięki zarządzaniu domeną, możesz ustawić regułę udostępniania dla swoich użytkowników korporacyjnych:

- nowo zarejestrowani użytkownicy w twojej domenie mogą poprosić o dostęp do twojej subskrypcji
- nowo zarejestrowani użytkownicy w twojej domenie automatycznie dołączają do twojej subskrypcji
- nowo zarejestrowani użytkownicy w twojej domenie automatycznie dołączają do twojej subskrypcji i użytkownicy w twojej domenie nie mogą tworzyć nowych zespołów Miro

![Add-a-domain-Image1.png](../../../../../../docs/enterprise-administration/user-management/images/21017653288082_Add-a-domain-Image1.png)*Zarządzanie domeną w ustawieniach bezpieczeństwa Miro*

## Jak działa licencjonowanie

Podczas zapraszania nowych użytkowników, administratorzy firmy mogą wybrać licencję dla zaproszonego w zależności od ustawień ich subskrypcji.

Użytkownicy, którzy są zapraszani przez osoby niepełniące funkcji administratora lub którzy są automatycznie dodawani do Twojej subskrypcji przez JIT, SCIM lub zarządzanie domeną, otrzymają *domyślną licencję*:

- **w przypadku abonamentów z nieelastycznymi licencjami (non-FLP):** domyślną licencją jest pełna licencja (jeśli organizacja nie ma wystarczającej liczby pełnych licencji, automatycznie przechwyceni użytkownicy otrzymają [bezpłatną ograniczoną](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) licencję).
- **w przypadku abonamentów z programem elastycznych licencji (FLP):** domyślną licencją może być licencja Free lub [bezpłatna ograniczona](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).

:::note
Dowiedz się więcej o naszych [modelach licencjonowania Enterprise](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md), [zarządzaniu licencjami w programie elastycznych licencji](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md), jak zarządzać przydziałem i zmianami na wyższą wersję za pomocą [zarządzania prośbami](09-request-management-on-enterprise-plan.md), i jak śledzić wykorzystanie licencji z [Zarządzanie aktywami oprogramowania](../security-integrations/software-asset-management/01-software-asset-management-miro-enterprise.md).
:::

## Często zadawane pytania

Czy zarządzanie domeną, gdy jest ustawione na przechwytywanie nowych użytkowników, działa podobnie do JIT, automatycznie przypisując użytkowników z określonymi domenami do domyślnego zespołu w ramach subskrypcji Enterprise?

Tak, ale zarządzanie domeną nie wymaga, aby pojedyncze logowanie (SSO) było skonfigurowane dla wersji Enterprise, może działać bez SSO.

Czy możemy zapobiec przyznaniu automatycznie dodanym użytkownikom pełnej licencji, zanim zaczną aktywnie pracować na tablicy?

Tak, jest to możliwe w ramach [programu elastycznych licencji (FLP)](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

Czy mogę ustawić kilka opcji udostępniania użytkowników dla mojej subskrypcji Enterprise?

Tak, można jednocześnie korzystać z kilku opcji udostępniania użytkowników.
