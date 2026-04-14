---
title: "Aper\xE7u de la classification automatique et sc\xE9narios"
article_id: 15431302000914
translation_id: 15431302000914
locale: fr
sidebar_position: 2
created_at: '2023-11-29T16:42:42Z'
updated_at: '2025-11-25T15:39:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Pour vous aider à protéger votre contenu sensible, Enterprise Guard inclut la fonctionnalité de classification automatique des données, qui classe les tableaux Miro en fonction du niveau de sensibilité de leur contenu. La classification automatique représente une avancée significative dans la façon dont vous gérez et protégez vos données sensibles. L’automatisation du processus de classification permet à votre organisation de renforcer la sécurité des données, de respecter les exigences réglementaires et de fournir une meilleure expérience d’administration de la sécurité. Le passage d’une classification manuelle à une classification automatique est une étape stratégique vers un cadre de sécurité des données plus précis, plus sécurisé et plus efficace.

## Comprendre les scénarios de classification automatique

### Prérequis

Pour utiliser la fonctionnalité de classification automatique, vous devez :

- [activer la découverte des données](../data-discovery/13-activate-privacy-related-data-discovery.md) ;
- [définir les niveaux de classification](07-define-classification-levels.md).

### Exemple de configuration de la classification automatique et des garde-fous

