---
title: "Connecteur Miro pour Okta\_Workflows"
article_id: 8264504421394
translation_id: 8264504421394
locale: fr
sidebar_position: 1
created_at: '2022-10-25T14:04:07Z'
updated_at: '2025-02-26T12:20:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: okta-workflows
---

Configurez le connecteur Miro pour Okta Workflows afin d’utiliser le connecteur Miro Administrator à partir de votre tableau de bord Okta Workflows.

[Découvrez plus en détail l’Administrator Connector (Connecteur admin) et le User Connector (Connecteur utilisateur) dans l’article sur la configuration de l’automatisation pour Okta Workflows.](03-set-up-miro-connectors-for-okta-workflows.md)

> **Disponible pour :** Forfait Enterprise
> **Qui peut le faire :** les admins d’entreprise

## Configurer les paramètres dans Miro

### Générer un jeton d’accès

1. Dans votre page de paramètres Miro Enterprise, accédez à **Applications et intégrations** > **Intégrations d'entreprise**, puis faites défiler la page jusqu'à **Okta Workflows**.

2. 2. Pour activer **Okta workflows**, cliquez sur le bouton à bascule correspondant.

![okta-workflows-turn-on.pngParamètres](images/24938288858898_okta-workflows-turn-on.png)
*d'intégration de Workflows dans Miro Enterprise*

3. 3. Pour copier le jeton d’accès, cliquez sur **Copy** (Copier).

4. 4. Pour générer un nouveau jeton d’accès, cliquez sur **Generate new token** (Générer un nouveau jeton).

![okta-workflows-enablement.pngToken](images/24938326197650_okta-workflows-enablement.png)
*d'*

:::warning
Si le bouton à bascule a déjà été activé par un autre admin d’entreprise, vous ne pourrez pas copier le jeton. Vous pourrez seulement désactiver l’intégration.
:::

:::warning
L’intégration est liée à l’équipe comptant le plus grand nombre d’utilisateurs. Il n’est pas possible de choisir une autre équipe. Cependant, l’intégration fonctionnera pour toutes les équipes du plan Enterprise et les événements liés à l’intégration seront affichés pour l’ensemble du plan dans vos journaux d’audit.
:::

## Configurer les paramètres sur Okta Workflows

### Créer une nouvelle connexion

1. 1. Dans votre tableau de bord Okta Workflows, rendez-vous sur **Connections** (Connexions).

2. 2. Cliquez sur le bouton **+ New Connection** (Nouvelle connexion).

3. 3. Dans la boîte de dialogue **New Connection** (Nouvelle connexion), sélectionnez le connecteur **Miro Administrator**.

![Miro-Administrator-connection.pngConnecteur](images/21019735550482_Miro-Administrator-connection.png)
*d'administration*

4. 4. Collez vos données **Organization ID** (ID d’organisation) et **Access Token** (Jeton d’accès) dans les champs d’entrée correspondants de la boîte de dialogue.

5. **Cliquez sur** Create (Créer).

![Paste-org-ID-and-access-token-click-create.pngCréer](images/21019791309458_Paste-org-ID-and-access-token-click-create.png)
*un nouveau connecteur*

6. Après avoir établi la connexion, vous pouvez commencer à créer sur Okta Workflows.
