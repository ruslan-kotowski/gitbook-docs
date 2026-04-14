---
title: "Configurer une int\xE9gration Looker"
article_id: 25112862440978
translation_id: 25112862440978
locale: fr
sidebar_position: 4
created_at: '2025-03-05T14:00:46Z'
updated_at: '2025-06-04T08:30:26Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: looker
---

:::note
Pour des documents administratifs complets avec des détails et des informations supplémentaires sur l'intégration Miro + Looker, veuillez vous référer à la [documentation de Looker pour les administrateurs](https://docs.google.com/document/d/1AUCQWRwDICLygwVmwSxXpz7RmRivPit0EIKgBMIkT6A/edit?usp=sharing).
:::

Pour configurer une intégration **Looker** avec Miro, vous devez enregistrer l'application OAuth dans Looker.

## Prérequis

- Assurez-vous qu'un **admin d'entreprise** a approuvé Looker pour votre organisation Miro.

## Enregistrer une application OAuth dans Looker

1. Dans le **Looker Marketplace**, trouvez et sélectionnez l'extension **API Explorer**.
2. Sélectionner **Installer**.
3. Allez à **Accueil** > **Applications** > **Extension API**.
4. Trouver et sélectionner **Enregistrer l'application OAuth**.
5. Sélectionner **Exécuter**.
6. Un menu s'ouvre où vous pouvez ajouter des données de demande.
   Ajoutez les valeurs suivantes :
   - **guid_client**: `15609152-a12a-4fa1-b364-337e7896d25d`
   - **corps** :

   ```
     "redirect_uri": "https://integrations.miro.com/api/contenthub/public/oauth/callback",
     "nom d'affichage" Miro
     Description Intégration Miro Looker
     "activé": true,
     "group_id": ""
   }
   ```
7. Sélectionner **Je comprends que ce point de terminaison API modifiera les données**.
8. Sélectionner **Exécuter**.
9. Une exécution réussie retourne le corps avec un code de réponse **HTTP 200**.
   - 💡 Si le corps retourné inclut `"enabled":false`, exécutez l'API Update OAuth App avec les mêmes valeurs qu'à l'étape 6.

Vous avez réussi à configurer une intégration Looker avec Miro.

## En savoir plus

- Voir la [référence de l'API Looker](https://developers.looker.com/api/explorer/4.0/methods/Auth/register_oauth_client_app) (externe).
