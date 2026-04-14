---
title: Référence pour Jira on-premise avec autorisation tiers utilisant OAuth 2.0
article_id: 26726425696530
translation_id: 26751166360338
locale: fr
sidebar_position: 11
created_at: '2025-05-16T09:09:40Z'
updated_at: '2025-11-25T15:51:16Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Qui peut le faire: Admins d’entreprise Quels forfaits: Entreprise'
---

Cet article fournit des détails techniques pour utiliser un serveur d'autorisation tiers avec OAuth 2.0 afin d'intégrer Jira à Miro.

Pour savoir comment établir une connexion, consultez [Connectez-vous à Jira sur site avec des serveurs d'autorisation tiers en utilisant OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Comment l'intégration de Jira avec Miro fonctionne en utilisant l'autorisation sur site et OAuth 2.0

Le graphique suivant montre le flux de communication entre Miro et un serveur d'autorisation Jira sur site.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Intégration de Miro et Jira utilisant un serveur d'autorisation sur site via une passerelle API*

## Paramètres de configuration

Pour configurer le flux d'autorisation entre Miro et Jira en utilisant un serveur d'autorisation tiers avec OAuth 2.0, vous devez spécifier les paramètres suivants :

- **Serveur d’autorisation**
  - URL de demande d'autorisation
  - URL de demande de jeton
  - Portée
- **Configuration de l’application d’autorisation**
  - Identifiant client
  - Clé secrète client
- **Instance Jira**
  - URL publique Jira
  - URL de base Jira ; URL interne

:::note
Miro fournit l'URL de redirection que le serveur d'autorisation valide par rapport à l'application enregistrée.
:::

**Plus d’informations :** Voir [Connecter à Jira sur site avec des serveurs d'autorisation tiers en utilisant OAuth 2.0](https://help.miro.com/hc/articles/25692796700306).

## Requêtes d'autorisation utilisateur entre Miro et le serveur d'autorisation sur site

Pour une intégration entre Miro et Jira utilisant un serveur d'autorisation tiers, le graphique suivant montre le flux de demande d'autorisation utilisateur.

![](../../../../../../docs/integrations-apps/atlassian/images/32535032016146_image.png)

*Demande d’autorisation de l’utilisateur*

### Demande d'autorisation

```
https://{authorization_URL}?
    type_de_réponse=code&
    client_id={CLIENT_ID}&
    redirect_uri={Miro Redirect URI}&
    scope={scope}&
    état={state}
```

L'utilisateur peut ajouter des paramètres à la demande d'autorisation sous forme de paires clé-valeur dans la configuration.

### Demande de jeton

```
curl --request POST \
    --url '{URL de demande de token}' \
    --header 'content-type: application/x-www-form-urlencoded' \
    --data grant_type=authorization_code \
    --data 'client_id={CLIENT_ID}' \
    --data 'client_secret={CLIENT_SECRET}' \
    --data 'code={Code d’Autorisation Obtenu}' \
    --data 'redirect_uri={Miro Redirect URI}' \
```

Après que Miro a reçu le code d'autorisation, Miro fournit l'état et demande une paire de jetons.

### Actualiser l'échange de jetons

```
curl --request POST \
    --url '{token request URL}' \
    --header 'content-type: application/x-www-form-urlencoded'
    --données grant_type=refresh_token \
    --data 'client_id={CLIENT_ID}' \
    --data 'refresh_token={jeton d'actualisation valide actuel}' \
```

Assurez-vous que l'opération de jeton de rafraîchissement est activée ; activez l'accès hors ligne aux API.

### Demandes d'API Jira

```
curl --request GET \
    --url {URL Jira Public}/rest/api/{apiversion}/... \
    --header 'autorisation: Titulaire {accessToken}' \
    --en-tête 'content-type: application/json'
```

Chaque requête utilise l'URL publique Jira fournie comme URL de base et le jeton d'accès utilisateur comme jeton d'autorisation.
