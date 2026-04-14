---
title: "Configurer les int\xE9grations Microsoft et Power BI"
article_id: 25132703621394
translation_id: 25132703621394
locale: fr
sidebar_position: 3
created_at: '2025-03-06T10:27:14Z'
updated_at: '2025-11-25T15:49:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: powerbi
---

:::note
Pour des documents administratifs complets sur l'intégration de Miro avec Microsoft ou Power BI, incluant des diagrammes détaillés et des FAQ supplémentaires, veuillez vous référer à la [documentation Microsoft admin](https://docs.google.com/document/d/1Gw94z5Pc-elS-pRXKGZVBWKKNEIFR9y9yzAAkbXKwMM/edit?usp=sharing) ou à la [documentation Power BI admin](https://docs.google.com/document/d/1hMepF163jQF8LI-U8ES8DzHVMW4TltXDr14fJ2KU29k/edit?tab=t.0#heading=h.gu9ng058yy7y).
:::

Cet article explique comment configurer une intégration avec Microsoft ou Power BI dans Miro.

## Configurer une intégration Microsoft ou Power BI

Pour configurer une intégration Microsoft ou Power BI, vous devez activer les utilisateurs pour autoriser leur contenu Microsoft ou Power BI dans Miro.

### Prérequis

- Assurez-vous que vous disposez d’un accès admin à Microsoft Entra.
- Un admin d'entreprise a approuvé Microsoft ou Power BI pour votre organisation Miro (cela fait référence aux politiques d'approbation des applications côté Miro si votre organisation restreint les installations d'applications).

### Procédure

Ces étapes se concentrent sur la configuration de Microsoft Entra pour permettre l'intégration Miro.

1. Connectez-vous à **Entra** en tant qu'admin.
2. Allez à **Applications d’entreprise** > **Consentement et autorisations**.
3. Pour **les utilisateurs peuvent demander le consentement de l'admin pour des applications auxquelles ils ne peuvent pas consentir**, sélectionnez **Oui**.
4. Sous **Qui peut examiner les demandes de consentement des admins**, choisissez les utilisateurs, rôles ou groupes nécessaires que vous souhaitez autoriser à examiner les demandes de consentement des admins pour les applications.

:::note
Les administrateurs Entra désignés à l'étape 4 ci-dessus peuvent ensuite accéder à **Applications d'entreprise > Demandes d'autorisation des administrateurs** dans Microsoft Entra pour examiner et approuver l'application "Contenthub PowerBI Integratio" (ou un nom similaire) pour l'organisation.
:::

## Validez votre intégration Microsoft ou PowerBI

Copiez et collez un lien vers votre tableau Miro.

Si l'application est pré-approuvée par l'admin d’entreprise, suivez ensuite les instructions modales à l'écran. Miro ajoute le contenu de votre application au tableau en tant qu’iFrame.

Si l'application n'est pas pré-approuvée, alors le modale **Ajouter & autoriser** s'ouvre et vous permet d'envoyer une demande à votre admin d’entreprise. Envoyer votre demande.

Lorsque votre admin d’entreprise répond, vous recevrez une notification.

**Plus d’informations :** Voir [Gestion des applications](../../enterprise-administration/managing-apps-on-enterprise-plan/02-app-management.md).
