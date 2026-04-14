---
title: Configuration de l’intégration Power BI (guide d’admin) (BÊTA)
article_id: 18945328862994
translation_id: 18945328862994
locale: fr
sidebar_position: 8
created_at: '2024-05-15T12:57:57Z'
updated_at: '2025-11-25T15:42:21Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
availability:
  notes: 'Disponible pour: forfaits Free, Starter, Business, Education et Enterprise
    Disponible sur: navigateur, application de bureau Rôle requis: admin d’entreprise'
---

Pour les organisations qui souhaitent intégrer Microsoft Power BI à Miro, ce guide fournit des instructions étape par étape afin de configurer l’intégration, l’activer pour une équipe et résoudre les problèmes de sécurité.

Fonctionnalités clés :

- Intégrer les rapports et les tableaux de bord Power BI dans des tableaux Miro
- Préciser les graphiques à importer dans les tableaux Miro
- Demander le contenu Power BI actualisé directement à partir des tableaux Miro

:::tip
L’intégration de Power BI est actuellement en bêta privée.
:::

### Mise en œuvre technique

Miro est intégré à Power BI via l’[API REST](https://learn.microsoft.com/rest/api/power-bi/) ainsi que les [API clientes Power BI Embedded Analytics](https://learn.microsoft.com/javascript/api/overview/powerbi/). Les utilisateurs peuvent aisément lier leurs rapports ou tableaux de bord Power BI aux tableaux Miro en autorisant l’accès à Power BI. Pour l’authentification, nous utilisons [OAuth2.0](https://learn.microsoft.com/entra/identity-platform/v2-protocols).

### Exigences d’intégration

Assurez-vous que votre abonnement comprend :

- Power BI Cloud
- Abonnements pris en charge :
  - SKU Power BI Premium par capacité
  - SKU de réservation de capacité Fabric

## Configurer l’intégration de Power BI

1. Connectez-vous à Microsoft Entra en tant qu’admin.
2. Allez à **Enterprise applications (Applications d’entreprise)** > **Consent and permissions (Consentement et autorisations)** > **Admin consent settings (Paramètres pour les consentements admin)**.
3. Sous **Admin consent requests (Demandes de consentement admin)**, sélectionnez **Yes (Oui)** pour l’option **Users can request admin consent to apps they are unable to consent to (Les utilisateurs peuvent demander le consentement admin pour les applications auxquelles ils ne peuvent pas consentir)**.
4. Sous **Who can review admin consent requests (Qui peut examiner les demandes de consentement admin)**, sélectionnez les utilisateurs, rôles et groupes qui seront habilités à le faire.
5. Ainsi, les utilisateurs pourront demander des approbations. Pour afficher l’écran des demandes d’approbation, l’utilisateur non-admin doit coller un lien Power BI sur un tableau Miro de l’équipe Miro activée pour les tests d’intégration de Miro et Power BI.
6. Les admins sélectionnés à l’étape 4 peuvent accéder à l’écran des demandes de consentement admin pour approuver les demandes en attente.
7. Une fois la demande approuvée, l’intégration de Miro et Power BI devient effective et chaque utilisateur peut effectuer des autorisations personnellement.
8. Pour vérifier le fonctionnement de l’intégration, collez un lien vers un tableau de bord ou un rapport Power BI sur un tableau Miro appartenant à une équipe pour laquelle vous avez activé l’intégration.
9. Cliquez sur **Se connecter** pour confirmer l’autorisation sur la page Web de Power BI.
10. Une boite de dialogue s’ouvre pour vous inviter à sélectionner les graphiques à intégrer. Sélectionnez un graphique et cliquez sur **Ajouter un graphique**.
11. Les graphiques seront ajoutés sous forme d’images à votre tableau Miro.

## Comment désactiver l’intégration de Power BI

Les admins peuvent retirer l’autorisation en supprimant l’application Miro des applications d’entreprise de Microsoft Entra.

1. Connectez-vous à Microsoft Entra.
2. Cliquez sur **Enterprise applications (Applications d’entreprise)** > **Consent and permissions (Consentement et autorisations)**.
3. Dans la liste des applications, repérez et sélectionnez **All applications (Toutes les applications)**.
4. Recherchez l’application **Contenthub Microsoft Power BI Integration (Intégration Microsoft Power BI Contenthub)** dans la liste.
5. Cliquez sur l’application pour accéder à ses propriétés.
6. Dans les propriétés de l’application, cliquez sur **Delete (Supprimer)**.

## Limites de l’intégration

- L’intégration sur les tableaux publics n’est pas prise en charge.
- L’intégration des liens de base de données n’est pas prise en charge.
- L’intégration des liens à partir du menu de partage n’est pas prise en charge.

## Conservation des données

Les données Power BI intégrées suivent la politique de conservation standard de Miro appliquée à toutes les données des clients. Lisez notre [Addenda Miro sur le traitement de données](https://miro.com/legal/documents/Miro-Data-Processing-Addendum.pdf).

Les différents types de données issus des liens Power BI collés sont récupérés sous forme d’image et stockés dans Miro :

- Images de vignettes provenant des tableaux de bord Power BI
- Images de visuels provenant des rapports Power BI
- Titres des tableaux de bord, rapports, visuels et vignettes Power BI
- Noms de pages issus des rapports Power BI
- Noms et valeurs des filtres issus des rapports Power BI

## Foire aux questions

Pourquoi l’intégration Power BI est-elle en version bêta ?

La phase bêta vise à recueillir des retours pour améliorer la stabilité et l’expérience utilisateur. La sécurité demeure une priorité.
