---
title: Modifier la politique de suppression
article_id: 19551033354002
translation_id: 19551033354002
locale: fr
sidebar_position: 18
created_at: '2024-06-14T19:50:51Z'
updated_at: '2025-12-08T16:14:46Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Pour modifier les politiques de suppression, vous devez avoir le rôle [d’admin de gouvernance des données](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin de gouvernance des données, contactez l’admin de votre entreprise.
:::

Pour modifier une politique de suppression, effectuez les étapes suivantes :

1. Allez dans vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **Cycle de vie du contenu**.
3. Cliquez sur l'onglet **Suppression**.
   La **page Politiques de suppression** s’affiche.
4. Sur la **page Politiques de suppression**, cliquez sur la politique de suppression que vous souhaitez modifier.
   La page affichant les informations relatives à la politique s’affiche.
5. Cliquez sur **Modifier** en haut à droite de la page, puis modifiez les champs requis. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Nom**  **(obligatoire)** | Nom de la politique de suppression.  Longueur maximale : 60 caractères. |
   | **Description**  **(optionnel)** | Description de cette politique de suppression.  Longueur maximale : 300 caractères. |
   | **Période de suppression**  **(obligatoire)** | Indiquez quand les tableaux sont automatiquement mis à la corbeille. Choisissez un nombre, sélectionnez **Mois** ou **Années**, puis choisissez si la période est calculée à partir de la date de **dernière modification** du tableau ou de **dernier accès**.  Si vous spécifiez la période de suppression en mois, vous devez sélectionner une période de suppression comprise entre 1 et 120 mois.  Si vous spécifiez la période de suppression en années, vous devez sélectionner une période de suppression comprise entre 1 et 10 ans.  Par exemple, si vous souhaitez que les tableaux soient déplacés dans la corbeille lorsqu'ils n'ont pas été modifiés pendant un an, vous pouvez sélectionner 1 an et choisir **Dernière modification**. |
   | **Champ d’application**  **(obligatoire)** | Sélectionnez le champ d’application de cette politique de suppression. Le champ d’application indique les tableaux pour lesquels cette politique de suppression est applicable. Vous pouvez définir le champ d’application d’une politique de suppression pour tous les tableaux d’une organisation ou pour des niveaux spécifiques de classification des tableaux.  **Définir la politique de suppression pour tous les tableaux de l’organisation** Si vous souhaitez définir la portée de la politique de suppression pour tous les tableaux de l’organisation, dans la liste **Portée**, sélectionnez **Tous les tableaux de l’organisation**.  **Définir la politique de suppression pour une ou plusieurs équipes dans l'organisation** Si vous souhaitez définir le périmètre de la politique de suppression pour une ou plusieurs équipes dans l'organisation, procédez comme suit :  1. Dans la liste **Portée**, sélectionnez **Équipe**. 2. Cliquez sur la case **Entrer l'équipe** et sélectionnez chaque équipe pour laquelle vous souhaitez appliquer la politique de suppression. Une coche apparaît à côté de l'équipe que vous avez sélectionnée pour associer à la politique de suppression.   ✏️ - Vous pouvez sélectionner plusieurs équipes pour une politique de suppression. Cependant, une équipe donnée ne peut être associée qu'à une seule politique de suppression à la fois.  - Vous pouvez sélectionner n'importe quelle équipe, y compris les équipes supprimées, comme périmètre lors de la définition de la politique de suppression.   - Une équipe sélectionnée comme périmètre pour une politique de suppression ne peut pas être supprimée définitivement tant qu'elle n'est pas retirée du périmètre.  **Définir la politique de suppression pour un niveau de classification de tableau**  ✏️ Pour définir la portée de la politique de suppression à un niveau spécifique de classification des tableaux, vous devez vous assurer que la fonction de classification des données est activée. Une fois qu’une politique de suppression utilise un niveau de classification des tableaux, vous ne pouvez pas désactiver la fonction de classification des données. Pour plus d’informations, consultez la documentation sur la [Classification des données](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Si vous souhaitez définir la portée de la politique de suppression pour un niveau spécifique de classification de tableau, procédez comme suit :  1. Dans la liste des **Scopes**, sélectionnez **Classification**. 2. Cliquez sur la liste à côté de la liste **Classification**, puis sélectionnez les niveaux de classification pour lesquels vous souhaitez appliquer la politique de suppression. Vous pouvez également rechercher les niveaux de classification, puis les sélectionner.  Une coche apparaît en regard des niveaux de classification que vous avez choisis d’associer à la politique de suppression.  ✏️ **Notes:** - Vous pouvez sélectionner plusieurs niveaux de classification à la fois. - Vous ne pouvez pas définir le même niveau de classification pour différentes politiques de suppression. Si un niveau de classification spécifique est déjà associé à une politique de suppression, le niveau de classification apparaît en grisé.  - Une fois qu’une politique de suppression utilise un niveau de classification de tableau, vous ne pouvez pas désactiver la fonctionnalité de Classification des données.  - Une fois qu'un niveau de classification est associé à une politique de suppression, vous ne pouvez pas supprimer ce niveau de classification spécifique. - Lorsqu’un tableau est régi par les politiques de suppression du périmètre de tous les tableaux de l’organisation et du périmètre de classification, c’est la politique dont la période de suppression est la plus longue qui s’applique. |
6. Cliquez sur **Suivant**.
   La page **Examen de l'impact** apparaît.
7. Examinez l’impact de la politique de suppression. La page d’impact de l’examen fournit les informations suivantes :
   - **Résumé :** configuration de la politique de suppression, telle que le nom de la politique, la période de suppression et le champ d’application.
   - **Impact de la politique :** nombre de tableaux qui seront régis par cette politique.
8. Pour enregistrer la configuration et appliquer la politique de suppression, cliquez sur **Publier**.
   Si vous n’avez pas activé les notifications de suppression, la boîte de dialogue **Activer les notifications de suppression** apparaît.
9. **Notifications de suppression** permettent aux utilisateurs de recevoir des alertes anticipées avant qu'un tableau ne soit automatiquement déplacé vers la Corbeille en raison de son inactivité. Ces alertes aident les utilisateurs à agir s'ils souhaitent conserver leur contenu.

   Si vous souhaitez activer les notifications de suppression :

   a. Cliquez sur **Notifier**.

   b. Configurez le nombre de jours d'avance pour l'envoi de la notification — une valeur entre **1 et 30 jours**.

   Si l’activation des notifications entraîne le **déplacement immédiat de certains tableaux vers la corbeille** (car ils ont déjà dépassé le seuil), il vous sera demandé si vous souhaitez informer les utilisateurs à propos de ces tableaux. Vous pouvez choisir :

   - **Oui** – pour informer les propriétaires et copropriétaires du tableau même si celui-ci est déplacé immédiatement vers la corbeille.

   - **Non** – pour déplacer les tableaux sans envoyer de notification pour cette action immédiate.

   Une fois activées, les utilisateurs ayant des tableaux sous le coup d'une politique de suppression avec notifications activées :

   - Recevront une notification dans leur **fil d’actualité** Miro pendant la fenêtre d’inspection configurée.

   - Pourront ouvrir le tableau directement depuis la notification.

   - Voir une **bannière** sur le tableau avertissant de la suppression automatique imminente, avec une option pour **garder le tableau** s’ils souhaitent le conserver.

:::note
La création, la mise à jour ou la suppression d’une politique déclenche le processus de suppression des politiques, qui peut prendre jusqu’à 24 heures. Cependant, la mise à jour du nom ou de la description d’une politique se fait immédiatement car ces actions ne déclenchent pas le processus de suppression des politiques.
:::

#
