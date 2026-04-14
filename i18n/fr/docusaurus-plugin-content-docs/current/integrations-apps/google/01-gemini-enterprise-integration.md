---
title: Intégration de Gemini Enterprise (bêta)
article_id: 32304596526482
translation_id: 32304596526482
locale: fr
sidebar_position: 1
created_at: '2026-01-05T10:38:04Z'
updated_at: '2026-02-17T09:38:53Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: bring-your-own-ai
availability:
  notes: 'Qui peut le faire: Les admins d’entreprise Quels forfaits: Business, Enterprise
    Quelles plateformes: Navigateur, Bureau'
---

En tant qu'admin d’entreprise, vous pouvez activer et configurer l’intégration Gemini Enterprise pour les équipes de votre organisation Miro.

L’intégration Gemini Enterprise vous permet de connecter Gemini Enterprise comme ressource de [connaissance](../../using-miro/miro-ai/09-knowledge.md) dans Miro. Par exemple, utilisez Gemini Enterprise pour fournir des renseignements sur l’entreprise aux partenaires d’IA et aux flux.

Vous pouvez également connecter Gemini Enterprise à l'application de [chat](../../using-miro/miro-ai/09-knowledge.md) autonome dans Miro.

Pour utiliser l’intégration Gemini Enterprise, suivez ces étapes :

1. Activer l'application Gemini Enterprise.
   1. En tant qu'admin d’entreprise, allez dans la **Console d’administration**.
   2. Accédez à **Applications et intégrations** > **Applications** > **Ajouter des applications**.
   3. Recherchez et trouvez **Gemini Enterprise**.
      Si vous ne trouvez pas l’application par son nom, recherchez en utilisant l'ID client suivant : `2392210303456548729`.
   4. Dans le profil de l'application, sélectionnez si vous souhaitez ajouter l'application pour **Toutes les équipes dans \{Team name\}**, ou choisissez **Dans** **des équipes spécifiques**.
   5. Cliquez sur **Ajouter**.
2. Configurer l'application Gemini Enterprise.
   1. Dans la **Console d'administration**, allez à **Applications et intégrations** > **Applications**.
   2. Pour Gemini Enterprise, assurez-vous que **Autorisée** est activée. Puis cliquez sur **Paramètres**.
   3. Ajoutez vos détails de configuration pour Gemini Enterprise.
      Pour savoir comment trouver l'ID de projet, consultez (Externe) [Localiser l'ID de projet](https://support.google.com/googleapi/answer/7014113?hl=en).
      Pour obtenir l'ID d'application, accédez à Gemini Enterprise > Applications, et utilisez la valeur dans la colonne ID.
      ![](images/33222207775122_image (2).png)
      *Configurez l'application Gemini Enterprise pour l'utiliser dans Miro.*

      > ✏️ **Projet ID** et **ID d'application** sont requis. Les autres champs sont facultatifs.
   4. Cliquez sur **Enregistrer**.

:::note
Lorsqu'un membre de l'équipe connecte Gemini Enterprise comme [ressource de connaissances](../../using-miro/miro-ai/09-knowledge.md) pour la première fois, ce membre doit s'authentifier. Le membre de l'équipe doit avoir une licence Gemini Enterprise.
:::
