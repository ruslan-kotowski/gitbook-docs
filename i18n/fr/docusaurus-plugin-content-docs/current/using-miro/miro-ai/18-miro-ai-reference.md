---
title: Référence Miro IA
article_id: 20970362792210
translation_id: 20970362792210
locale: fr
sidebar_position: 18
created_at: '2024-08-26T09:34:26Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: comments
availability:
  notes: 'Qui peut le faire: Tous les utilisateurs Quels forfaits: Free, Starter,
    Business, Enterprise, Education Quelles plateformes: Navigateur, Bureau, Mobile'
---

Cet article de référence décrit les fonctionnalités de Miro IA.

## Modèles de Miro IA

Les modèles sont généralement hébergés sur l'infrastructure du fournisseur, ou sur le service Azure AI de Microsoft ou AWS Bedrock. Pour les clients qui achètent Miro via AWS Marketplace, tous les modèles sont hébergés sur AWS Bedrock.

### Création et itération assistées par l'IA

| **Fonctionnalité Miro IA** | **Description** | **Modèle** |
| --- | --- | --- |
| Résumés de conversations | Génère un résumé des fils de commentaires longs sur votre tableau Miro. | GPT 4o-mini |
| Créer un diagramme - Organigramme | Crée un organigramme à partir d'un prompt utilisateur et du contenu sélectionné du tableau. | GPT-4o |
| Modifier le diagramme - Flux | Modifie un flux à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | GPT-4o |
| Créer un diagramme - Carte mentale | Crée une carte mentale à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | GPT 4o-mini |
| Modifier le diagramme - Carte mentale | Modifie une carte mentale à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | GPT-4o |
| Créer un diagramme - ERD | Crée un diagramme de relation d’entité (ERD) à partir d’un prompt saisi par l’utilisateur. Une option **Créer avec l’IA**. | GPT 4o-mini |
| Modifier le diagramme - ERD | Modifie un ERD à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | GPT-4o |
| Numériser le diagramme | Transforme les images de diagrammes dessinés à la main en diagrammes entièrement éditables dans Miro. | Claude 3.7 Sonnet (AWS Bedrock) |
| Créer un document | Crée un document Miro à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. Une option **Créer avec l'IA**. | GPT-4o |
| Modifier un document | Modifie un document Miro à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | GPT-4o |
| Créer une image | Crée une image à partir d’un prompt saisi par l’utilisateur, y compris des objets sur le tableau pour le contexte. Une option de **Création avec l’IA**. | Segmind Stable Diffusion 1B (SSD-1B) + StabilityAI Diffusion XL Refiner 1.0 |
| Modifier l'image | Modifie une image à partir d’un prompt saisi par l’utilisateur, incluant des objets sur le tableau comme contexte. Une option **Créer avec l’IA**. | GPT-4o |
| Convertir l'image en prototype | Convertit une esquisse ou une image de prototype en un Miro Prototype modifiable. | Modèle propriétaire Miro + Claude 3.7 Sonnet |
| Texte alternatif de l’image | Génère du texte alternatif pour une image. Ne consomme pas de crédit d’IA. | Modèle propriétaire de Miro |
| Créer des pense-bêtes | Crée des pense-bêtes Miro à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | GPT-4o |
| Modifier les pense-bêtes | Modifie les pense-bêtes Miro à partir d’un tableau utilisateur et du contenu sélectionné sur le tableau. | GPT-4o |
| Capture de pense-bêtes | Convertit une image de pense-bêtes physiques en pense-bêtes Miro. | Modèle propriétaire Miro |
| Créer un prototype | Crée un prototype Miro à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | GPT-4o + Claude 4.5 Sonnet + GPT 4o-mini + Gemini 2.5 Flash Image (nano-banana) |
| Modifier l’écran du prototype | Modifie l’écran d’un prototype Miro à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | Claude 4.5 Sonnet + Gemini 2.5 Flash Image (nano-banana) |
| Supprimer l’arrière-plan | Supprime l'arrière-plan d'une image. | Modèle propriétaire de Miro |
| Dessins intelligents | Convertit un dessin au crayon en ligne, en forme ou en pense-bête. | Modèle propriétaire de Miro |
| Créer une table | Crée une table Miro à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | Claude 3.7 Sonnet |
| Modifier une table | Modifie une table Miro à partir d’un prompt saisi par l’utilisateur et du contenu sélectionné sur le tableau. | Claude 3.7 Sonnet |

