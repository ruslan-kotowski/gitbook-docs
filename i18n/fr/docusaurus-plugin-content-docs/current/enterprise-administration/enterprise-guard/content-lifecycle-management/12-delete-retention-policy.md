---
title: Supprimer la politique de conservation
article_id: 19205219887762
translation_id: 19205219887762
locale: fr
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

La suppression d’une politique de conservation libère les tableaux conservés associés à cette politique. Ces tableaux peuvent ensuite être supprimés définitivement sans contraintes.

:::note
Pour supprimer des politiques de conservation, vous devez avoir le [Data Governance Admin role>](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md)rôle d’administrateur de la gouvernance des données.</span></span> Pour demander le rôle d'administrateur de la gouvernance des données, contactez l'admin de votre entreprise.
:::

Pour supprimer une politique de conservation, procédez comme suit :

1. [Accédez à vos paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard**, cliquez sur **Cycle de vie du contenu**.
3. Cliquez sur l'onglet **Rétention**.
4. Sur la page **Conservation** **de politiques**, cliquez sur la politique de conservation que vous souhaitez supprimer.
   La page affichant les informations relatives à la politique s’affiche.
5. Cliquez sur **Supprimer** en haut à droite de la page.
6. Examinez l’impact de la suppression de la politique de conservation. La page d’impact de l’examen fournit les informations suivantes :
   - **Résumé :** configuration de la politique de conservation, telle que le nom de la politique, la période de conservation et le champ d'application.
   - **Impact sur la politique :** nombre de tableaux qui seront libérés de la conservation et pourront être définitivement supprimés sans contraintes. La politique de conservation s’applique également aux tableaux mis à la corbeille, qui sont inclus dans le calcul de l’impact de la révision.
7. Pour supprimer la politique de conservation, cliquez sur **Supprimer la politique**.

:::note
La création, la mise à jour ou la suppression d’une politique déclenche le processus des politiques de conservation, qui peut prendre jusqu’à 24 heures. Cependant, la mise à jour du nom ou de la description d’une politique se fait immédiatement, car ces actions ne déclenchent pas le processus des politiques de conservation.
:::
