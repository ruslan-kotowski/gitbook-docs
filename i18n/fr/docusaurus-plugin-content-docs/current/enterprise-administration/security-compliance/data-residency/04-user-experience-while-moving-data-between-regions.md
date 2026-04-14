---
title: L’expérience utilisateur lors du déplacement de données d’une région à une
  autre
article_id: 25075857856658
translation_id: 25075857856658
locale: fr
sidebar_position: 4
created_at: '2025-03-04T08:51:38Z'
updated_at: '2025-05-09T08:47:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Qui peut le faire: tous les utilisateurs Avec quel forfait: Enterprise Sur
    quelles plateformes: navigateur, ordinateur de bureau, mobile'
---

Cet article décrit l’expérience utilisateur pendant la migration des données d’une région à une autre, pour les imports et les exports aussi bien [automatiques](../../canvas-25-admin-features/data-residency/05-move-data-between-regions-–-automated-migration.md) que [manuels](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## L’expérience utilisateur pendant la migration automatisée (bêta)

Les sections suivantes décrivent ce qui se produit avant, pendant et après un déplacement automatisé des données d’une région à une autre.

### Avant la migration automatisée

Deux semaines avant la migration, tous les utilisateurs de votre organisation Enterprise reçoivent les notifications suivantes :

- **Via une bannière intégrée au produit**
  Annonce la date de la migration et la période prévue dans le fuseau horaire local
- **Par e-mail**
  Décrit la prochaine maintenance planifiée pour tous les utilisateurs de votre organisation Enterprise

:::note
Si vous êtes membre de plusieurs comptes Miro, vos autres comptes restent accessibles pendant la migration.
:::

### Pendant la migration automatisée

Une migration automatisée entraine environ 8 heures d’inactivité.

Pendant une migration automatisée, vous ne pouvez pas accéder aux données de votre organisation Enterprise, y compris les tableaux, les équipes et les paramètres.

Le tableau de bord Miro affiche une notification indiquant qu’une migration des données de votre organisation est en cours. Pendant le processus de migration, vous n’aurez pas accès aux tableaux, aux équipes ni aux paramètres de l’organisation.

:::tip
Si vous êtes membre de plusieurs organisations, vous pouvez passer à une autre organisation à partir de votre tableau de bord et continuer à utiliser Miro.
:::

### Après la migration automatisée

Lorsque la migration est terminée, vous recevez un e-mail de confirmation. Un message apparait sur votre tableau de bord Miro pour confirmer que la migration a bien été effectuée.

Si la migration échoue, vous recevez une notification par e-mail. Vous pouvez continuer à utiliser Miro dans la région UE en vous connectant sur [miro.com](https://miro.com).

### La redirection depuis le tableau après la migration automatique

Tous les tableaux que vous avez mis en signet dans votre région initiale redirigent automatiquement vers la nouvelle région et leur URL est mise à jour.

## L’expérience utilisateur pendant l’export et l’import manuels

Les utilisateurs doivent exporter manuellement les sauvegardes des tableaux depuis leur région source, puis importer leurs sauvegardes dans la région cible.

**Pour en savoir plus :** consultez [Déplacer des données d’une région à une autre : l’export et l’import manuels](../../canvas-25-admin-features/data-residency/06-move-data-between-regions-–-manual-export-and-import.md).

## Les collaborations interrégionales

Les utilisateurs de Miro sont rattachés à une région. Pour collaborer avec des utilisateurs appartenant à une organisation située en dehors de votre région, vous devez avoir un profil d’utilisateur dans leur région.

Par exemple, si vous êtes un utilisateur appartenant à la région UE et que vous souhaitez collaborer avec des utilisateurs d’une organisation de la région Australie, vous devez créer un profil d’utilisateur distinct sur [au.miro.com](https://au.miro.com/).