Vous devez [configurer la classification automatique et les garde-fous](https://help.miro.com/hc/articles/15853672236946) en fonction de vos exigences de sécurité et de gouvernance. Le tableau suivant répertorie la configuration utilisée pour tous les exemples de scénarios de cette page et n’est destiné qu’à des fins explicatives.

|  |  |  |  |
| --- | --- | --- | --- |
| **Classification de tableau** | **Degré de sensibilité** | **Critères de classification automatique** | **Garde-fous** |
| PUBLIC | 1  (le moins sensible) | Aucun | Aucun |
| INTERNE (par défaut) | 2 | TÉLÉCOM | - Blocage du partage public |
| CONFIDENTIEL | 3 | RGPD  PCI DSS | - Blocage du partage public  - Blocage du partage avec des équipes |
| RESTREINT | 4 (le plus sensible) | HIPAA  IDENTIFIANTS | - Blocage du partage public  - Blocage du partage avec des équipes  - Blocage du partage avec l’organisation |

*Tableau 1 : exemple de configuration destiné uniquement à des fins explicatives.*

## Mise à jour manuelle de la classification du tableau pour remplacer la classification automatique

Seuls les propriétaires, copropriétaires ou éditeurs du tableau peuvent mettre à jour sa classification pour remplacer le niveau attribué par la classification automatique. Si le propriétaire, les copropriétaires ou les éditeurs du tableau mettent à jour sa classification pour lui attribuer un niveau moins sensible, ils doivent sélectionner ou fournir une raison pour le changement, et cette information est ajoutée aux journaux d’audit.

### Mise à jour manuelle de la classification vers un niveau de sensibilité inférieur

**Scénario**
Imaginez un scénario dans lequel John Smith est propriétaire d’un tableau qui a été classé automatiquement comme **Confidentiel**, soit un degré de sensibilité de **3** selon notre configuration.

John examine les informations et décide de mettre à jour le niveau de classification pour le passer à **Interne**, dont le degré de sensibilité est de **2**, soit inférieur à celui attribué par la classification automatique (**3** pour **Confidentiel**).

:::note
Seuls les propriétaires, copropriétaires ou éditeurs du tableau peuvent mettre à jour manuellement le niveau de classification.
:::

**Résultat**

John étant propriétaire du tableau, il est en mesure de mettre à jour sa classification pour passer à un niveau de sensibilité inférieur (niveau **2** pour **Interne**). Dans ce scénario, John est invité à expliquer pourquoi il souhaite modifier le niveau de classification du tableau pour le rendre moins sensible (figure 1). John peut sélectionner la raison et cliquer sur **Mettre à jour**.

Le niveau de classification du tableau est mis à jour et les informations relatives à ce changement sont ajoutées aux journaux d’audit.

### Mise à jour manuelle de la classification vers un niveau de sensibilité supérieur

**Scénario**

Imaginez un scénario dans lequel John Smith est propriétaire d’un tableau qui a été classé automatiquement comme **Confidentiel**, soit un degré de sensibilité de **3** selon notre configuration.

John examine les informations et décide de mettre à jour le niveau de classification pour le passer à **Restreint**, dont le degré de sensibilité est de **4** (le plus élevé), soit supérieur à celui attribué par la classification automatique (**3** pour **Confidentiel**).

:::note
Seuls les propriétaires, copropriétaires ou éditeurs du tableau peuvent mettre à jour manuellement le niveau de classification.
:::

**Résultat**

John étant propriétaire du tableau, il est en mesure de mettre à jour sa classification pour passer à un niveau de sensibilité supérieur.

Le tableau suivant résume les différents scénarios et leurs résultats, sachant que le tableau a été classé automatiquement à un moment donné puis qu’une personne propriétaire, copropriétaire ou éditrice a mis à jour la classification manuellement à une date ultérieure.

|  |  |  |
| --- | --- | --- |
| **Niveau de classification automatique** | **Action du propriétaire du tableau** | **Nouveau niveau de classification** |
| CONFIDENTIEL | **Mise à jour vers un niveau de classification inférieur**  John, le propriétaire du tableau, met à jour manuellement la classification du tableau vers  **INTERNE**, soit un degré de sensibilité de 2, c’est-à-dire inférieur à celui attribué par la classification automatique (CONFIDENTIEL, niveau 3). | John étant propriétaire du tableau, il est en mesure de mettre à jour sa classification pour passer à un niveau de sensibilité inférieur, **INTERNE**.  Dans ce scénario, la personne propriétaire du tableau est invitée à expliquer pourquoi elle souhaite en modifier le niveau de classification pour le rendre moins sensible. John peut sélectionner la raison et cliquer sur **Mettre à jour**.  Le niveau de classification du tableau est mis à jour sur **INTERNE** et les informations relatives à ce changement sont ajoutées aux journaux d’audit. |
| CONFIDENTIEL | **Mise à jour vers un niveau de classification supérieur**  John, le propriétaire du tableau, décide de mettre à jour sa classification vers **RESTREINT**, qui présente le niveau de sensibilité le plus élevé (4), soit un niveau supérieur à celui attribué par la classification automatique (CONFIDENTIEL, niveau 3). | John étant propriétaire du tableau, il est en mesure de mettre à jour sa classification pour passer à un niveau de sensibilité supérieur. |

*Tableau 2 : scénarios et niveaux de classification automatique résultants*

## Mise à jour automatique de la classification du tableau

Le cycle de découverte des données s’effectue toutes les heures. Si le contenu d’un tableau est modifié, avec l’ajout ou la suppression de données hautement sensibles, le tableau concerné est de nouveau classifié automatiquement, en fonction du contenu mis à jour et du niveau de classification non automatique le plus récent. Les sections suivantes fournissent des exemples de scénarios de mises à jour automatiques du niveau de classification.

### Données hautement sensibles supprimées du tableau

Après le cycle de découverte des données suivant, la classification du tableau est automatiquement mise à jour pour correspondre au niveau de sensibilité applicable.

**Exemple de contenu du tableau dans ce scénario**

Le tableau contient des données hautement sensibles correspondant aux badges de sensibilités suivants : IDENTIFIANTS, HIPAA, RGPD, PCI DSS. Une fois le cycle de découverte des données terminé, la classification automatique a donc classé ce tableau comme **RESTREINT**, niveau 4, soit le degré de sensibilité le plus élevé selon notre exemple de configuration de la classification automatique. Le tableau qui suit décrit les informations suivantes :

- **Dernière classification non automatique :** il s’agit de la classification non automatique du tableau la plus récente. Elle peut avoir été effectuée [manuellement](03-auto-classification-overview-and-scenarios.md), via une [classification par défaut](../data-security/02-data-classification.md), ou par les API de [mise à jour](https://developers.miro.com/reference/enterprise-dataclassification-board-set)/[mise à jour par lot de la classification du tableau](https://developers.miro.com/reference/enterprise-dataclassification-team-boards-bulk).

- **Classification automatique :** niveau de classification appliqué automatiquement au tableau suite au cycle de découverte des données.

- **Mesure prise :** mesure prise et mises à jour apportées au contenu du tableau, après la classification automatique.

- **Nouvelle classification :** nouvelle classification compte tenu des mesures prises et de tous les autres aspects, tels que le contenu du tableau et la dernière classification non automatique.

|  |  |  |  |
| --- | --- | --- | --- |
| **Dernière classification non automatique** | **Classification automatique** | **Action de l’utilisateur** | **Nouveau niveau de classification automatique** |
| INTERNE (via la classification par défaut du tableau) | RESTREINT | Toutes les données sensibles ont été supprimées du tableau. | Une fois le cycle de découverte des données suivant terminé, la classification du tableau est automatiquement mise à jour vers **INTERNE**, car il ne comporte plus d’informations sensibles, mais la classification non automatique précédente (causée par la classification par défaut) était INTERNE. |
| CONFIDENTIEL | RESTREINT | Toutes les données sensibles ont été supprimées du tableau. | Une fois le cycle de découverte des données suivant terminé, la classification du tableau est automatiquement mise à jour vers **CONFIDENTIEL** (degré de sensibilité de 3), même s’il ne comporte plus d’informations sensibles, car le niveau de classification non automatique précédent était CONFIDENTIEL (niveau 3). |
| NON CLASSÉ | RESTREINT | Le contenu IDENTIFIANTS et HIPAA, de niveau RESTREINT (degré de sensibilité 4), est effacé du tableau. | Après le cycle de découverte des données suivant, la classification du tableau est automatiquement mise à jour vers **CONFIDENTIEL**, niveau de sensibilité 3, car : - le tableau ne contient plus d’informations IDENTIFIANTS et HIPAA, mais il contient toujours des données sensibles PCI DSS, qui correspondent au niveau **CONFIDENTIEL** ; - le tableau n’était pas classifié avant la classification automatique. |
| RESTREINT | RESTREINT | Le contenu IDENTIFIANTS et HIPAA, de niveau RESTREINT (degré de sensibilité 4), est effacé du tableau. | Une fois le cycle de découverte des données suivant terminé, le tableau reste au niveau **RESTREINT** (degré de sensibilité 4), même s’il ne comporte plus d’informations de type IDENTIFIANTS et HIPAA, car le niveau de classification non automatique précédent était RESTREINT (niveau 4). |
| NON CLASSÉ | RESTREINT | Toutes les données sensibles ont été supprimées du tableau. | Une fois le cycle de découverte des données suivant terminé, la classification du tableau est automatiquement mise à jour vers **NON CLASSÉ**, car il ne comporte plus d’informations sensibles et n’était pas classé avant la classification automatique. |

*Tableau 3 : scénarios et niveaux de classification automatique résultants*

### Données hautement sensibles ajoutées au tableau

Une fois le cycle de découverte des données suivant terminé, la classification du tableau est automatiquement mise à jour vers le niveau de sensibilité applicable en fonction du plus haut degré de sensibilité des données trouvé.

|  |  |  |
| --- | --- | --- |
| **Niveau de classification automatique le plus récent** | **Action de l’utilisateur** | **Nouveau niveau de classification automatique** |
| PUBLIC | Un collaborateur a ajouté un numéro de carte bancaire. | **CONFIDENTIEL** PCI DSS |
| INTERNE | Un collaborateur a ajouté un jeton d’authentification. | **RESTREINT** IDENTIFIANTS |
| RESTREINT | Un collaborateur a ajouté un jeton d’authentification. | **RESTREINT** Reste inchangé. |
| INTERNE | Un collaborateur a ajouté un numéro de permis de conduire allemand. | **CONFIDENTIEL**  RGPD |
| CONFIDENTIEL | Un collaborateur a ajouté une adresse MAC. | **RESTREINT**  IDENTIFIANTS |

*Tableau 4 : scénarios et niveaux de classification automatique résultants*
