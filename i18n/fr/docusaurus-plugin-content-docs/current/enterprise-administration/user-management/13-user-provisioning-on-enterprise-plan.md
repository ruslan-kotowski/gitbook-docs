---
title: "Provisionnement d\u2019utilisateurs sur un forfait Enterprise"
article_id: 4403139914130
translation_id: 4403139914130
locale: fr
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

Avec le provisionnement automatique, tous les nouveaux utilisateurs dans vos domaines d'entreprise sont dirigés vers votre abonnement Enterprise et accèdent aux ressources de votre entreprise.

Miro Enterprise fournit plusieurs options de provisionnement : invitations, provisionnement Juste-à-temps (JIT), gestion des identités inter-domaines (SCIM) et contrôle de domaine.

> **Disponible pour :** forfait Enterprise

## Invitations

Vous pouvez inviter des utilisateurs dans votre abonnement en utilisant le bouton **Inviter des membres** sur votre tableau de bord. Les invitations sont envoyées immédiatement et ne nécessitent aucune configuration supplémentaire.

Pour en savoir plus sur la façon dont vous pouvez partager votre travail et collaborer dans Miro, consultez [Gérer les invitations sur le forfait Enterprise](05-manage-user-invitations-on-enterprise-plan.md) et [Partager des tableaux et inviter des collaborateurs](../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md).

![invite_members_button.jpg](../../../../../../docs/enterprise-administration/user-management/images/21017653284754_invite%20members%20button.jpg)*L'option pour inviter des membres sur le tableau de bord Miro*

## Provisionnement Juste-à-temps (JIT)

Le provisionnement JIT, intégré à [l'authentification unique (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), ajoute automatiquement tous les nouveaux utilisateurs enregistrés sous vos domaines SSO d'entreprise à une équipe spécifique dans votre forfait Enterprise.
Le provisionnement JIT peut être facilement activé dans vos paramètres SSO de Miro. Apprenez [comment configurer le SSO](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md).

![user_provisioning_jit_provisioning.png](../../../../../../docs/enterprise-administration/user-management/images/21017682931730_user_provisioning_jit_provisioning.png)*Activation du provisionnement Just-in-Time (JIT) dans les paramètres SSO*

## Système de gestion des identités inter-domaines (SCIM)

Le SCIM, intégré avec [l’authentification unique (SSO)](../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), vous permet de provisionner et de gérer automatiquement les utilisateurs de votre forfait Enterprise grâce à votre fournisseur d’identité préféré.

Avec le SCIM activé, vous pouvez ajouter des utilisateurs à des équipes spécifiques, mettre à jour leurs infos et e-mails, et gérer leur état d’activation directement depuis votre fournisseur d’identité choisi. Cette fonctionnalité automatise l’échange des informations des utilisateurs entre votre compte Miro et votre fournisseur d’identité.

Le SCIM automatise l’échange d’informations sur les utilisateurs entre Miro et votre fournisseur d’identité, vous permettant de gérer l’accès des employés à votre forfait Enterprise de manière centralisée depuis le fournisseur d’identité.

En savoir plus sur les [fonctionnalités SCIM](../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) et consultez les étapes de configuration pour [Entra ID](../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md), [OKTA](../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md) ou [OneLogin](../security-integrations/system-for-cross-domain-identity-management-scim/06-setting-up-automated-provisioning-with-onelogin.md).

## Contrôle de domaine

[Contrôle de domaine](../canvas-25-admin-features/domain-control/01-domain-control.md) vous permet d’ajouter automatiquement de nouveaux utilisateurs à votre abonnement Enterprise, de limiter la capacité des utilisateurs de votre entreprise à créer des abonnements Miro séparés et de surveiller l’activité des utilisateurs au sein de votre domaine.

Grâce au contrôle de domaine, vous pouvez définir une règle de provisionnement pour vos utilisateurs d'entreprise :

- Les utilisateurs nouvellement enregistrés dans votre domaine peuvent demander l’accès à votre abonnement
- Les utilisateurs nouvellement enregistrés dans votre domaine rejoignent automatiquement votre abonnement
- Les utilisateurs nouvellement enregistrés dans votre domaine rejoignent automatiquement votre abonnement et les utilisateurs de votre domaine ne sont pas autorisés à créer de nouvelles équipes Miro

![Add-a-domain-Image1.png](../../../../../../docs/enterprise-administration/user-management/images/21017653288082_Add-a-domain-Image1.png)*Contrôle de domaine dans les paramètres de sécurité de Miro*

## Comment fonctionne l’attribution de licences

Lorsqu’ils invitent de nouveaux utilisateurs, les admins d’entreprise peuvent choisir une licence à attribuer à la personne invitée en fonction de la configuration de l’abonnement.

Les utilisateurs invités par des utilisateurs autres que les admins ou automatiquement ajoutés à votre abonnement par JIT, SCIM ou contrôle de domaine, se verront attribuer la *licence par défaut* :

- **Pour les forfaits avec des licences non flexibles (non-FLP) :** la licence par défaut est une licence complète (si l'organisation ne dispose pas de suffisamment de licences complètes, les utilisateurs ajoutés automatiquement obtiendront une [licence gratuite restreinte](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md)).
- **Pour les forfaits avec le programme de licences flexibles (FLP) :** la licence par défaut peut être Free ou [gratuite restreinte](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).

:::note
En savoir plus sur nos [modèles de licence Enterprise](../enterprise-subscription-management/enterprise-licensing/02-enterprise-licensing.md), [la gestion des licences dans le programme de licences flexibles](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md), comment gérer l'attribution des licences et changer de forfait avec [la gestion des demandes](09-request-management-on-enterprise-plan.md), et comment suivre l'utilisation des licences avec la [gestion des actifs logiciels](../security-integrations/software-asset-management/01-software-asset-management-miro-enterprise.md).
:::

## Foire aux questions

Lorsque le contrôle de domaine est configuré pour capturer de nouveaux utilisateurs, fonctionne-t-il de manière similaire à JIT en assignant automatiquement des utilisateurs avec des domaines spécifiques à une équipe par défaut au sein de l’abonnement Enterprise ?

Oui, mais le contrôle de domaine ne nécessite pas de configurer l’authentification unique pour le forfait Enterprise. Il peut fonctionner sans l’authentification unique.

Pouvons-nous empêcher les utilisateurs auto-provisionnés de recevoir une licence complète tant qu'ils n'ont pas commencé à travailler activement sur un tableau ?

Oui, c'est possible avec le [programme de licences flexibles](../enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).

Puis-je configurer plusieurs options de provisionnement pour mon abonnement Enterprise ?

Oui, vous pouvez utiliser plusieurs options de provisionnement en même temps.
