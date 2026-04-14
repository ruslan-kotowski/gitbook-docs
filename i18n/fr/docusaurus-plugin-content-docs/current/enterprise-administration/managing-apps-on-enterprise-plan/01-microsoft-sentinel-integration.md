---
title: "Int\xE9gration de Microsoft Sentinel"
article_id: 31325908249362
translation_id: 31325908249362
locale: fr
sidebar_position: 1
created_at: '2025-11-24T18:16:15Z'
updated_at: '2025-12-16T15:49:35Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: audit-logs
---

## Aperçu

Le connecteur [Miro](https://miro.com/) ingère les journaux d'audit et les journaux d'activité de contenu des [Miro REST APIs](https://developers.miro.com/reference/overview) dans Microsoft Sentinel en utilisant le cadre sans code (CCF). Cela centralise la surveillance de l'activité de l'espace de travail Miro dans Microsoft Sentinel pour la détection des menaces de sécurité, l'investigation des incidents et le reporting de conformité.

## Connecteurs de données

Cette solution inclut deux connecteurs de données.

| Connecteur | Exigences du forfait | Ce qu'il capture | Références |
| --- | --- | --- | --- |
| **Journaux d’audit Miro (Forfait Enterprise)** | Forfait Enterprise | Événements d’audit à l’échelle de l’organisation, y compris l’authentification des utilisateurs, l’accès aux contenus, les changements d’équipe et les actions administratives. | [Documentation API](https://developers.miro.com/reference/enterprise-get-audit-logs) | [Aperçu des journaux d'audit](https://developers.miro.com/reference/audit-logs) |
| **Journaux de Contenu de Miro (Enterprise Plan + Enterprise Guard)** | Forfait Enterprise + module complémentaire Enterprise Guard | Suivi de l'activité du contenu incluant la création, les mises à jour et les suppressions d'éléments pour la conformité et la recherche électronique. | [Documentation API](https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch) | [Vue d'ensemble des journaux de contenu](https://developers.miro.com/reference/board-content-logs) |

## Prérequis

### Exigences générales

- Espace de travail Microsoft Sentinel actif.
- Rôle d'admin d’entreprise dans votre organisation Miro.
- Jeton d’accès OAuth Miro (non-expirant).

### Conditions spécifiques aux connecteurs

#### Pour le connecteur de journaux d’audit

- Forfait Miro Enterprise.
- Portée OAuth : `auditlogs:read`.
- Jeton d’accès.

#### Pour le connecteur de journaux de contenu

- Forfait Miro Enterprise + module complémentaire Enterprise Guard.
- Portée : `contentlogs:export`.
- Jeton d’accès.
- Identifiant de l’organisation Miro.

## Installation

Il existe deux façons de configurer les connecteurs Miro.

- **Option 1 (recommandée) :** Utiliser les intégrations d'entreprise. Configuration la plus simple avec génération automatique de jeton.
- **Option 2 (alternative) :** Créer une application OAuth personnalisée. Plus de contrôle sur la configuration de l’application OAuth.

**Remarque :** Lors de l'utilisation de l'option 1, l'intégration est automatiquement liée à l'équipe ayant le plus grand nombre d'utilisateurs dans votre organisation. Lors de l'utilisation de l'option 2, vous pouvez choisir l'équipe sur laquelle installer l'application. Cependant, le choix de l'équipe n'affecte pas les journaux collectés. Les deux options offrent un accès aux journaux à l'échelle de l'organisation. Tous les événements pertinents pour l'intégration de toutes les équipes sont inclus dans vos journaux.

### Option 1 : Utiliser les intégrations Enterprise (recommandé)

C'est l'option la plus simple pour la plupart des utilisateurs. Elle crée automatiquement une application OAuth et génère un jeton d'accès pour vous via les paramètres d'intégration Enterprise de Miro.

#### Pour le connecteur de journaux d'audit

1. Ouvrez les [paramètres de l'entreprise Miro](https://miro.com/app/settings/).
2. Développez la section **Applications et intégrations**.
3. Cliquez sur **Intégrations Enterprise**.
4. Activez le basculeur **SIEM**.
5. Copiez la valeur du **jeton d’accès** qui apparaît.
6. Conservez le jeton en lieu sûr.

#### Pour le connecteur des journaux de contenu

1. Ouvrez les [paramètres de l’entreprise Miro](https://miro.com/app/settings/).
2. Développez la section **Applications et intégrations**.
3. Cliquez sur **Intégrations Enterprise**.
4. Activez le basculement **eDiscovery**.
5. Copiez la valeur du **Jeton d'accès** qui apparaît.
6. Obtenez votre **ID d'organisation** à partir de l'URL du navigateur :
   - Regardez l'URL du navigateur pour trouver votre ID d'organisation.
   - Le format de l'URL est le suivant : `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Copiez votre ID d'organisation à partir de l'URL (la valeur numérique).
7. Stockez en toute sécurité à la fois le token et l'ID d'organisation.

### Option 2 : Utiliser une application OAuth personnalisée (alternative)

Cette option vous donne plus de contrôle sur la configuration de l'application OAuth. Utilisez-la si vous avez besoin de personnaliser les scopes, de gérer plusieurs intégrations ou si vous préférez la gestion manuelle des applications OAuth.

#### Étape 1 : Créer une application OAuth Miro

1. Connectez-vous à votre compte Miro.
2. Rendez-vous sur les [paramètres de l'application Miro](https://miro.com/app/settings/user-profile/apps).
3. Cliquez sur **Créer une nouvelle application**.
4. Sélectionnez l'option **Jeton d'accès non expirant** lors de la création de l'application ([en savoir plus sur les jetons OAuth](https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens)).
5. Activer les portées OAuth requises :
   - `auditlogs:read` pour le connecteur des journaux d’audit.
   - `contentlogs:export` pour le connecteur des journaux de contenu (nécessite Enterprise Guard).
6. Cliquez sur **Installer l’application et obtenir le jeton OAuth**.
7. Copiez le **Jeton d’Accès** et conservez-le en toute sécurité.

Pour des instructions détaillées sur la configuration OAuth, voir [Guide de démarrage avec OAuth](https://developers.miro.com/docs/getting-started-with-oauth).

#### Étape 2 : Obtenir l’ID de l’organisation (pour les journaux de contenu uniquement)

1. Allez dans les [paramètres de l'entreprise Miro](https://miro.com/app/settings/).
2. Regardez l'URL de votre navigateur pour trouver votre ID d'organisation :
   - Le format de l'URL est : `https://miro.com/app/settings/company/\{ORGANIZATION_ID\}/`.
   - Copiez votre ID d'organisation depuis l'URL (sa valeur numérique).

### Déployer la solution dans Microsoft Sentinel

1. Dans Microsoft Sentinel, accédez à **Content Hub**.
2. Recherchez **"Miro"** et cliquez sur la solution.
3. Cliquez sur **Installer** et suivez l'assistant de déploiement.
4. Sélectionnez votre espace de travail pour l’analyse des journaux.
5. Complétez l'installation.

### Configurer les connecteurs de données

#### Connecteur des journaux d’audit Miro

1. Dans Microsoft Sentinel, allez dans **Connecteurs de données**.
2. Trouvez **Miro Audit Logs (Enterprise Plan)** et cliquez sur **Ouvrir la page du connecteur**.
3. Cliquez sur **Connecter**.
4. Entrez votre **Jeton d'accès**.
5. Cliquez sur **Connecter** pour activer le connecteur.

#### Connecteur des journaux de contenu Miro

1. Dans Microsoft Sentinel, allez à **Connecteurs de données**.
2. Trouvez **Journaux de contenu Miro (Forfait Enterprise + Enterprise Guard)** et cliquez sur **Ouvrir la page du connecteur**.
3. Cliquez sur **Connecter**.
4. Entrez votre **ID d'organisation**.
5. Entrez votre **Jeton d'accès**.
6. Cliquez sur **Connecter** pour activer le connecteur.

L'ingestion de données commence 5 à 10 minutes après l'activation du connecteur.

## Tableaux de données

### MiroAuditLogs_CL

Événements d'audit au niveau de l'organisation comprenant :

- Authentification et accès des utilisateurs.
- Opérations sur le contenu.
- Modifications au niveau de l'organisation.
- Modifications de profil des utilisateurs.
- Actions administratives.

**Colonnes clés**

| Colonne | Description |
| --- | --- |
| `TimeGenerated` | Horodatage de l'événement. |
| `event` | Nom de l'événement identifiant l'action ou l'activité spécifique. |
| `logType` | Type d'entrée de journal. |
| `category` | Catégorie d'événement regroupant les événements connexes. |
| `createdBy_email` | Utilisateur qui a déclenché l'événement. |
| `context_ip` | Adresse IP de l'événement. |
| `details` | Informations supplémentaires spécifiques à l'événement (JSON). |

### MiroContentLogs_CL

Journaux d'activité au niveau du contenu comprenant :

- Opérations sur les éléments avec l’attribution d’utilisateur et les horodatages.
- Transitions d'état et modifications.
- Suivi d'activité pour la conformité et la découverte électronique.

**Colonnes clés**

| Colonne | Description |
| --- | --- |
| `TimeGenerated` | Horodatage de l'événement. |
| `actionType` | Type d'action effectuée sur le contenu. |
| `actor_email` | Utilisateur ayant effectué l'action. |
| `itemType` | Type d'élément de contenu affecté. |
| `contentId` | Identifiant unique du contenu. |
| `state` | Informations sur l'état de l'élément (JSON). |

## Exemples de requêtes

### Consulter les événements d'audit récents

```
MiroAuditLogs_CL
| sort by TimeGenerated desc
| project TimeGenerated, event, category, createdBy_email, context_ip
| take 20
```

### Activité par utilisateur et type d'événement

```
MiroAuditLogs_CL
| summarize EventCount = count() by createdBy_email, event, category
| order by EventCount desc
```

### Modifications de contenu par utilisateur

```
MiroContentLogs_CL
| where TimeGenerated > ago(7d)
| summarize Changes = count() by actor_email, actionType
| order by Changes desc
```

### Tendances des événements au fil du temps

```
MiroAuditLogs_CL
| summarize count() by event, bin(TimeGenerated, 1h)
| render timechart
```

### Utilisateurs les plus actifs (modifications de contenu)

```
MiroContentLogs_CL
| where TimeGenerated > ago(30d)
| summarize TotalActions = count() by actor_email
| top 10 by TotalActions desc
```

## Résolution des problèmes

### Aucune donnée disponible

- Vérifiez que le jeton d'accès est valide et dispose des permissions correctes.
- Pour les journaux de contenu, confirmez que votre organisation dispose du module complémentaire Enterprise Guard.
- Vérifiez que l'ID de l'organisation est correct (pour les journaux de contenu).
- Attendez 5 à 10 minutes pour l'ingestion initiale des données.
- Vérifiez l'état du connecteur sur la page **Connecteurs de données**.

### Erreurs d’authentification

#### Si vous utilisez l’option 1 (bascule des intégrations Enterprise)

- Accédez aux [paramètres de l’entreprise Miro](https://miro.com/app/settings/), développez **Applications et intégrations**, et cliquez sur **Intégrations Enterprise**.
- Vérifiez que la bascule (SIEM pour les journaux d’audit, eDiscovery pour les journaux de contenu) est toujours activée.
- Si un autre admin a désactivé la bascule, le jeton sera invalidé.
- Réactivez la bascule pour générer un nouveau jeton et mettez à jour la configuration du connecteur.
- Vérifiez que vous avez le rôle d’admin d’entreprise dans Miro.

#### Si vous utilisez l'option 2 (application OAuth personnalisée)

- Vérifiez que le jeton n'a pas été révoqué dans les [paramètres de l'application Miro](https://miro.com/app/settings/user-profile/apps).
- Assurez-vous que l'application OAuth a les permissions requises activées.
- Régénérez le jeton si nécessaire et mettez-le à jour dans la configuration du connecteur.
- Vérifiez que vous avez le rôle d’admin d’entreprise dans Miro.

### Journaux de contenu ne fonctionnent pas

- Vérifiez que votre forfait Miro inclut le module complémentaire **Enterprise Guard** (non disponible avec le forfait de base Enterprise).
- Confirmez que l'export au format `contentlogs:export` est activé.
- Vérifiez à nouveau que l'identifiant de l'organisation est correct.
- Contactez votre gestionnaire de compte Miro si vous devez changer de forfait pour Enterprise Guard.

## Ressources

### Ressources du Centre d’assistance Miro

- **Journaux d'audit Miro :** `../security-integrations/security-management/01-audit-logs.md
- **Journaux de contenu Miro :** `../canvas-25-admin-features/ediscovery/06-content-logs-overview.md
- **Guide d'intégration Miro avec Sentinel :** `01-microsoft-sentinel-integration.md`.

### Documentation pour développeurs Miro

- **Démarrage avec l'API Enterprise :** `https://developers.miro.com/docs/getting-started-with-enterprise-api`.
- **Démarrage avec OAuth :** `https://developers.miro.com/docs/getting-started-with-oauth`.
- **Autorisation par jeton OAuth :** `https://developers.miro.com/reference/authorization-flow-for-non-expiring-access-tokens`.
- **API des journaux d'audit :** `https://developers.miro.com/reference/enterprise-get-audit-logs`.
- **API des journaux de contenu :** `https://developers.miro.com/reference/enterprise-board-content-item-logs-fetch`.
- **Référence de l'API :** `https://developers.miro.com/reference`.

### Microsoft Sentinel

- **Documentation Microsoft Sentinel :** `https://docs.microsoft.com/azure/sentinel/`.
