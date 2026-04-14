---
title: "Aper\xE7u des sc\xE9narios de suppression"
article_id: 19596032332434
translation_id: 19596032332434
locale: fr
sidebar_position: 6
created_at: '2024-06-17T17:24:29Z'
updated_at: '2025-12-08T16:00:51Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-lifecycle-management
---

## Déplacement automatique des tableaux vers la corbeille

Les tableaux sont automatiquement placés dans la corbeille à la date de leur suppression désignée. Si aucune politique de conservation active n'affecte le tableau, sa suppression permanente sera déterminée par la politique de gestion de la corbeille.
![disposition1.png](images/21019706099858_disposition1.png)

Prenons l’exemple d’un tableau de projet qui doit être transféré dans la corbeille le 1er juillet 2025, conformément à la politique de suppression, et qui n’est soumis à aucune politique de conservation. Le tableau sera automatiquement déplacé dans la corbeille le 1er juillet 2025 et définitivement supprimé le 29 septembre 2025, conformément à la politique de la corbeille de 90 jours.

:::note
Une politique de conservation active remplace la politique de la corbeille. Par conséquent, la date de suppression définitive du tableau suivra la politique de conservation en vigueur.
:::

Si les notifications de suppression sont activées pour la politique, les utilisateurs recevront une notification en fonction du nombre de jours configurés avant que le tableau ne soit prévu pour être déplacé dans la corbeille.

La notification apparaît dans le fil d’actualité de Miro et renvoie directement au tableau. Une bannière est également affichée en haut du tableau pour avertir l'utilisateur de l'action de mise à la corbeille à venir. Bo">Les propriétaires et copropriétaires ont l'option de conserver le tableau.

## Suppression de tableaux à l’initiative de l’utilisateur

Lorsque le propriétaire d’un tableau le place dans la Corbeille, la politique de suppression n’a plus d’incidence sur le cycle de vie du tableau. Si aucune politique de conservation active ne s’applique au tableau, sa suppression permanente suivra la politique corbeille.

![disposition2.png](images/21019694974610_disposition2.png)

Prenons l’exemple d’un tableau de plan opérationnel dont la suppression est prévue le 13 octobre 2024. Si le propriétaire du tableau déplace de manière préemptive le tableau vers la Corbeille le 15 mai 2024, et qu’il n’y a pas de politiques de gestion de la conservation actives affectant le tableau, celui-ci adhérera à la politique de la corbeille. Le tableau sera définitivement supprimé le 13 août 2024, conformément à la politique de la corbeille de 90 jours.

:::note
Si le tableau fait l’objet d’une politique de conservation active, cette politique remplacera la politique corbeille et fixera la date de suppression permanente conformément à la politique de conservation.
:::

## Restauration du tableau à l’initiative de l’utilisateur

Lorsqu’un utilisateur restaure un tableau depuis la corbeille, toute politique de suppression pertinente est automatiquement réappliquée. Ainsi, le tableau réintègre son cycle de vie en rétablissant tous les paramètres originaux de la politique.

![disposition3.png](images/21019706104082_disposition3.png)

Par exemple, si un utilisateur restaure de la corbeille, le 20 juin 2024, un tableau de stratégie marketing auquel s’appliquait auparavant une politique de suppression d’un an, cette politique est automatiquement réappliquée lors de la restauration. La nouvelle date de suppression du tableau sera recalculée à partir de la date de restauration, fixant sa date de suppression actualisée au 20 juin 2025 ou à un an de la date à laquelle ce tableau a été modifié pour la dernière fois après restauration.

## Notifications de suppression

Les notifications de suppression alertent les utilisateurs à l'avance lorsqu'un tableau est programmé pour être automatiquement déplacé dans la corbeille en raison de l'inactivité, sur la base d'une politique de suppression active.

- Les admins peuvent activer les notifications lors de la publication d'une politique.
- Le délai de notification est configurable de 1 à 30 jours avant le déplacement prévu.
- Les notifications sont envoyées selon le nombre de jours configuré, lorsque la notification de suppression doit être envoyée avant la date de mise en corbeille.

Lorsqu'un tableau entre dans la période d'inspection :

- Une notification apparaît dans le fil d'actualité de l'utilisateur.
- En cliquant dessus, vous ouvrez le tableau avec une bannière en haut qui avertit du déplacement imminent vers la corbeille.
- Les utilisateurs peuvent choisir de conserver le tableau pour le garder, ce qui réinitialise le minuteur de suppression.

