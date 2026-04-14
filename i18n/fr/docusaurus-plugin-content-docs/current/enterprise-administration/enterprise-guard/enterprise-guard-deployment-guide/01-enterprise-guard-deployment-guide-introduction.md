---
title: "Guide de d\xE9ploiement d'Enterprise Guard : Introduction"
article_id: 17120515162386
translation_id: 17120515162386
locale: fr
sidebar_position: 0
created_at: '2024-02-19T09:17:20Z'
updated_at: '2025-11-25T15:40:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

Ce document vous guidera dans le déploiement du produit de sécurité avancée de Miro, Enterprise Guard, en détaillant les meilleures pratiques pour la configuration et l'activation de l'utilisateur final. Si vous avez des questions concernant le contenu de ce guide, veuillez contacter l'équipe chargée de votre compte Miro.

## Comment utiliser ce guide

- Naviguez d'une section à l'autre à l'aide du plan situé à gauche de votre écran.
- Utilisez ce guide en conjonction avec la documentation sur les fonctionnalités dont les liens figurent dans le présent document.
- Personnalisez les modèles fournis pour faire gagner du temps à vos utilisateurs.

## Schéma du guide

- [Partie 1 | Configurer les rôles d'admin.](02-enterprise-guard-deployment-guide-part-1-configure-admin-roles.md)
- [Partie 2 - Déployer la sécurité des données](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md)
- [Partie 3 - Gérer le cycle de vie du contenu](04-enterprise-guard-deployment-guide-part-3-manage-content-lifecycle.md)

## Pourquoi avez-vous besoin d'Enterprise Guard ?

Miro est l'espace de travail en ligne prêt à l'emploi pour l'innovation qui transforme la façon dont les équipes distribuées, quelle que soit leur taille, accomplissent leur travail.

Nous avons constaté une augmentation considérable du travail stratégique effectué à Miro et, avec cette croissance, il y a encore plus de contenu à protéger et à régir.

Les données sensibles apparaissent là où les clients s'y attendent le moins. Sur la base d'un échantillon de 100 entreprises clientes, nous avons constaté que 62 % d'entre elles avaient des tableaux contenant des données sensibles telles que des informations personnelles identifiables, des informations de santé personnelles et des informations sur les cartes de crédit. Cette surface de risque ne fait qu'augmenter, car le nombre de tableaux pour nos entreprises clientes croît de 250 % chaque année.

Cette croissance du contenu rend encore plus difficile la gestion des risques au moyen des outils traditionnels existants ou en s'appuyant sur l'adhésion des employés aux politiques de l'entreprise.

Enterprise Guard est le module complémentaire de sécurité et de gouvernance des données pour Miro. Les entreprises peuvent trouver et sécuriser les contenus sensibles et gérer les cycles de vie des contenus, automatiquement et à grande échelle.

## Présentation d’Enterprise Guard : une solution complète de sécurité et de gouvernance pour Miro

Conscient de ces défis, Miro présente **Enterprise Guard**, un module complémentaire de sécurité et de gouvernance avancées. Enterprise Guard offre une série de fonctionnalités qui permettent aux entreprises d’identifier, de classer, de sécuriser et de gérer efficacement les contenus sensibles sur l’ensemble des tableaux Miro. Cette solution est adaptée pour garantir la conformité et une protection robuste des données à l’échelle.

Avec l’intégration d’Enterprise Guard dans l’écosystème d’entreprise de Miro, les organisations peuvent désormais tirer parti d’un cadre de sécurité plus robuste, plus automatisé et plus complet. Ce module complémentaire ne se limite pas à la protection des données, il permet aux Enterprise de continuer à innover et à collaborer sur Miro en toute sécurité, sans entraver les activités de l’entreprise.

## Enterprise Guard General Availability : caractéristiques principales

![Principales caractéristiques de la version de disponibilité générale d’Enterprise Guard](images/26240543449234_Enterprise-Guard-Data-Security.png)

- **Découverte de données :** Enterprise Guard permet un processus proactif et approfondi de découverte des données, crucial pour identifier les données sensibles telles que les numéros de carte de crédit, les numéros de sécurité sociale et d’autres informations critiques dispersées dans divers tableaux Miro. Cette stratégie proactive est cruciale pour identifier et atténuer les vulnérabilités potentielles, vous aidant ainsi à prévenir les violations de données et à garantir la conformité.
- eDiscovery Permettre la conservation, le suivi et l'exportation sécurisés des données des tableaux pour répondre aux exigences légales, de conformité et de sécurité. La fonction eDiscovery d'Enterprise Guard aide les entreprises à respecter leurs obligations réglementaires grâce aux fonctions de [conservation inaltérable](../../canvas-25-admin-features/ediscovery/02-legal-hold-overview.md), de [journaux de contenu](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md) et d'[exportation de tableaux](../../canvas-25-admin-features/ediscovery/13-board-export-api-overview.md).

  Les conservations inaltérables permettent d'éviter la suppression définitive de contenus liés à des enquêtes ou à des affaires juridiques en préservant tous les tableaux avec lesquels l'utilisateur concerné interagit, y compris toutes leurs versions. Les journaux de contenu fournissent des enregistrements détaillés de l'activité des utilisateurs, qui peuvent être exportés et intégrés dans des outils externes à des fins d'audit ou d'examen juridique. Grâce aux API eDiscovery, les clients Enterprise peuvent également exporter des données de tableau à l'échelle, garantissant ainsi l'accès aux informations critiques pour les workflows juridiques et de conformité.
- **Classification automatique :** Définissez des critères permettant à Miro de classer automatiquement vos tableaux en fonction du contenu sensible qui s’y trouve.
- ****Garde-fous intelligents :**** Appliquez des règles de sécurité en temps réel et limitez ce que les utilisateurs peuvent faire avec un tableau, par exemple en restreignant les capacités de réplication et de partage du contenu du tableau à différents niveaux (public, équipe, organisation), en fonction de la classification manuelle ou automatisée du tableau. Cela permet de garantir durablement la confidentialité et la conformité sans entraver les activités de l’entreprise.
- **Politique en matière de corbeilles:** La politique de la corbeille d’Enterprise Guard offre un contrôle renforcé sur la suppression et la restauration des tableaux Miro. Les entreprises peuvent définir des délais de suppression automatique (30, 60, 90, 180 jours) pour se conformer aux exigences réglementaires, en répondant à la nécessité de conservation des données tout en limitant les risques pour l’entreprise.
- **Conservation :** Assurez la protection des données et la conformité en permettant aux administrateurs de définir, modifier et supprimer des politiques adaptées aux besoins de leur organisation. Ces politiques jouent un rôle crucial dans la sauvegarde des tableaux Miro au sein de l’organisation, en vous permettant de conserver certains tableaux pendant une période déterminée. La conservation garantit que les tableaux Miro ne sont pas supprimés accidentellement ou intentionnellement jusqu’à ce que la période de conservation du tableau soit terminée. En s’appuyant sur les politiques de conservation, les entreprises peuvent assurer la protection des données, la conformité et la préservation des informations critiques.
- Suppression Activez le nettoyage automatique des tableaux en les archivant et en les supprimant en fonction des politiques de conservation. La [suppression](../../canvas-25-admin-features/content-lifecycle-management/03-disposition-overview.md) garantit que les tableaux ne sont conservés que le temps nécessaire et qu'ils sont automatiquement déplacés vers la Corbeille après une période d'inactivité. Ensuite, les paramètres standard de la corbeille déterminent qui peut restaurer les tableaux et quand ils seront définitivement supprimés, ce qui favorise la conformité, l'efficacité opérationnelle et la sécurité des données.
- ****Gestion des clés de chiffrement** **(EKM) :**** La gestion des clés de chiffrement assure un contrôle centralisé des clés de chiffrement, ce qui permet aux organisations de surveiller les activités liées aux clés et de révoquer l’accès chaque fois que nécessaire, garantissant ainsi une couche supplémentaire de sécurité des données.
