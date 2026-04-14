---
title: "Aper\xE7u des garde-fous intelligents"
article_id: 14375998880018
translation_id: 14375998880018
locale: fr
sidebar_position: 0
created_at: '2023-10-12T12:35:03Z'
updated_at: '2025-11-25T16:22:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Les éléments du tableau Miro peuvent contenir des données privées et réglementaires (telles que PII, PHI, PCI) ou un contenu d'affaires confidentiel critique (comme des informations financières, des informations RH, une PI, des secrets commerciaux). Après la découverte de données et la classification automatique, les organisations doivent mettre en place des contrôles proactifs essentiels pour maintenir la confidentialité, la sécurité et la conformité continue avec les réglementations pertinentes.

- Avec les garde-fous, vous pouvez désormais appliquer automatiquement des contrôles proactifs, tels que :
  Restreindre automatiquement les capacités de partage à différents niveaux (public, équipe, organisation) en fonction du contenu du tableau et du niveau de classification.
- Restreindre la réplication du contenu.
- Bloquer l'utilisation de Miro IA pour empêcher les interactions basées sur l'IA avec des données sensibles ou classées.

Ces contrôles proactifs garantissent la confidentialité et la conformité sans entraver les activités de l'entreprise.

Les admins ont deux options pour déployer les Garde-fous Intelligents dans leur organisation :
- **Mode par défaut :** Par défaut, les garde-fous n'affectent pas les options de partage actives sur les tableaux afin d'éviter de perturber la collaboration en cours, même lorsque les tableaux sont reclassés lors de la classification automatique.

- **Mode strict :** Lorsque le commutateur **Appliquer les garde-fous en mode strict** est activé, les garde-fous remplacent toutes les options de partage actives. Cela offre aux admins les niveaux de contrôle les plus stricts, mais cela peut également entraîner la perte immédiate d'accès au tableau pour certains utilisateurs.

Considérez un scénario où vous avez configuré des garde-fous pour garantir que les utilisateurs de tableaux classés comme CONFIDENTIEL ne soient pas autorisés à partager le tableau avec le public, à partager avec des équipes, à partager avec l'organisation ou à reproduire du contenu. Quelqu'un dans votre organisation a créé un nouveau tableau nommé Plan Financier, a ajouté quelques chiffres de revenus et a assigné le niveau de classification *CONFIDENTIEL* à ce tableau. Les réglages des garde-fous sont automatiquement appliqués et tous les utilisateurs ne peuvent pas partager le tableau, et tous les utilisateurs sauf le propriétaire du tableau ne peuvent pas reproduire le contenu (Figure 2).

Pour plus d'informations sur chaque garde-fou, leurs descriptions et les utilisateurs concernés, consultez la [documentation de référence sur les garde-fous](02-guardrails-reference.md).
