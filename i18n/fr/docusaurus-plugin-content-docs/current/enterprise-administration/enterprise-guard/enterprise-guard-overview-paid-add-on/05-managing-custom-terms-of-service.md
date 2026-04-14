---
title: "Gestion des conditions d\u2019utilisation personnalis\xE9es"
article_id: 27621616452882
translation_id: 27621616452882
locale: fr
sidebar_position: 3
created_at: '2025-06-24T23:29:13Z'
updated_at: '2025-11-04T14:10:40Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

## Créer des conditions d’utilisation personnalisées

:::note
Notes :

- Les admins doivent avoir les privilèges Enterprise Guard suivants pour consulter et gérer les Conditions d’utilisation personnalisées :
  - L'admin de contenu sensible dispose des autorisations intégrées.
  - Les rôles d’admin personnalisés doivent inclure :
    - Consulter les conditions d’utilisation personnalisées
    - Gérer les conditions d’utilisation personnalisées
- Les invités et les utilisateurs externes sont exclus.
- Miro ne stocke pas les conditions, seulement le lien et les métadonnées.
:::

1. Allez dans **Paramètres** > **Enterprise Guard** > **Conditions d’utilisation personnalisées**.
2. Si vous créez des conditions d’utilisation personnalisées pour la première fois, cliquez sur **Ajouter des conditions d’utilisation**.
   Si vous possédez déjà une configuration existante et souhaitez en ajouter une autre, cliquez sur **Créer nouveau** depuis la vue de liste.
3. Dans **Configuration** → **Conditions** :

- **Déclencheur** : Choisissez entre **Connexion réussie** ou **Utilisation de l’IA**.
  **Connexion réussie**

  - Le dialogue apparaît immédiatement après la connexion.
  - Les utilisateurs peuvent cliquer sur **Continuer** pour accepter et procéder, ou sur **Déconnexion**.

  **Utilisation de l’IA**

  - La boîte de dialogue apparaît lorsque l'utilisateur interagit avec Miro IA, comme pour basculer la mise en page IA, ouvrir le panneau latéral IA, ou démarrer un outil ou une action IA (par exemple, le partenaire d'IA).
  - Les utilisateurs peuvent cliquer sur **Continuer** pour accepter et utiliser les fonctionnalités IA. Si les utilisateurs cliquent sur **Annuler**, ils restent connectés et peuvent continuer à utiliser toutes les fonctionnalités non IA.
- **Périmètre**: **Tous les utilisateurs et admins de l’organisation**.
- **Période de récurrence** : entrez un nombre et sélectionnez **Jours**, **Semaines** ou **Mois**.Par défaut : deux semaines.
  Les utilisateurs ne seront pas sollicités à nouveau tant que la période de récurrence ne sera pas terminée ou que les conditions n'auront pas été mises à jour.

4. Dans **Paramétrer** → **Contenu** :
   - **Titre** (max 32 caractères)
   - **Description** (max 200 caractères)
   - **Lien :** Liens de politique (hébergés à l'extérieur). Pour inclure des liens supplémentaires, cliquez sur +Ajouter un lien. Jusqu'à trois liens sont pris en charge. Chaque URL de lien doit être unique.
   - **Texte du lien** (max 60 caractères). Chaque texte de lien doit être unique.
5. Cliquez sur **Afficher l'aperçu** (en haut à droite) pour examiner le contenu de la boîte de dialogue des conditions d'utilisation personnalisées. Apportez des ajustements au contenu des conditions d'utilisation personnalisées, si nécessaire.
6. Une fois prêt avec le contenu des conditions d’utilisation personnalisées, cliquez sur **Suivant**.
7. Vérifiez les conditions d’utilisation personnalisées, confirmez vos paramètres et votre contenu, puis cliquez sur **Publier**.
   L'application est immédiate pour le déclencheur sélectionné.

## Modifier les conditions d’utilisation personnalisées

1. Ouvrez **Paramètres** > **Enterprise Guard** > **Conditions d’utilisation personnalisées**.
2. Dans la liste, sélectionnez la configuration des conditions d’utilisation personnalisées que vous souhaitez mettre à jour, puis cliquez sur **Modifier**.
3. Mettez à jour les champs selon vos besoins dans **Conditions** et **Contenu**.
4. Si vous souhaitez mettre à jour les conditions d’utilisation personnalisées et réinitialiser immédiatement toutes les acceptations des utilisateurs, cliquez sur **Publier immédiatement.**
   Si vous souhaitez mettre à jour les conditions d’utilisation personnalisées et inviter de nouveau les utilisateurs après la fin de la période de récurrence configurée, cliquez sur la flèche vers le bas, sélectionnez **Publier au prochain cycle**, puis cliquez sur **Publier au prochain cycle**.

## Suppression des conditions d’utilisation personnalisées

La suppression désactive immédiatement les conditions d’utilisation personnalisées et ne peut pas être annulée.

1. Ouvrez **Paramètres** > **Enterprise Guard** > **Conditions d’utilisation personnalisées**.
2. Dans la liste, sélectionnez la configuration des conditions d’utilisation personnalisées que vous souhaitez supprimer, puis cliquez sur **Supprimer**.
3. Pour supprimer définitivement les conditions d’utilisation personnalisées que vous avez sélectionnées, cliquez sur **Supprimer les conditions**.
