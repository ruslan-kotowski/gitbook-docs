---
title: Connecter les outils avec Zapier
article_id: 30124629305106
translation_id: 30124629305106
locale: fr
sidebar_position: 2
created_at: '2025-10-10T11:48:03Z'
updated_at: '2025-10-14T12:37:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Connectez Miro Insights à des centaines d'outils via [Zapier](http://zapier.com/) pour capturer automatiquement les avis et les données de sources qui n'ont pas d'intégrations directes. Cela vous permet de centraliser les insights clients de l'ensemble de votre pile technologique.

L'intégration Zapier vous permet de :

- Créer automatiquement des éléments de feedback à partir de tickets du service d’assistance, d'enquêtes ou de conversations de chat.
- Capturer des données à partir de n'importe quel outil pris en charge par Zapier, même si Miro Insights n'a pas d'intégration directe.
- Réduire la saisie manuelle des données en configurant des workflows automatisés.

## Créer des feedbacks

Zapier propose deux actions principales pour créer des éléments de feedback dans Miro Insights.

### Créer des feedbacks

L’action standard pour créer des éléments de feedback généraux dans Miro Insights avec les champs suivants :

- **Titre du feedback** : Bref résumé du feedback.
- **Contenu** : Contenu détaillé ou description du feedback.
- **Nom du reporter** : Nom de la personne fournissant le feedback.
- **Email du reporter** : Adresse e-mail de la personne fournissant le feedback.
- **Email du propriétaire** : Propriétaire interne ou assigné pour le feedback.
- **Date et heure fournies** : Quand le feedback a été donné initialement.
- **URL d'origine** : Lien vers la source originale (ticket, réponse à un sondage, etc.).
- **Nom de l'entreprise** : Organisation associée au retour.
- **Domaine de l'entreprise** : Domaine du site web de l'entreprise.

### Créer un feedback (Appel)

Une action spécialisée conçue spécifiquement pour capturer des retours provenant d'appels et de conversations avec ces champs :

- **Titre de l'appel** : Titre ou sujet de l'appel.
- **Transcription de l'appel** : Transcription complète ou notes de l'appel.
- **URL d'origine** : Lien vers l'enregistrement de l'appel ou les détails de la réunion.
- **Participants** : Informations sur les participants à l'appel.
  - **Adresse e-mail** : Adresse e-mail du participant.
  - **Nom** : Nom du participant.
- **Adresse e-mail du propriétaire** : Propriétaire interne ou responsable du feedback de l'appel.
- **Date et heure de début** : Quand l'appel a eu lieu.
- **Nom de l'entreprise** : Organisation associée à l'appel.
- **Domaine de l'entreprise** : Domaine du site web de l'entreprise.

## Configuration de l'intégration Zapier

Pour commencer avec Zapier et Miro Insights, suivez ces étapes.

### Prérequis

- Compte Miro Insights actif
- Compte Zapier (gratuit ou payant)
- Accès à l'outil source que vous souhaitez connecter

### Démarrage rapide avec des modèles

Miro Insights propose des modèles Zapier préconfigurés pour des outils d'intelligence conversationnelle populaires, tels que Grain, Fathom et Fireflies.

Pour configurer un Zap à l'aide d'un modèle :

1. Accédez aux paramètres de Miro Insights > à la section **Intégrations & Automatisations**.
2. Sélectionnez votre outil de conversation. Par exemple, Grain.
3. Connectez-vous à Zapier, si nécessaire.
4. Connectez votre compte **Grain**.
5. Cartographiez les champs de Grain vers les champs de Miro Insights.
6. Testez et activez l'intégration préconfigurée.

Les modèles offrent une configuration plus rapide grâce à une cartographie optimisée des champs pour chaque outil spécifique, ce qui facilite grandement la capture des retours clients issus de vos conversations enregistrées.

### Configuration de base

1. **Créez un nouveau Zap** dans votre tableau de bord Zapier.
2. Choisissez votre **application de déclenchement**. L'outil d'où les retours proviennent.
3. Sélectionnez **Miro Insights** comme votre application d'action.
4. Choisissez votre **événement d'action** :
   - **"Créer un feedback"** pour les éléments de feedback généraux.
   - **"Créer un feedback (Appel)"** pour le feedback spécifique aux appels.
5. Connectez votre **compte Miro Insights** lorsque cela est demandé.
6. **Cartographiez les champs** de votre application de déclenchement vers les champs de Miro Insights.
7. Testez l'intégration pour vous assurer que les données circulent correctement.
8. **Activez le Zap** pour commencer la collecte automatisée de données.

### Meilleures pratiques de cartographie de champs

Lors de la cartographie des champs de votre outil source vers Miro Insights, considérez les pratiques recommandées suivantes pour garantir une capture de données de haute qualité.

**Champs obligatoires :**

- **Titre du feedback**: Utilisez des titres clairs et descriptifs issus de vos données sources.
- **Contenu**: Cartographiez le contenu principal du feedback ou combinez plusieurs champs.

**Champs recommandés :**

- **Informations sur le rapporteur** : Capturez les coordonnées du client si disponibles.
- **Données de l'entreprise** : Essentielles pour la gestion de produit basée sur le compte.
- **URL d'origine** : Maintenez la traçabilité jusqu'aux sources originales.
- **Date fournie** : Utilisez la date réelle du feedback, pas la date de traitement.

**Conseils pour la cartographie des champs :**

- Utilisez les outils de formatage de Zapier pour combiner plusieurs champs sources.
- Incluez le nom de l'outil source dans le titre ou le contenu pour plus de clarté.
- Utilisez des formats cohérents pour les dates, les noms de société et les catégories.
- Définissez des valeurs par défaut pour les champs optionnels.