Ce mécanisme de notification s'applique à tous les scénarios où :

- Une politique de suppression avec notifications est active.
- Le tableau entre dans sa période d'inspection (selon le nombre de jours configuré avant la date de suppression).

### Scénario 1 : Tableaux conformes à une politique de suppression

Ces tableaux relèvent d'une politique et seront déplacés vers la corbeille après la période d'inactivité définie.

Si les notifications de suppression sont activées pour la politique, une notification sera envoyée selon le nombre de jours configuré lorsque la notification de suppression doit être envoyée avant le déplacement programmé du tableau vers la corbeille. Le tableau affichera également une bannière permettant aux utilisateurs de l'examiner ou de le conserver.

### Scénario 2 : Tableaux avec un badge de classification ajouté après la dernière modification du tableau

Ces tableaux sont rétroactivement intégrés au champ d'application et suivent toujours le même calendrier de suppression basé sur leur date de dernière modification.

Si les notifications de suppression sont activées, les utilisateurs recevront une notification selon le nombre de jours configuré avant la date prévue pour le déplacement vers la corbeille, même si le badge a été appliqué après la dernière modification.

### Scénario 3 : Tableaux avec un badge de classification retiré avant la publication de la politique

Ces tableaux ne relèvent plus de la politique et sont exclus de l'évaluation de la suppression.

Étant donné qu'ils sont hors champ, aucune notification de suppression ne sera envoyée.

### Scénario 4 : Tableaux récemment modifiés et pas encore dans le seuil de suppression

Ces tableaux ont été modifiés récemment et ne sont pas encore éligibles à la suppression.

Une notification ne sera envoyée que si le tableau entre dans la période d'inspection, c'est-à-dire selon le nombre de jours configuré avant la date de suppression. Jusque-là, aucune notification n'est déclenchée.

### Scénario 5 : Tableaux modifiés après l'entrée en période d'inspection

Une fois qu'un tableau entre dans la période d'inspection, sa date de suppression est verrouillée. Cela signifie que, sauf si un propriétaire de tableau choisit explicitement de conserver le tableau, il sera automatiquement déplacé dans la corbeille à la date prévue.

Modifier ou accéder au tableau pendant la période d'inspection n'affecte pas le calendrier de suppression. Les actions suivantes n'affecteront pas le résultat de la suppression : modifier ou consulter le tableau, changer son badge de classification ou d'équipe, ou même supprimer la politique associée.

Si les notifications de suppression sont activées, une notification sera envoyée selon le nombre de jours configuré avant la date prévue de passage à la corbeille, et le tableau affichera une bannière permettant à l’utilisateur de l’examiner ou de le conserver.

### Scénario 6 : Tableaux qui ont déjà été supprimés ou déplacés manuellement dans la corbeille

Ces tableaux sont déjà retirés de l'espace de travail et ne sont plus gérés par des politiques de suppression.

Aucune notification de suppression n'est envoyée pour les tableaux qui sont déjà dans la corbeille ou définitivement supprimés.

### Scénario 7 : Tableaux soumis à plusieurs politiques

Les tableaux peuvent être soumis à plus d'une politique de suppression active à la fois, surtout si plusieurs politiques ciblent le même badge de classification ou la même équipe.

Si plus d'une politique avec notifications activées s'applique à un tableau, l'utilisateur ne recevra qu'une seule notification lorsque le tableau entrera en période d'inspection. La notification est basée sur la politique avec la date de suppression la plus proche et est envoyée selon le nombre de jours configuré avant cette date.

## Scénario 8 : Tableaux déjà en état d'inspection et la politique de suppression est supprimée par la suite

Si un tableau est déjà entré dans la période d'inspection et que des notifications de suppression ont été envoyées (si activées), la date de suppression prévue est verrouillée. Même si la politique de suppression associée est ensuite supprimée ou modifiée, le tableau sera toujours automatiquement déplacé dans la corbeille à la date de suppression initiale, à moins que le propriétaire du tableau ne choisisse de le conserver.

En revanche, si la politique est supprimée avant qu'un tableau n'entre dans la période d'inspection, le tableau est considéré comme hors champ et ne sera pas déplacé vers la corbeille.
Cela garantit qu'une fois que les utilisateurs ont été notifiés, l'action de suppression reste cohérente et prévisible, quelles que soient les modifications de la politique effectuées par la suite.
