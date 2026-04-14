---
title: 'Déplacer des données d’une région à une autre : export et import manuels'
article_id: 24778387087122
translation_id: 24778387087122
locale: fr
sidebar_position: 6
created_at: '2025-02-20T09:07:00Z'
updated_at: '2025-11-25T15:49:48Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Qui peut le faire: les propriétaires de tableaux, les copropriétaires de
    tableaux, les admins de contenu, les admins d’entreprise Avec quel forfait: Enterprise
    Sur quelle plateforme: navigateur, bureau'
---

Cet article décrit les modalités d’export et d’import manuels pour déplacer des données d’une région à une autre. Pour en savoir plus sur les options de déplacement des données entre différentes régions, et notamment la migration automatisée, consultez [Déplacer des données d’une région à une autre](../../canvas-25-admin-features/data-residency/03-move-data-between-regions.md).

## Préparer un export et un import manuels dans une nouvelle région

En tant qu’admin d’entreprise, les meilleures pratiques suivantes vous aident à préparer un transfert manuel vers une nouvelle région :

- Pour créer une organisation dans votre région cible, contactez votre interlocuteur ou interlocutrice Miro.
- Pour bien gérer tous les utilisateurs de votre domaine, vérifiez tous les domaines qui vous appartiennent avec la vérification DNS.
- Dans la politique de contrôle des domaines, activez **Bloquer la création d’abonnements** pour éviter que les utilisateurs ne créent accidentellement des abonnements Miro gratuits dans votre ancienne région.
- Regroupez les équipes et/ou les organisations en une seule organisation avec un seul abonnement.
- Auditez les intégrations utilisées et les besoins de votre organisation dans la nouvelle région, puis préparez un calendrier pour reconfigurer chaque intégration dans votre nouvelle région.
- Auditez tous les paramètres utilisés actuellement par votre organisation, puis préparez un calendrier pour reconfigurer tous les paramètres nécessaires dans votre nouvelle région.

## Exporter et importer manuellement des données vers une nouvelle région

Miro crée une nouvelle organisation Enterprise dans la région cible. Les utilisateurs doivent exporter leurs tableaux sous forme de sauvegardes depuis la région source, puis importer leur sauvegarde dans la région cible.

**Pour en savoir plus :** Consultez [Comment sauvegarder un tableau](../../../using-miro/import-and-export/export/05-how-to-save-board-backup.md).

Seuls les utilisateurs disposant des autorisations suivantes peuvent exporter et importer du contenu manuellement :

- Propriétaire du tableau
- Copropriétaire de tableau
- Admin d’entreprise
- Admin de contenu

:::note
Tout partage du tableau est désactivé. Les utilisateurs doivent restaurer leurs autorisations de partage après avoir chargé leur sauvegarde dans la région cible.
:::

Pour importer des contenus manuellement, les utilisateurs peuvent se connecter à leur nouvelle URL régionale :

- (Australie) [au.miro.com](https://au.miro.com/), ou
- (États-Unis) [us.miro.com](https://us.miro.com/)

:::note
Avant de vous connecter pour la première fois en tant qu’utilisateur, vérifiez si votre organisation utilise l’authentification unique (SSO). Si vous utilisez l’authentification unique, attendez que votre admin d’entreprise reconfigure les paramètres de l’authentification unique pour votre nouvelle région.
:::

## Marche à suivre après une exportation et une importation manuelles

Après une migration des données interrégionale, assurez-vous de faire le nécessaire :

- Le cas échéant, reconfigurez immédiatement l’authentification unique pour les nouveaux sous-domaines régionaux. Par exemple, au.miro.com.
  > ✏️ Vos utilisateurs ne peuvent pas se connecter à la nouvelle région tant que l’authentification unique n’a pas été reconfigurée du côté de l’Identity provider.
- Reconfigurez le SCIM pour les nouveaux sous-domaines régionaux. Par exemple, au.miro.com.
- Dans les paramètres de contrôle de domaine, vérifiez que **Bloquer la création d’abonnements** est activé.
- Validez tous les autres paramètres de l’organisation, du contrôle des domaines et des équipes.
- Réinstallez et configurez chaque application et intégration Enterprise, notamment SIEM, SAM, eDiscovery, Smarsh et Okta.
- Invitez les utilisateurs à l’organisation dans la nouvelle région.

## FAQ sur l’export et l’import manuels des données vers une nouvelle région

**En quoi consiste le déplacement manuel vers une nouvelle région ?**

Les admins se chargent de reconfigurer l’organisation et l’ensemble de ses équipes, les paramètres de l’équipe et les utilisateurs ; les utilisateurs finaux téléchargent manuellement les sauvegardes des tableaux depuis l’ancienne organisation, puis les chargent dans la nouvelle organisation.

**Qui peut accéder à cette fonctionnalité ?**

Les clients Enterprise peuvent déplacer leurs données vers une autre région. Pour plus d’informations, contactez votre interlocuteur ou interlocutrice Miro.

**Quelles données sont concernées par un déplacement manuel ?**

Seuls les tableaux déplacés par les utilisateurs. Pour plus d’informations, consultez Exporter et importer manuellement des données vers une nouvelle région.

**La migration a-t-elle un coût ?**

Non. Miro peut créer une nouvelle organisation en Australie ou aux États-Unis selon le contrat Enterprise standard.

**Quels sont les délais pour un déplacement manuel ?**

La durée d’un déplacement manuel dépend de la vitesse à laquelle les utilisateurs exportent les tableaux enregistrés en tant que sauvegarde et les importent vers la région cible.

**Comment est-ce que Miro garantit que les données de mon organisation sont supprimées de la région source ?**

Notifiez le service d’assistance Miro une fois que vous avez terminé l’exportation et l’importation manuelles vers votre nouvelle région, y compris la reconfiguration, et que tous les utilisateurs ont importé leurs sauvegardes vers la région cible. Le service d’assistance de Miro supprimera alors votre organisation et toutes les données de la région source.
