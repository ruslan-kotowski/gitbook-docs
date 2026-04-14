---
title: Gestion de la confidentialité et de la découverte des équipes dans le plan
  Enterprise
article_id: 360011821219
translation_id: 360011821219
locale: fr
sidebar_position: 12
created_at: '2020-02-07T12:46:14Z'
updated_at: '2025-12-10T12:23:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: sharing-settings
availability:
  notes: 'Disponible pour: Forfait Enterprise Rôle requis: Admin d’entreprise'
---

Travailler au sein d’une grande organisation va souvent de pair avec un contenu et des utilisateurs répartis dans plusieurs équipes. Assurez-vous que tout le personnel a accès à ce dont il a besoin en permettant aux membres de votre abonnement de voir et de rejoindre les équipes pertinentes.

### Découverte de l’équipe

**Découverte de l’équipe** est un paramètre configuré au niveau de l’équipe. Il contrôle la façon dont les membres de l’organisation peuvent trouver l’équipe et la rejoindre.  Pour gérer les paramètres de découverte d'une équipe, accédez aux **paramètres de l'entreprise > Équipes**, puis cliquez sur l'équipe dont vous souhaitez modifier les paramètres. Sélectionnez ensuite l'onglet **Paramètres**.

![liste de gestion des équipes.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921803038994_team-management-list.png) *Liste des équipes dans les paramètres de l'entreprise*

> [⚠️](../../administration/user-management/02-invitation-settings.md)La fonctionnalité Découverte de l’équipe peut être configurée par les admins d’entreprise et les admins d’équipe si ceux-ci sont autorisés à inviter des utilisateurs dans l’équipe (ils recevront également les demandes des utilisateurs qui souhaitent rejoindre l’équipe).

Trois états sont possibles pour la fonctionnalité Découverte de l’équipe :

- **Masquée** : à moins que les membres ne soient invités dans l’équipe, ils ne pourront pas la trouver.
- **Les membres peuvent rejoindre l’équipe après approbation** : l’équipe est visible et les membres peuvent demander à la rejoindre.
- **Ouverte aux membres** : l’équipe est visible et les membres peuvent la rejoindre immédiatement.

Si une équipe a [des restrictions sur la liste d'autorisation des domaines](../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md)seuls les utilisateurs dont les domaines d'e-mail figurent sur la liste d'autorisation de l'équipe pourront découvrir l'équipe et demander à la rejoindre. Ce paramètre garantit que la découvrabilité de l'équipe respecte les restrictions de domaine définies au niveau de l'équipe.

> Activez notre fonctionnalité Découverte de l’équipe ainsi que le [provisionnement Juste-à-temps](../user-management/13-user-provisioning-on-enterprise-plan.md)) et l’équipe par défaut que vous définissez pour les utilisateurs nouvellement enregistrés sera également visible pour les utilisateurs existants.

![team-management-discovery-settings.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780537234_team-management-discovery-settings.png)
*Paramètres de découverte de l'équipe*

La fonctionnalité Découverte de l’équipe n’affecte pas la manière dont les membres voient les autres utilisateurs au sein de votre abonnement.  Ainsi, à moins que les paramètres définis dans la fonctionnalité Confidentialité des équipes ne l’empêchent, les membres peuvent consulter la liste complète des autres membres dans les paramètres./span>

Les membres de votre plan Enterprise pourront trouver des équipes qu'ils peuvent rejoindre en ouvrant le menu Équipes en haut à gauche du tableau de bord et en sélectionnant ![icon-zoom-in.svg](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921803048338_icon-zoom-in.svg) **Rejoindre une équipe**. Une liste d'équipes s'affiche avec l'option **Rejoindre** ou **Demander à rejoindre**, en fonction des paramètres de sécurité de l'équipe concernée.

![gestion-équipe-jonction.png](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780544914_team-management-join.png) *Liste des équipes découvrables*

### Confidentialité des équipes

La fonctionnalité **Confidentialité des équipes** est disponible au niveau de l’entreprise et définit la visibilité des équipes et des utilisateurs. Elle se trouve dans les paramètres de l **'entreprise** > **Sécurité** > **Partage,** dans la section **Confidentialité de l'équipe**.

![team-management-privacy.pngParamètres](../../../../../../docs/enterprise-administration/managing-enterprise-teams-and-content/images/23921780547218_team-management-privacy.png)
*de confidentialité de l'*

- Lorsque la fonctionnalité Confidentialité des équipes est désactivée, les membres de l’abonnement peuvent voir la liste complète des utilisateurs dans les paramètres, ainsi que la liste des équipes pouvant être découvertes.  Il s’agit du réglage par défaut dans les forfaits Enterprise, pour permettre à tous les membres de trouver du contenu pertinent et de collaborer avec les autres utilisateurs afin de favoriser le partage des connaissances, la transparence et la réduction des tâches similaires./span>
- Lorsque la fonctionnalité Confidentialité des équipes est activée, les membres de l’abonnement peuvent uniquement voir les équipes auxquelles ils ont été invités et la liste des membres de ces équipes.  Elle peut être activée lorsque des équipes indépendantes travaillent avec des clients différents, afin d’assurer la confidentialité des échanges. Si la fonctionnalité Confidentialité des équipes est activée, il n’est pas possible de partager des tableaux avec l’ensemble de l’entreprise en un clic./span>

### Utilisation conjointe des fonctionnalités Confidentialité des équipes et Découverte de l’équipe

La fonctionnalité Confidentialité des équipes a une priorité supérieure par rapport à la Découverte de l’équipe, qui est configurée au niveau de l’équipe. Une notification vous indiquera que les paramètres de découverte de l’équipe ne sont pas actifs. Vous pouvez tout de même gérer ses options, qui s’activeront une fois que la fonctionnalité Confidentialité des équipes sera désactivée.

> [✏️](../user-management/13-user-provisioning-on-enterprise-plan.md) Les fonctionnalités Confidentialité des équipes et Découverte de l’équipe affectent toutes les deux l’expérience des membres de l’abonnement, mais n’ont aucune incidence sur la façon dont un utilisateur peut rejoindre l’abonnement lui-même.
