---
title: Politique de partage sur le plan d’Entreprise
article_id: 360017730133
translation_id: 360017730133
locale: fr
sidebar_position: 7
created_at: '2019-02-11T10:09:02Z'
updated_at: '2025-11-25T16:00:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible pour: Forfait Enterprise Rôle requis: Admin d’entreprise'
---

La sécurité et la confidentialité des données sont des préoccupations importantes pour la plupart des entreprises. C’est pourquoi notre forfait Enterprise fournit des outils renforcés pour contrôler les risques de sécurité de l’information. Ceux-ci permettent notamment une gestion des accès plus sûre avec une option d'authentification unique (SSO) basée sur SAML et un meilleur contrôle des droits et autorisations des utilisateurs avec des capacités d'administration améliorées. De plus, nous introduisons des restrictions facultatives : partage en dehors des domaines autorisés et partage via un lien public.

:::note
Les paramètres de politique de partage influencent également les paramètres d'accès disponibles lors de l'intégration de tableaux dans une application spécifique. En savoir plus : [Gérer la politique de partage pour les intégrations embarquées sur un compte Enterprise](../../managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).
:::

## Restreindre le partage en dehors des domaines autorisés

Au niveau de l’entreprise Au niveau de l’équipe

Une fois que vous avez défini les domaines autorisés au niveau de l’entreprise, l’option de partager des tableaux en dehors des domaines sera restreinte pour tous les membres et équipes de l’entreprise.

1. Allez dans les paramètres de **l’entreprise** > **Sécurité** > **Partage**.
2. Activez l’option **Restreindre les domaines autorisés**.
3. Ajoutez la liste des domaines de confiance utilisés dans votre forfait Enterprise.

Pour activer le partage avec [des collaborateurs invités](../../../using-miro/sharing-boards/07-collaboration-with-guests.md) et contourner la liste des domaines autorisés, cochez la case **Autoriser le partage avec des invités en dehors de ces domaines**.