### Partenaires d'IA

|  |  |  |
| --- | --- | --- |
| **Fonctionnalité Miro IA** | **Description** | **Modèle** |
| Partenaire d’IA - coach Agile | Identifie les thèmes clés d'une rétrospective et suggère les prochaines étapes. | GPT-4o |
| Partenaire d’IA - Responsable de produit | Fournit des avis et suggestions sous forme de commentaires sur les cadres, pense-bêtes ou texte. Propose aussi des solutions sous forme de pense-bêtes. | GPT-4o |
| Partenaire d’IA - Alliance marketing produit | Fournit des avis et suggestions sous forme de commentaires sur les cadres, pense-bêtes ou texte. | GPT-4o |

### Regroupement piloté par l’IA

| **Fonctionnalité Miro IA** | **Description** | **Modèle** |
| --- | --- | --- |
| Catégorisation des pense-bêtes par mots-clés | Regroupe les pense-bêtes en ensembles par mot-clé, avec un titre pour chaque ensemble. | Claude 3.5 Haiku + Amazon Nova Micro |
| Catégorisation des pense-bêtes par sentiment | Regroupe les pense-bêtes par sentiment, comme les opinions et les points de vue, en ensembles positifs, neutres et négatifs. | Claude 3.5 Haiku |

### Édition de texte par l'IA

Le tableau suivant montre l'édition de texte propulsée par Miro IA :

|  |  |  |
| --- | --- | --- |
| **Fonctionnalité Miro IA** | **Description** | **Modèle** |
| Modifier le ton | Modifiez le ton du texte sélectionné pour le rendre amical, professionnel, commercial ou léger. | GPT-5 nano |
| Corriger la grammaire et l'orthographe | Corrige l’orthographe et la grammaire du texte sélectionné. | GPT-5 |
| Réécrire pour plus de clarté | Réécrit le texte sélectionné pour plus de clarté. | GPT-5 Chat |
| Raccourcir le texte | Reformule le texte sélectionné en une version plus courte sans perdre en clarté ni en lisibilité. | GPT-5 mini |
| Traduire | Traduit le texte sélectionné en anglais, espagnol, allemand, français, japonais, portugais, coréen, polonais, italien, turc, arabe, russe, danois, finnois, norvégien, néerlandais, suédois ou thaïlandais. Vous pouvez traduire des objets uniques ou multiples simultanément. | GPT-5 mini |

### Cartes mentales alimentées par l'IA

| **Fonctionnalité Miro IA** | **Description** | **Modèle** |
| --- | --- | --- |
| Générer une carte mentale | Génère une carte mentale à partir d'un nœud racine sélectionné. | GPT 4o-mini |
| Carte mentale - Développer avec des idées | Génère des idées à partir d'un nœud racine ou d'un nœud enfant sélectionné. | GPT 4o-mini |
| Carte mentale - Développer avec des sujets | Génère des sujets à partir d’un nœud racine ou d’un nœud enfant sélectionné. | GPT 4o-mini |
| Carte mentale - Développer avec des questions | Génère une question à partir d’un nœud racine ou d’un nœud enfant sélectionné. | GPT 4o-mini |

### Diapositives enrichies par l’IA

Les Diapositives Miro utilisent les modèles suivants :

- Amazon Titan
- Claude 4 Sonnet
- Claude 3.7 Sonnet
- Claude 3.5 Sonnet
- GPT-5
- GPT-4o
- Stable Diffusion 3.5 Large
- Stability Image Core

### Miro Insights

