---
title: Modifier la politique de conservation
article_id: 19205184829330
translation_id: 19205184829330
locale: fr
sidebar_position: 11
created_at: '2024-05-28T18:01:39Z'
updated_at: '2025-12-08T16:07:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Pour modifier les politiques de conservation, vous devez avoir le rôle d’[admin de la gouvernance des données](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander ce rôle, contactez l'admin de votre entreprise.
:::

Pour modifier une politique de conservation, procédez comme suit :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet gauche, sous **Enterprise Guard**, cliquez sur **Cycle de vie du contenu**.
3. Cliquez sur l'onglet **Conservation**.
4. Sur la page des **politiques de conservation**, cliquez sur la **politique de conservation** que vous souhaitez modifier.
   La page affichant les informations relatives à la politique s’affiche.
5. Cliquez sur **Modifier** en haut à droite de la page, puis modifiez le champ requis. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Nom**  **(obligatoire)** | Nom de la politique de conservation.  Longueur maximale : 60 caractères. |
   | **Description**  **(facultatif)** | Description de cette politique de conservation.  Longueur maximale : 300 caractères. |
   | **Période de conservation**  **(obligatoire)** | Empêchez la suppression définitive des tableaux pendant une période spécifique en fonction de l'un des critères suivants : **Dernier accès**, **Dernière modification**, ou **Créé le**. Sélectionnez un chiffre, choisissez **mois** ou **années**, puis sélectionnez l'événement à partir duquel la période de conservation est calculée.  Si vous spécifiez la durée de conservation en mois, vous devez sélectionner une durée de conservation comprise entre 1 et 120 mois.  Si vous spécifiez la durée de conservation en années, vous devez sélectionner une durée de conservation comprise entre 1 et 10 ans. |
   | **Portée**  **(obligatoire)** | Sélectionnez la portée de cette politique de conservation. La portée indique les tableaux pour lesquels cette politique de conservation est applicable. Vous pouvez définir la portée d’une politique de conservation pour tous les tableaux d’une organisation ou pour des niveaux spécifiques de classification des tableaux.  **Définir la politique de conservation pour tous les tableaux de l'organisation** Si vous souhaitez définir le périmètre de la politique de conservation pour tous les tableaux de l'organisation, dans la liste **Périmètre**, sélectionnez **Tous les tableaux de l'organisation**.  **Définir la politique de conservation pour une ou plusieurs équipes de l'organisation** Si vous souhaitez définir le périmètre de la politique de conservation pour une ou plusieurs équipes de l'organisation, effectuez les étapes suivantes :  1. Dans la liste **Portée**, sélectionnez **Équipe**. 2. Cliquez sur la case Entrer une équipe et sélectionnez chaque équipe pour laquelle vous souhaitez appliquer la politique de conservation. Une coche apparaît à côté de l'équipe que vous avez choisie pour associer à la politique de conservation.   ✏️ - Vous pouvez sélectionner plusieurs équipes pour une politique de conservation. Cependant, une équipe donnée ne peut être associée qu'à une seule politique de conservation à la fois. - Vous pouvez sélectionner n'importe quelle équipe, y compris les équipes supprimées, comme périmètre lors de la définition de la politique de conservation.   - Une équipe sélectionnée comme périmètre pour une politique de conservation ne peut pas être supprimée définitivement tant qu'elle n'est pas retirée du périmètre.  **Définir la politique de conservation pour un niveau de classification de tableau**  ✏️ Pour définir la portée de la politique de conservation à un niveau spécifique de classification des tableaux, vous devez vous assurer que la fonctionnalité de classification des données est activée. Une fois qu'une politique de conservation utilise un niveau de classification des tableaux, vous ne pouvez pas désactiver la fonctionnalité de classification des données. Pour plus d'informations, consultez la documentation sur [la classification des données](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Si vous souhaitez définir la portée de la politique de conservation pour un niveau de classification spécifique, procédez comme suit :  1. Dans la liste **Portée**, sélectionnez **Classification**. 2. Cliquez sur la liste à côté de la liste **Classification**, puis sélectionnez les niveaux de classification pour lesquels vous souhaitez appliquer la politique de conservation. Vous pouvez également rechercher les niveaux de classification, puis les sélectionner.  Une coche apparaît à côté des niveaux de classification associés à la politique de conservation.  ✏️ **Notes :** - Vous pouvez sélectionner plusieurs niveaux de classification à la fois. - Vous ne pouvez pas définir le même niveau de classification pour différentes politiques de conservation. Si un niveau de classification spécifique est déjà associé à une politique de conservation, le niveau de classification apparaît en grisé.  - Une fois qu’une politique de conservation utilise un niveau de classification de tableau, vous ne pouvez pas désactiver la fonction de classification des données.  - Une fois qu’un niveau de classification est associé à une politique de conservation, vous ne pouvez pas supprimer ce niveau de classification spécifique. - Lorsqu’un tableau est régi à la fois par la politique de conservation de tous les tableaux du périmètre de l’organisation et par la politique de conservation du périmètre de classification, c’est la politique dont la durée de conservation est la plus longue qui s’applique. |
6. Lorsque vous avez terminé, cliquez sur **Suivant**.
   La **page d'impact de la révision** apparaît.
7. Examinez l’impact de la politique de conservation. La page d’impact de l’examen fournit les informations suivantes :
   - **Résumé :** configuration de la politique de conservation, telle que le nom de la politique, la période de conservation et la portée.
   - **Impact de la politique :** nombre de tableaux qui seront régis par cette politique. La politique de conservation s’applique également aux tableaux mis à la corbeille, qui sont pris en compte dans le calcul d’examen de l’impact.

   > ✏️ Lorsqu’un tableau est régi à la fois par une politique de conservation basée sur la durée et par une politique de conservation basée sur la classification, la politique dont la durée de conservation est la plus longue est applicable.
8. Pour enregistrer la configuration et appliquer la politique de conservation, cliquez sur **Publier**.

:::note
La création, la mise à jour ou la suppression d’une politique déclenche le processus des politiques de conservation, qui peut prendre jusqu’à 24 heures. Cependant, la mise à jour du nom ou de la description d’une politique se fait immédiatement, car ces actions ne déclenchent pas le processus des politiques de conservation.
:::