Lorsque l’option **Autoriser le partage avec des invités en dehors de ces domaines** est activée, les utilisateurs dont les domaines ne figurent pas sur la liste autorisée peuvent avoir des tableaux partagés avec eux, mais ils ne pourront toujours pas trouver les équipes sous [la découvrabilité d'équipe.](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md)

![sharing-allowed-domains.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956412562_sharing-allowed-domains.png)
*La liste des domaines de confiance et l'option pour le partage avec des invités en dehors de ces domaines*

Tout utilisateur qui avait été invité sur l’abonnement avant l’activation du paramètre est autorisé à rester dans votre forfait et à conserver l’accès au contenu partagé. Cependant, il ne sera pas possible de partager d'autres contenus avec eux.

De plus, vous pouvez **vérifier tous les utilisateurs par rapport à la liste des autorisations** au cas où il y en aurait dont le domaine n’est pas autorisé. Vous pouvez les supprimer dans la fenêtre pop-up suivante :

![validate_against_the_allowlist.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017004911250_validate%20against%20the%20allowlist.jpg)*Utilisateurs dont les adresses e-mail ne correspondent pas à la liste des domaines autorisés*

En restreignant l'accès au niveau de l'équipe, les utilisateurs en dehors des domaines autorisés ne pourront pas accéder ou être invités dans l'équipe ou aux tableaux qu'elle contient. L’option vous permet d’activer les paramètres pour une équipe spécifique sans restreindre les règles de partage pour tous les utilisateurs Enterprise. Cela vous offre également l’option d’autoriser un domaine particulier pour une équipe sans qu’il soit nécessaire de l’autoriser pour l’ensemble de l’entreprise.

:::note
Si les domaines autorisés ne sont pas configurés au niveau de l’équipe, les paramètres de l’entreprise sont effectifs. Si la liste d’autorisation au niveau de l’équipe est configurée, cela remplace les restrictions au niveau de l’entreprise. Par exemple, si **le Domaine 1** est autorisé au niveau de l’entreprise et **le Domaine 2**  est autorisé au niveau de l’équipe, **le Domaine 1**  ne sera pas autorisé au niveau de l’équipe sauf s'il est ajouté à la liste d’autorisations au niveau de l’équipe.
:::

Pour configurer les domaines autorisés pour une équipe spécifique :

1. Allez dans **Équipes** et sélectionnez l’équipe que vous souhaitez configurer.
2. Allez dans **Paramètres** et faites défiler jusqu’à **Domaines autorisés pour l’équipe**.
3. Activez l’option **Restreindre les domaines autorisés**.
4. Saisissez vos domaines autorisés et cliquez sur **Ajouter**.
   Pour autoriser le partage avec des invités en dehors des domaines, cochez la case **Activer le partage avec des invités en dehors des domaines autorisés**.

![sharing-team-allowed-domains.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921804702226_sharing-team-allowed-domains.png)
*L’option de restreindre les domaines autorisés pour une équipe particulière avec un abonnement Enterprise*

Une fois que vous avez restreint le partage en dehors des domaines autorisés, les utilisateurs de l’entreprise pourront partager leurs tableaux uniquement avec les utilisateurs des domaines spécifiés. Lorsque le paramètre est activé, si un utilisateur de l’entreprise essaie de partager son tableau avec un domaine non autorisé, il reçoit le message suivant :

![can_t_share_outside_the_allowlist.jpg](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956416146_can%27t%20share%20outside%20the%20allowlist.jpg)*Le tableau ne peut pas être partagé avec un utilisateur dont le domaine n’est pas dans la liste de domaines autorisés*

:::note
Si le partage via un lien public est autorisé dans votre entreprise, [les tableaux publics](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#partage-de-tableaux-via-un-lien-public) restent accessibles à *toute personne disposant du lien du tableau* (et du mot de passe s’il est configuré).
:::

## Restreindre le partage via un lien public

Les admins d’entreprise peuvent empêcher tous les utilisateurs de l’entreprise ou les membres d’une équipe en particulier de [partager publiquement les tableaux de l’entreprise](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#partage-de-tableaux-via-un-lien-public). Une fois le paramètre désactivé, l’option **Toute personne disposant du lien** disparaît du menu Partager des tableaux de l’entreprise ou de l’équipe.

Au niveau de l’entreprise Au niveau de l’équipe

Pour empêcher le partage public pour tous les utilisateurs de l’entreprise :

1. Allez dans **Entreprise** **Paramètres >** **Sécurité > Partage**.
2. Désactivez **Les tableaux peuvent être partagés publiquement**.

En procédant ainsi, vous supprimerez l’option « Toute personne ayant le lien » du menu Partager du tableau. Cela signifie également que tous les tableaux partagés jusqu'à présent via un lien public ou intégrés à des sites deviendront indisponibles pour les utilisateurs publics et que leurs sessions actives sur les tableaux seront fermées.

Si les admins activent à nouveau la possibilité de partager publiquement des tableaux, les utilisateurs devront réactiver manuellement le partage public pour chaque tableau.

Si vous souhaitez autoriser les modifications sur les tableaux partagés publiquement, cochez l’option **Autoriser les modifications sur les tableaux partagés publiquement***.* Si vous *décochez la case,* l’accès public à tous les tableaux précédemment partagés pour l’édition publique sera restreint.

:::note
Le partage via un lien public est activé par défaut au niveau de l’équipe et défini sur "Tout le monde peut voir et commenter" pour les équipes nouvellement créées. Cependant, si cette option est **désactivée** au niveau de l’entreprise, les équipes ne peuvent pas partager les tableaux publiquement, même si cela est autorisé au niveau de l’équipe.
:::

Pour restreindre le partage public des tableaux pour une équipe donnée :

1. Allez dans **Équipes** et sélectionnez l’équipe que vous souhaitez configurer.
2. Allez dans **Paramètres** et faites défiler jusqu'à **Paramètres de partage**.
3. Sous **Partage de tableau** > **Via un lien public**, vous verrez trois options : vous pouvez choisir d’autoriser le partage public pour la consultation et l’ajout de commentaires uniquement, pour la consultation, les commentaires et la modification, ou de restreindre le partage public pour l’équipe.

![sharing-public-link.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978809746_sharing-public-link.png)
*L’option de configurer le partage via un lien public pour une équipe dans un abonnement Enterprise*

**Expiration du lien public (au niveau de l’entreprise)**

Pour accroître la sécurité des tableaux partagés publiquement, activez l’expiration du lien public. Cela signifie que les liens vers le tableau partagés avec les visiteurs cesseront de fonctionner après un certain temps si le tableau n’a pas été ouvert. Cette fonction s’applique à tous les tableaux une fois l’expiration du lien public activée dans les paramètres de l’entreprise.

Pour activer l’expiration du lien public :

1. Allez dans **Paramètres de l’entreprise > Sécurité > Partage**.
2. Faites défiler jusqu’à la section **Contenu**.
3. Cochez la case pour **Expiration du lien de partage public**.
4. Définissez le nombre de jours avant l’expiration des liens inactifs. Vous pouvez choisir entre 30 et 999 jours.

:::warning
Si le mot de passe d'un tableau est réinitialisé, la date d'expiration du tableau sera également réinitialisée pour ce tableau.
:::

## Exiger des mots de passe pour les tableaux publics (au niveau de l’entreprise)

Vous pouvez également rendre obligatoire l’utilisation de mots de passe pour tous les tableaux partagés publiquement par un lien.

1. Allez dans **Paramètres de l’entreprise > Sécurité > Partage**.
2. Faites défiler jusqu'à la section **Contenu**.
3. Cochez la case **Exiger un mot de passe pour les tableaux partagés publiquement**.

Une fois cette fonctionnalité cochée, elle s'appliquera immédiatement aux tableaux précédemment accessibles avec un lien public et tous les tableaux à venir ne pourront plus être accessibles publiquement sans mot de passe.

- *Pour les tableaux précédemment accessibles par* [*lien public*](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md#partage-de-tableaux-via-un-lien-public) *sans mots de passe :*
  Si les tableaux étaient jusque-là accessibles par un lien public sans mots de passe, les sessions ouvertes seront révoquées et les visiteurs seront invités à entrer un mot de passe s’ils essaient d’accéder à un lien accessible auparavant.
- *Pour tous les tableaux :*
  Pour rendre un tableau accessible publiquement par un lien, un mot de passe doit être défini par le propriétaire du tableau ou l’[admin du contenu](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md). Si un mot de passe est supprimé, l’option **Toute personne disposant du lien** dans le menu Partager du tableau passera automatiquement au statut **Aucun accès**. Les membres de l’équipe disposant de droits de modification peuvent partager un tableau via un lien public si le mot de passe a déjà été défini, sinon, ils doivent contacter le propriétaire du tableau pour définir un mot de passe.
- Lorsque l'option « *Expiration du lien lorsque le tableau a été inactif pendant 'x' jours* » est activée, une icône d’horloge apparaîtra dans la boîte de dialogue Partager, avec un message indiquant que l'accès public disparaîtra après le nombre de jours spécifié.
  ![1-2.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978811282_1-2.png)
*Option de partage public sur le forfait Enterprise avec mots de passe obligatoires*

Vous pouvez également exiger que les mots de passe soient complexes et spécifier les critères que les mots de passe doivent respecter. Ceux-ci peuvent inclure :

- Longueur minimale du mot de passe (de 6 à 14 caractères ; par défaut, 8).
- Lettres majuscules et minuscules.
- Chiffres.
- Caractères spéciaux.

![complex-board-password.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956422418_complex-board-password.png)
*Paramètres pour les mots de passe complexes des tableaux*

## Restreindre le partage à l’échelle de l’équipe et de l’entreprise (au niveau de l’équipe)

:::note
Le partage à l’échelle de l’équipe et de l’entreprise est activé par défaut si les paramètres n’ont pas été personnalisés par l’admin d’entreprise.
:::

Les admins d’entreprise Enterprise peuvent également activer/désactiver le partage à l’échelle de l’entreprise ou de l’équipe.

1. Allez dans **Équipes** et sélectionnez l’équipe que vous souhaitez configurer.
2. Allez dans **Paramètres** et faites défiler jusqu’à **Paramètres de partage**.
3. Dans **Partage de tableau**, choisissez si le partage avec une équipe est autorisé ou non. Pour les paramètres à l’échelle de l’entreprise, choisissez si l’entreprise peut consulter et commenter les tableaux partagés, consulter/commenter/modifier ou si le partage n’est pas autorisé.![sharing-board-sharing.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921804722706_sharing-board-sharing.png)*Paramètres de partage du tableau sur le forfait Enterprise*

L’activation du partage de tableaux avec une équipe permet aux membres de l’équipe de partager facilement leurs tableaux et leurs projets avec toute l’équipe.

Désactiver cette option entraînera sa suppression du menu Partager des tableaux et projets d'équipe. Les tableaux et les projets partagés précédemment ne seront plus disponibles pour les utilisateurs de l’équipe, sauf s’ils sont partagés par d’autres moyens.

Si l’admin réactive la possibilité de partager avec l’équipe, les tableaux et projets partagés auparavant ne seront pas automatiquement partagés avec l’équipe et les utilisateurs devront les partager à nouveau manuellement.

![1-3.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978812178_1-3.png)
*L’option de partager un tableau avec l’équipe peut être masquée dans le menu Partager*

Les utilisateurs sur les forfaits Enterprise dont la [confidentialité de l’équipe](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) est désactivée peuvent également [partager leurs tableaux avec l’ensemble de l’entreprise pour consultation, ajout de commentaires ou modification en un seul clic](../../../using-miro/sharing-boards/03-sharing-boards-and-inviting-collaborators.md). Vous pouvez verrouiller cette option pour une équipe particulière en sélectionnant **Non autorisé** sous le paramètre **Avec toute l’entreprise**. Ou vous pouvez autoriser le partage pour la consultation et les commentaires uniquement, ou également pour la modification.

Veuillez noter que si la [confidentialité de l’équipe](../../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md) est activée dans votre entreprise, l’option de partage des tableaux avec l’ensemble de l’entreprise ne sera pas disponible, même si le partage est autorisé au niveau de l’équipe.

![1-4.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956423442_1-4.png)
*L’option de partager un tableau avec toute l’entreprise peut être masquée dans le menu Partager*

## Restreindre la possibilité de déplacer des tableaux vers d’autres équipes (au niveau de l’équipe)

:::note
La possibilité de déplacer des tableaux vers d’autres équipes est activée par défaut si le paramètre n’a pas été personnalisé par l’admin d’entreprise.
:::

Lorsqu’un admin d’entreprise interdit le déplacement des tableaux pour une équipe, ses membres ne pourront pas déplacer les tableaux vers d’autres équipes ou en dehors de leur équipe. Le paramètre est configuré pour chaque équipe dans **Team settings > Permissions**.

:::note
️ Les utilisateurs qui ne sont pas des admins ne peuvent pas déplacer des tableaux vers une équipe si l’[option de création de tableaux leur est interdite](../../managing-enterprise-teams-and-content/10-team-permissions-on-enterprise-plan.md) dans l’équipe cible.
:::

![sharing-moving-boards.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584956424082_sharing-moving-boards.png)
*L’option de restreindre le déplacement des tableaux dans et hors de l’équipe*

## Restreindre le partage de modèles personnalisés à l’échelle de l’entreprise

> **Disponible pour :** Forfait Enterprise
> **Qui peut le faire :** Admins d’entreprise

Les admins d’entreprise peuvent autoriser ou restreindre le partage de modèles personnalisés au niveau de l’entreprise. Lorsque le partage est restreint, les membres de l’équipe ne pourront pas partager un modèle personnalisé avec l’entreprise sans l’approbation de l’admin.

1. Allez dans **Paramètres de l'entreprise** > **Sécurité** > **Paramètres**.
2. Faites défiler jusqu’à **Rôles et autorisations**.
3. Activez l’option **Restreindre le partage des modèles de l’entreprise**.

![sharing-restrict-templates.png](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/22584978813202_sharing-restrict-templates.png)
*L’option de restriction du partage de modèles avec l’entreprise*

## Foire aux questions

Les membres reçoivent-ils des notifications lorsque les admins d’entreprise modifient les paramètres de partage mentionnés ci-dessus au niveau de l’équipe ou de l’entreprise ?

Non, il n’y a aucune notification dans de tels cas. Les règles s’appliquent immédiatement.

Avons-nous un tableau de bord où nous pouvons suivre tous les tableaux partagés avec un lien public ?

Il n’existe actuellement aucun tableau de bord de ce type.

J’ai désactivé l’option de restriction des domaines autorisés, mais nous ne pouvons toujours pas partager de tableaux avec des utilisateurs en dehors des domaines autorisés. Comment puis-je résoudre ce problème ?

Il est possible que le paramètre soit toujours activé au niveau de l’entreprise/de l’équipe. Veuillez vérifier si la restriction est désactivée dans les paramètres de l'entreprise ou dans les paramètres de l'équipe.
