---
title: Supprimer la politique de suppression
article_id: 19551053395090
translation_id: 19551053395090
locale: fr
sidebar_position: 19
created_at: '2024-06-14T19:52:35Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

Si une politique de suppression est supprimée, toutes les dates de suppression associées pour les tableaux le seront également. Par conséquent, les tableaux liés à cette politique ne seront plus automatiquement déplacés vers la corbeille.

:::note
Pour supprimer les politiques de suppression, vous devez avoir le [rôle d’admin de gouvernance des données](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin de gouvernance des données, contactez votre admin d’entreprise.
:::

Pour supprimer une politique de suppression, procédez comme suit :

1. Accédez aux [Paramètres de Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard**, cliquez sur **Cycle de vie du contenu**.
3. Sur la page **Cycle de vie du contenu,** cliquez sur **Suppression**.
   La page **Politiques de suppression** s’affiche.
4. Sur la page **Politiques de suppression**, cliquez sur la politique que vous souhaitez modifier.
   La page contenant les informations relatives à cette politique s’affiche.
5. Cliquez sur **Supprimer** en haut à droite de la page.
6. Examinez l’impact de l’annulation de la politique de suppression. La page d’examen de l’impact fournit les informations suivantes :
   - **Résumé :** les éléments de configuration de la politique de suppression, tels que le nom de la politique, la période de suppression et la portée.
   - **Impact de la politique :** le nombre de tableaux qui seront gouvernés par cette politique.
7. Pour supprimer la politique de suppression, cliquez sur **Supprimer la politique**.

:::note
Le fait de créer, de mettre à jour ou de supprimer une politique déclenche le processus de politiques de suppression, susceptible de durer jusqu’à 24 heures. Toutefois, la modification du nom ou la description d’une politique se fait immédiatement, car ces actions ne déclenchent pas le processus de politiques de suppression.
:::
