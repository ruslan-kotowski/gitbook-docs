---
title: Ajouter une politique de suppression
article_id: 19551031552018
translation_id: 19551031552018
locale: fr
sidebar_position: 17
created_at: '2024-06-14T19:49:31Z'
updated_at: '2025-12-08T16:13:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

:::note
Pour ajouter des politiques de suppression, vous devez avoir le rôle d’[admin de gouvernance des données](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d'admin de gouvernance des données, contactez l'admin de votre entreprise.
:::

Pour ajouter une politique de suppression, procédez comme suit :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le panneau de gauche, sous **Enterprise Guard,** cliquez sur **Cycle de vie du contenu**.
3. Cliquez sur l'onglet **Suppression**.
   La page **Politiques de suppression** s'affiche.
4. Cliquez sur **Ajouter une politique de suppression**.
5. Saisissez ou sélectionnez les informations appropriées pour chaque champ. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Nom**  **(obligatoire)** | Nom de la politique de suppression.  Longueur maximale : 60 caractères. |
   | **Description**  **(facultatif)** | Description de cette politique de suppression.  Longueur maximale : 300 caractères. |
   | **Période de suppression**  **(obligatoire)** | Précisez quand les tableaux sont automatiquement mis à la Corbeille. Choisissez un nombre, sélectionnez **Mois** ou **Années**, puis choisissez si la période est calculée à partir de la date de **dernière modification** ou de **dernier accès** du tableau.  Si vous spécifiez la période de suppression en mois, vous devez sélectionner une période de suppression comprise entre 1 et 120 mois.  Si vous spécifiez la période de suppression en années, vous devez sélectionner une période de suppression comprise entre 1 et 10 ans.  Par exemple, si vous souhaitez que les tableaux soient déplacés dans la corbeille lorsqu'ils n'ont pas été modifiés pendant un an, vous pouvez sélectionner 1 an et choisir **Dernière modification**. |
   | **Champ d’application**  **(obligatoire)** | Sélectionnez le champ d’application de cette politique de suppression. Le champ d’application indique les tableaux pour lesquels cette politique de suppression est applicable. Vous pouvez définir le champ d’application d’une politique de suppression pour tous les tableaux d’une organisation ou pour des niveaux spécifiques de classification des tableaux.  **Définir la politique de suppression pour tous les tableaux de l'organisation** Si vous souhaitez définir le champ d'application de la politique de suppression pour tous les tableaux de l'organisation, dans la liste **Champ d'application**, sélectionnez **Tous les tableaux de l'organisation**.  **Définir la politique de suppression pour une ou plusieurs équipes de l'organisation** Si vous souhaitez définir le champ d'application de la politique de suppression pour une ou plusieurs équipes de l'organisation, suivez les étapes suivantes :  1. Dans la liste **Portée**, sélectionnez **Équipe**. 2. Cliquez sur la case **Entrer équipe** et sélectionnez chaque équipe pour laquelle vous souhaitez appliquer la politique de suppression. Une coche apparaît à côté de l'équipe que vous avez sélectionnée pour l'associer à la politique de suppression.   ✏️ - Vous pouvez sélectionner plusieurs équipes pour une suppression. Cependant, une équipe donnée ne peut être associée qu'à une seule suppression à la fois.  - Vous pouvez sélectionner n'importe quelle équipe, y compris les équipes supprimées, comme périmètre lors de la configuration de la politique de suppression.   - Une équipe sélectionnée comme périmètre pour une politique de suppression ne peut pas être supprimée définitivement tant qu'elle n'est pas retirée du périmètre.  **Configurer la politique de suppression pour un niveau de classification de tableau**  ✏️ Pour définir la portée de la politique de suppression à un niveau spécifique de classification des tableaux, vous devez vous assurer que la fonctionnalité de classification des données est activée. Une fois qu'une politique de suppression utilise un niveau de classification de tableau, vous ne pouvez pas désactiver la fonctionnalité de classification des données. Pour plus d'informations, consultez la documentation sur [Classification des données](https://help.miro.com/hc/sections/15451275412498-Auto-classification).  Si vous souhaitez définir la portée de la politique de suppression pour un niveau de classification de tableau spécifique, procédez comme suit :  1. Dans la liste **Portée**, sélectionnez **Classification**. 2. Cliquez sur la liste à côté de la liste **Classification**, puis sélectionnez les niveaux de classification pour lesquels vous souhaitez appliquer la politique de suppression. Vous pouvez également rechercher les niveaux de classification, puis les sélectionner.  Une coche apparaît en regard des niveaux de classification que vous avez choisis d’associer à la politique de suppression.  ✏️ **Notes :** - Vous pouvez sélectionner plusieurs niveaux de classification à la fois. - Vous ne pouvez pas définir le même niveau de classification pour différentes politiques de suppression. Si un niveau de classification spécifique est déjà associé à une politique de suppression, le niveau de classification apparaît en grisé.  - Une fois qu'une politique de suppression utilise un niveau de classification de tableau, vous ne pouvez pas désactiver la fonctionnalité de classification des données.  -Une fois qu'un niveau de classification est associé à une politique de suppression, vous ne pouvez pas supprimer ce niveau de classification spécifique. - Lorsqu’un tableau est régi à la fois par la politique de suppression de tous les tableaux du périmètre de l’organisation et par la politique de suppression du périmètre de classification, c’est la politique dont la durée de suppression est la plus longue qui s’applique. |
6. Cliquez sur **Suivant**.
   La **page de révision de l'impact** s'affiche.
7. Examinez l’impact de la politique de suppression. La page d’impact de l’examen fournit les informations suivantes :
   - **Résumé :** configuration de la politique de suppression, telle que le nom de la politique, la période de suppression et le champ d’application.
   - **Impact de la politique :** nombre de tableaux qui seront régis par cette politique.
8. Pour enregistrer la configuration et appliquer la politique de suppression, cliquez sur **Publier**.
   La boîte de dialogue **Activer la notification de suppression** apparaît.
9. **Notifications de suppression** permettent aux utilisateurs de recevoir des alertes préalables avant qu'un tableau ne soit automatiquement déplacé vers la corbeille en raison d'inactivité. Ces alertes aident les utilisateurs à prendre des mesures s'ils souhaitent conserver leur contenu.

   Si vous souhaitez activer les notifications de suppression :

   a. Cliquez sur **Notifier**.

   b. Configurez combien de jours à l'avance la notification doit être envoyée — une valeur comprise entre **1 et 30 jours**.

   Si l’activation des notifications entraîne **le déplacement immédiat de certains tableaux vers la corbeille** (car ils ont déjà dépassé le seuil), vous serez invité à indiquer si vous souhaitez notifier les utilisateurs à propos de ces tableaux spécifiques. Vous pouvez choisir :

   - **Oui** – pour notifier les propriétaires et copropriétaires des tableaux même si le tableau est déplacé immédiatement vers la corbeille.

   - **Non** – pour déplacer les tableaux sans envoyer de notification pour cette action immédiate.

   Une fois activée, les utilisateurs dont les tableaux sont sous le champ d'application d'une politique de suppression avec notifications activées :

   - Recevront une notification dans leur Miro **fil d’actualité** pendant la période d'inspection configurée.

   - Pourront ouvrir directement le tableau à partir de la notification.

   - Voir une **bannière** sur le tableau avertissant de la prochaine suppression automatique, avec une option pour **Conserver le tableau** s'ils souhaitent le garder.

:::note
La création, la mise à jour ou la suppression d’une politique déclenche le processus de suppression des politiques, qui peut prendre jusqu’à 24 heures. Cependant, la mise à jour du nom ou de la description d’une politique se fait immédiatement car ces actions ne déclenchent pas le processus de suppression des politiques.
:::

#
