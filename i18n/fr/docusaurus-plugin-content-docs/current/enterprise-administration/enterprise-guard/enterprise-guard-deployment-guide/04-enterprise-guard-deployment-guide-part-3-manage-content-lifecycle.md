---
title: 'Enterprise Guard Deployment Guide Part 3 : Gérer le cycle de vie du contenu'
article_id: 17121851926546
translation_id: 17121851926546
locale: fr
sidebar_position: 3
created_at: '2024-02-19T10:01:34Z'
updated_at: '2025-11-25T15:41:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
availability:
  notes: 'Équipes concernées: ** Les équipes avec lesquelles vous devrez peut-être
    vous associer pour déployer les fonctionnalités du cycle de vie du contenu sont,
    par exemple, la GRC (gouvernance, risque, conformité), la gestion de la conformité,
    le service juridique et/ou la gestion des archives.'
---

## Aperçu de la gestion du cycle de vie du contenu

Dans la plupart des Enterprise, le contenu croît de manière exponentielle, tant en volume qu'en complexité. Une gestion et une gouvernance adéquates des tableaux Miro sont essentielles pour de multiples raisons :

- Respecter de manière proactive les réglementations spécifiques à l'industrie ou les directives internes de l'organisation.
- Minimiser les risques dans des scénarios tels que les litiges juridiques ou les failles de sécurité
- Maintenir l'efficacité de l'organisation

Nous prenons actuellement en charge les fonctionnalités suivantes :

- [Politiques de gestion de la corbeille](https://help.miro.com/hc/articles/13860817985426-Trash-Policy)
- [Politiques de conservation](https://help.miro.com/hc/articles/16855776325778-Retention-policies)

## Vue d'ensemble du déploiement de la gestion du cycle de vie du contenu

Alors que le processus recommandé de [Partie 2 : Déployer la sécurité des données](03-enterprise-guard-deployment-guide-part-2-deploy-data-security.md) inclut la configuration progressive et la communication avec l'utilisateur final, ce qui n'est pas le cas de la gestion du cycle de vie du contenu.

Ni les politiques corbeille ni les politiques de conservation ne sont susceptibles de perturber l'activité de l'utilisateur final dans Miro et peuvent donc être configurées immédiatement.

## Déployer une politique de conservation globale

Actuellement, seule une politique de conservation globale est prise en charge par Enterprise Guard. D'autres options de configuration seront disponibles et offriront une plus grande flexibilité à l'avenir. Prenez en compte les exigences réglementaires de votre secteur et les politiques de votre organisation pour déterminer la durée de votre politique de conservation globale.

Comme il n'est pas possible d'obtenir une plus grande granularité, il peut être utile de configurer votre politique de conservation globale de manière à ce qu'elle corresponde à l'exigence la plus longue prévue par votre organisation. Par exemple, si certains contenus dans Miro doivent être conservés pendant 5 ans en raison d'une exigence réglementaire, votre politique de conservation globale doit être fixée à 5 ans.

Vous pouvez réduire l'étendue des tableaux conservés dans le cadre de cette politique de conservation de cinq ans lorsque Miro mettra en place des niveaux de conservation plus granulaires, tels que le niveau de classification ou l'équipe.

[Comment configurer les politiques de conservation ?](https://help.miro.com/hc/articles/16855776325778-Retention-policies)

## Configurer la politique de gestion de la corbeille

Par défaut, les tableaux Miro sont automatiquement et définitivement supprimés de la Corbeille après 90 jours. Vous pouvez mettre à jour le paramètre par défaut et choisir de supprimer automatiquement et définitivement les tableaux de la Corbeille dans 30, 60, 90 ou 180 jours.

Lorsque vous mettez à jour la période de suppression automatique et permanente des tableaux, la période mise à jour ne s’applique qu’aux tableaux nouvellement déplacés vers la Corbeille. Les tableaux doivent être déplacés manuellement vers la corbeille par les propriétaires ou copropriétaires du tableau.

Lorsqu'un tableau se trouve dans la corbeille mais que la période de suppression n'est pas terminée, certains utilisateurs peuvent supprimer manuellement et définitivement les tableaux. Choisissez qui peut le faire dans les tableaux de la corbeille entre les propriétaires du tableau et les administrateurs.

[Comment configurer les politiques de gestion de la corbeille ?](https://help.miro.com/hc/articles/13860817985426-Trash-settings)

## La conservation et la corbeille travaillent ensemble

Les politiques de conservation l'emportent sur les politiques de corbeille et la suppression manuelle et permanente. Voir les exemples et le diagramme ci-dessous.

Exemples

- Si un tableau est déplacé vers la Corbeille et supprimé manuellement et définitivement par son propriétaire, mais que le tableau est soumis à une politique de conservation, il sera conservé. À la fin de la période de conservation, le tableau sera immédiatement et définitivement supprimé.
- Si un tableau est déplacé vers la Corbeille et que la période de suppression permanente se termine mais que le tableau est soumis à une politique de conservation, le tableau sera conservé. À la fin de la période de conservation, le tableau sera immédiatement et définitivement supprimé.

![Enterprise Guard-Politiques de la corbeille.pngRétention](images/21017043245074_Enterprise-Guard-Trash-Policies.png)
*et corbeille travaillent ensemble*
