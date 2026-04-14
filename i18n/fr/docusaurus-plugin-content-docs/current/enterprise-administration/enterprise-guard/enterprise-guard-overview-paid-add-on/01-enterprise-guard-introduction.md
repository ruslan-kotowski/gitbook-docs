---
title: "Introduction \xE0 Enterprise Guard"
article_id: 15699815402514
translation_id: 15699815402514
locale: fr
sidebar_position: 0
created_at: '2023-12-11T23:40:22Z'
updated_at: '2025-11-25T15:40:09Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

À l’ère du numérique, la croissance exponentielle des données, en particulier des informations sensibles, est devenue une préoccupation importante pour les entreprises. Miro, connu pour son espace de travail collaboratif en ligne prêt pour l'entreprise qui favorise l'innovation et le travail d'équipe, a observé une augmentation substantielle de la complexité et de la quantité de contenu au sein de ses tableaux. Un nombre important de tableaux Miro contiennent des données hautement sensibles, telles que des informations personnelles identifiables (PII), des informations de santé protégées (PHI), des informations de cartes de paiement (PCI), et plus encore, ce qui pose des défis en matière de gestion des risques et de conformité. Cette tendance souligne l’importance de mettre en œuvre des mesures de sécurité et de conformité avancées pour aider à prévenir les violations de données potentielles et les fuites de propriété intellectuelle.

## Présentation d’Enterprise Guard : une solution complète de sécurité et de gouvernance pour Miro

Conscient de ces défis, Miro présente **Enterprise Guard**, un module complémentaire de sécurité et de gouvernance avancées. Enterprise Guard offre une série de fonctionnalités qui permettent aux entreprises d'identifier, de classer, de sécuriser et de gérer efficacement les contenus sensibles sur l'ensemble des tableaux Miro. Cette solution est adaptée pour garantir la conformité et une protection robuste des données à l’échelle.

Avec l’intégration d’Enterprise Guard dans l’écosystème d’entreprise de Miro, les organisations peuvent désormais tirer parti d’un cadre de sécurité plus robuste, plus automatisé et plus complet. Ce module complémentaire ne se limite pas à la protection des données—il permet aux entreprises de continuer à innover et à collaborer sur Miro en toute sécurité, sans entraver les opérations commerciales.

## Enterprise Guard General Availability : caractéristiques principales

![Principales caractéristiques de la version de disponibilité générale d’Enterprise Guard](images/21019694879890_Enterprise-Guard-Data-Security.png)

- **Découverte de données :** Enterprise Guard permet un processus proactif et approfondi de [découverte des données](../../canvas-25-admin-features/data-discovery/01-data-discovery-overview.md), crucial pour identifier les données sensibles telles que les numéros de carte de crédit, les numéros de sécurité sociale et d’autres informations critiques dispersées dans divers tableaux Miro. Cette stratégie proactive est cruciale pour identifier et atténuer les vulnérabilités potentielles, vous aidant ainsi à prévenir les violations de données et à garantir la conformité.
- **eDiscovery :** Activer la préservation, le suivi et l'exportation sécurisés des données des tableaux pour répondre aux exigences légales, de conformité et de sécurité. La fonctionnalité eDiscovery d'Enterprise Guard aide les organisations à répondre aux obligations réglementaires grâce aux capacités de [réserves légales](../../canvas-25-admin-features/ediscovery/02-legal-hold-overview.md), de [journaux de contenu](../../canvas-25-admin-features/ediscovery/06-content-logs-overview.md) et d'[exportation de tableaux](../../canvas-25-admin-features/ediscovery/13-board-export-api-overview.md).

  Les mises en suspens juridiques empêchent la suppression définitive de contenus pertinents pour les enquêtes ou les affaires juridiques en préservant tous les tableaux avec lesquels un utilisateur sous suspens interagit, y compris toutes leurs versions. Les journaux de contenu fournissent des enregistrements détaillés de l'activité des utilisateurs, qui peuvent être exportés et intégrés dans des outils externes pour des audits ou des examens légaux. Grâce aux API d'eDiscovery, les clients Enterprise peuvent également exporter des données de tableau à grande échelle, garantissant ainsi que les informations critiques sont accessibles pour les flux de travail juridiques et de conformité.
- **Classification automatique** : Définissez des critères permettant à Miro de [classer automatiquement vos tableaux](../../canvas-25-admin-features/data-classification/03-auto-classification-overview-and-scenarios.md) en fonction du contenu sensible qui s’y trouve.
- **Garde-fous intelligents** **:** [Appliquez des règles de sécurité en temps réel](../../canvas-25-admin-features/data-classification/01-intelligent-guardrails-overview.md) et limitez ce que les utilisateurs peuvent faire avec un tableau, par exemple en restreignant les capacités de réplication et de partage du contenu du tableau à différents niveaux (public, équipe, organisation), en fonction de la classification manuelle ou automatisée du tableau. Cela permet de garantir durablement la confidentialité et la conformité sans entraver les activités de l’entreprise.
- **Politique de corbeille** : La [politique de la corbeille d’Enterprise Guard](https://help.miro.com/hc/articles/13860817985426) offre un contrôle renforcé sur la suppression et la restauration des tableaux Miro. Les entreprises peuvent définir des délais de suppression automatique (30, 60, 90, 180 jours) pour se conformer aux exigences réglementaires, en trouvant un équilibre entre la conservation des données et la minimisation des risques pour l’entreprise.
- **Conservation :** Assurez la protection des données et la conformité en permettant aux administrateurs de définir, modifier et supprimer des politiques adaptées aux besoins de leur organisation. Ces politiques jouent un rôle crucial dans la sauvegarde des tableaux Miro au sein de l'organisation, en vous permettant de conserver certains tableaux pendant une période déterminée. [La conservation](https://help.miro.com/hc/articles/16855776325778) garantit que les tableaux Miro ne sont pas supprimés accidentellement ou intentionnellement jusqu’à ce que la période de conservation du tableau soit terminée. En s’appuyant sur les politiques de conservation, les entreprises peuvent assurer la protection des données, la conformité et la préservation des informations critiques.
- ****Suppression :**** Activer le nettoyage automatique des tableaux en les archivant et en les supprimant selon les politiques de conservation. [Disposition](../../canvas-25-admin-features/content-lifecycle-management/03-disposition-overview.md) garantit que les tableaux sont conservés uniquement aussi longtemps que nécessaire et sont automatiquement mis à la Corbeille après une période d'inactivité. À partir de là, les paramètres standards de la corbeille déterminent qui peut restaurer les tableaux et quand ils seront supprimés définitivement, soutenant la conformité, l'efficacité opérationnelle et la sécurité des données.
- **Gestion des clés de chiffrement****(EKM)** **:** [EKM](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md) offre un contrôle centralisé sur les clés de chiffrement, permettant aux organisations de surveiller les activités liées aux clés et de révoquer l'accès lorsque nécessaire, assurant ainsi une couche supplémentaire de sécurité des données.
