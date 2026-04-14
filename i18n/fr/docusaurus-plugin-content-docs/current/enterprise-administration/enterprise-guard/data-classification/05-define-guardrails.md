---
title: "D\xE9finir les garde-fous"
article_id: 16494716849810
translation_id: 16494716849810
locale: fr
sidebar_position: 4
created_at: '2024-01-19T19:01:45Z'
updated_at: '2025-11-25T15:40:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Définir les garde-fous est la troisième étape du flux de configuration de la classification automatique et des garde-fous. À cette étape du processus, vous allez configurer les garde-fous, qui sont les restrictions applicables à chaque niveau de classification, telles que bloquer le partage public, bloquer le partage avec les équipes, bloquer le partage avec l'organisation ou bloquer la réplication de contenu. Par exemple, vous pouvez configurer des garde-fous pour bloquer le partage public, bloquer le partage avec les équipes, bloquer le partage dans l’organisation, et bloquer la réplication du contenu pour les utilisateurs de tableaux classés comme CONFIDENTIELS.

### Prérequis

- Vous devez compléter la première et la deuxième étape du processus d'auto-classification et de garde-fous, [1: Définir les niveaux de classification](07-define-classification-levels.md) et [2: Définir la classification automatique](07-define-classification-levels.md).
- Vous devez connaître les garde-fous que vous souhaitez attribuer à chaque niveau de classification en fonction de vos exigences en matière de sécurité et de gouvernance.
- Vous devez disposer du [rôle d’admin de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.

Les admins ont deux options pour déployer les Garde-fous intelligents au sein de leur organisation :
**Mode par défaut :** Par défaut, les garde-fous n'affectent pas les options de partage actives sur les tableaux pour éviter de perturber la collaboration en cours, y compris lorsque les tableaux sont reclassés lors de l'auto-classification.

- **Mode strict :** Lorsque le basculement Appliquer les garde-fous en mode strict est activé, les garde-fous prennent le pas sur toutes les options de partage actives. Cela offre aux Admins les niveaux de contrôle les plus stricts, mais peut également entraîner la perte immédiate de l'accès aux tableaux pour certains utilisateurs.

![garde-fous.png](images/26201253165970_guardrails.png)

## Attribuer des garde-fous

Pour attribuer des garde-fous à un niveau de classification, procédez comme suit :

1. Sur la page **Définir des garde-fous**, cliquez sur l'icône **Modifier** du niveau de classification pour lequel vous souhaitez attribuer les garde-fous. Par exemple, si vous souhaitez attribuer des garde-fous au niveau de classification CONFIDENTIEL, cliquez sur l'icône de modification sur la ligne du niveau de classification CONFIDENTIEL.
2. Sélectionnez la case à cocher pour chaque étiquette de garde-corps que vous souhaitez attribuer à ce niveau de classification. Par exemple, si vous souhaitez bloquer le partage public, bloquer le partage avec les équipes, bloquer le partage avec l'organisation, bloquer la réplication du contenu pour les utilisateurs des tableaux classés comme CONFIDENTIEL, bloquer le partage en dehors des domaines autorisés et bloquer l'utilisation de Miro AI, sélectionnez les cases suivantes :
   - **Bloquer la réplication du contenu**- **Bloquer l’utilisation de Miro IA (Beta)**
   - **Bloquer le partage public**
   - **Bloquer le partage avec les équipes**
   **Bloquer le partage dans l’organisation**
   **- Bloquer le partage en dehors des domaines autorisés (Bêta)**
   Après avoir sélectionné cette case à cocher, vous devez ajouter les domaines que vous souhaitez autoriser en tapant et en sélectionnant dans la liste de domaines autorisés dans l'organisation, ou en tapant un nouveau domaine dans la case et en cliquant sur + **Ajouter**.
   Pour plus d'informations sur chaque contenu et garde-fou de partage, consultez [Aperçu et scénarios des Garde-Fous Intelligents](01-intelligent-guardrails-overview.md).
3. Par défaut, les garde-fous n’affectent pas les options de partage actives sur les tableaux afin de ne pas perturber la collaboration en cours, y compris lorsque les tableaux sont reclassifiés lors de la classification automatique.

   Si vous souhaitez appliquer des garde-fous et remplacer toutes les options de partage actives, activez le bascule **Appliquer les garde-fous en mode strict**. Cela peut entraîner la perte d'accès des utilisateurs aux tableaux. Cela offre aux administrateurs les niveaux de contrôle les plus stricts, mais peut également entraîner la perte immédiate de l'accès aux tableaux pour certains utilisateurs.
   ![garde-fous.png](images/26201253165970_guardrails.png)
4. Cliquez sur **Terminé**.
   Votre configuration est enregistrée, mais elle ne prendra effet qu'après avoir cliqué sur **Publier** sur la page [**Vérifier l'impact**](06-review-impact.md).
5. Une fois que vous avez terminé de définir les garde-fous pour les différents niveaux de classification, passez à la [Configuration complète des garde-fous](05-define-guardrails.md).

## Configuration complète des garde-fous

Après avoir terminé d'assigner des garde-fous pour différents niveaux de classification, cliquez sur **Suivant**. Votre configuration est enregistrée, mais elle ne prendra effet qu'après avoir cliqué sur **Publier** sur la page [Vérifier l'impact](06-review-impact.md).