Pour synthétiser les retours des clients, [Miro Insights](https://help.miro.com/hc/articles/25438311770770) utilise GPT-4o.

### Clients AWS Marketplace

**Modèles AWS Marketplace**

| **Fonctionnalité Miro IA** | **Modèle** |
| --- | --- |
| Résumés de conversation | Claude Haiku 3.7 (AWS Bedrock) |
| Créer un diagramme – Graphique de flux | Claude Sonnet 3.7 (AWS Bedrock) |
| Modifier le diagramme – Graphique de flux | Claude Sonnet 3.7 (AWS Bedrock) |
| Créer un diagramme – Carte mentale | Claude Sonnet 3.7 (AWS Bedrock) |
| Modifier un diagramme – Carte mentale | Claude Sonnet 3.7 (AWS Bedrock) |
| Créer un diagramme – DER | Claude Sonnet 3.7 (AWS Bedrock) |
| Modifier le diagramme – MRD | Claude Sonnet 3.7 (AWS Bedrock) |
| Créer un document | Claude Sonnet 3.7 (AWS Bedrock) |
| Modifier le document | Claude Sonnet 3.7 (AWS Bedrock) |
| Créer des pense-bêtes | Claude Sonnet 3.7 (AWS Bedrock) |
| Modifier les pense-bêtes | Claude Sonnet 3.7 (AWS Bedrock) |
| Capture de pense-bêtes | Claude Sonnet 3.7 (AWS Bedrock) + modèle propriétaire de Miro |
| Créer une image | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Modifier une image | Claude Haiku 3.7 (AWS Bedrock) + Bedrock Stability SD3.5 Large V1 |
| Texte alternatif de l'image | Claude Sonnet 3.7 (AWS Bedrock) |
| Créer un prototype | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Modifier l'écran du prototype | Claude Sonnet 3.7 (AWS Bedrock) + Bedrock Stability Image Core |
| Convertir l'image en prototype | Claude Sonnet 3.7 + Miro proprietary model |
| Créer une table | Claude Sonnet 3.7 (AWS Bedrock) |
| Modifier la table | Claude Sonnet 3.7 (AWS Bedrock) |
| Numériser le diagramme | Claude Sonnet 3.7 (AWS Bedrock) |
| Catégorisation des pense-bêtes par mots-clés | Claude Sonnet 3.7 (AWS Bedrock) + modèle propriétaire Miro |
| Catégorisation des pense-bêtes par sentiment | modèle propriétaire Miro |
| Partenaires d’IA | Claude Sonnet 3.7 (AWS Bedrock) |
| Édition de texte alimentée par l'IA | Claude Sonnet 3.7 (AWS Bedrock) |
| Cartes mentales alimentées par l'IA | Claude Sonnet 3.7 (AWS Bedrock) |

## Sélectionnez votre propre modèle

Les listes suivantes indiquent quels modèles sont disponibles avec [Choisissez votre modèle](10-select-your-own-model-beta.md), disponible pour les [flux](04-flows-overview.md) et les partenaires d’IA.

### Les grands modèles de langage

**Claude**

- Claude 3.7 Sonnet
- Claude Sonnet 4

**OpenAI**

- GPT-4o
- GPT-4o mini
- OpenAI o4-mini
- GPT-5
- GPT-5 mini
- GPT-4.1
- GPT-4.1 mini

### Modèles d'images

**Stability AI**

- Stable Image Core
- Stable Image Ultra
- Stable Diffusion 3.5 Large

**Amazon**

- Générateur d'images Titan d'Amazon
- Canevas Nova d'Amazon

**Google**

- Image flash Gemini 2.5 (Nano Banana)
- Vertex AI Imagegen 3
- Vertex AI Imagegen 3 Rapide
- Vertex AI Imagegen 4

## Crédits d’IA Miro et module complémentaire

Miro attribue un nombre défini de crédits d’IA à votre compte chaque mois. Le nombre de crédits attribués dépend de votre forfait. Votre allocation est réinitialisée le premier jour de chaque mois civil.

Pour chaque action d’IA que vous effectuez, vous consommez des crédits d’IA. La plupart des actions d’IA consomment un (1) crédit par action, mais certaines fonctionnalités peuvent en consommer davantage.

Pour augmenter votre allocation de crédits d’IA, vous pouvez souscrire à un abonnement supplémentaire de crédits d’IA Miro. Pour en savoir plus, consultez [Crédits d’IA Miro et module complémentaire d’IA](../../plans-billing/billing-and-payments/03-miro-ai-credits.md).

## Confidentialité et sécurité de Miro IA

À partir du 3 février 2025, Miro collectera des données d'interaction d'IA des utilisateurs du forfait Free pour améliorer les fonctionnalités de Miro IA telles que les résumés par IA, les diagrammes et les partenaires d’IA.

Pour en savoir plus sur la manière dont Miro utilise les interactions d’IA pour améliorer Miro IA, et comment vous pouvez contrôler vos préférences de données, consultez [Améliorations de qualité de Miro IA](19-miro-ai-quality-improvements.md).
