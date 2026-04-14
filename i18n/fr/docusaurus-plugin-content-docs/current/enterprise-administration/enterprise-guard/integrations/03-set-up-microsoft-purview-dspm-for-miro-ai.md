---
title: "Configurer Microsoft Purview DSPM pour Miro IA (b\xEAta)"
article_id: 28698434922386
translation_id: 28698434922386
locale: fr
sidebar_position: 8
created_at: '2025-08-11T19:20:50Z'
updated_at: '2026-01-12T11:28:20Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Utilisez cette procédure pour configurer Microsoft Purview Data Security Posture Management (DSPM) pour Miro IA afin que les prompts et réponses de Miro apparaissent dans le DSPM pour l'IA de Microsoft Purview. Après la configuration, vous validerez les événements et apprendrez à gérer l'intégration.

## **Prérequis**

### **Miro**

- Forfait Enterprise avec **Enterprise Guard** activé.
- Vous êtes un **admin d'entreprise**.
- **Microsoft Entra ID** est configuré comme **fournisseur SSO** dans Miro.
- Pour activer cette fonctionnalité en bêta, contactez votre responsable Customer Success.

### **Microsoft**

- Licence Microsoft Purview active avec prise en charge de la DSPM pour l'IA.
- ID de locataire Microsoft Entra ID utilisé pour l'authentification unique Miro (le GUID qui identifie votre organisation/locataire Microsoft).
- Un rôle Entra qui peut accorder un consentement administrateur pour l'ensemble du locataire à une application.

## **Configurer l’intégration dans Miro**

1. Dans Miro, ouvrez **Paramètres Enterprise → Intégrations Enterprise**.
2. Faites défiler vers le bas, puis cliquez pour activer **Microsoft Purview DSPM pour l'IA**.
3. Dans la case ID de locataire, entrez votre **ID de locataire Microsoft Entra**.
4. Cliquez sur **Connecter**.
5. Lorsqu'on vous le demande, connectez-vous à Microsoft Entra avec un compte pouvant accorder un **consentement administratif généralisé**.
6. Examinez le consentement pour l'application **gouvernance Miro AI** et cliquez sur **Accepter**.
7. Retournez à Miro et confirmez que l'intégration affiche **Connecté**.

## **Valider l'activité dans Microsoft Purview**

1. Dans Miro, effectuez une simple action d'IA (par exemple, **résumer** les pense-bêtes sur un tableau).
2. Attendez **de 10 à 30 minutes** pour l'ingestion.
3. Dans Microsoft Purview, allez à **Microsoft Purview → DSPM pour IA → Explorateur d'activités** (la vue Purview qui liste les activités d'IA). Vous pouvez également consulter les informations dans les journaux d'audit.
   Note : Tous les prompts et réponses basés sur du texte des fonctionnalités Miro IA sont transmis à Purview. Actuellement, le contenu des images n'est pas transmis à Microsoft Purview.
4. Filtrez pour les événements **récents** et localisez l'activité provenant de Miro (par exemple, prompts et réponses).

## **Gérer l'intégration**

- **Déconnecter** : Dans Miro, allez dans **Intégrations d'entreprise → Microsoft Purview pour l'IA → Déconnecter**.
- **Changer de locataire** : **Déconnectez** d'abord, puis **Connectez**-vous à nouveau en utilisant un **ID de locataire** différent.

## **Dépannage**

- **Option d'intégration manquante** : Assurez-vous que votre organisation dispose de **Enterprise Guard** et que votre compte peut accéder aux **Intégrations d'entreprise**. Demandez à un **Admin de l'entreprise** d'accorder l'accès.
- **ID de locataire incorrect ou erreur de connexion** : L'ID de locataire doit **correspondre exactement** au locataire Microsoft Entra utilisé pour le **SSO** de Miro.
- **Consentement échoué ou boucle de connexion** : Connectez-vous avec un compte capable d'accorder le **consentement administrateur global** (travaillez avec votre admin Microsoft).
- **Aucune activité visible** : Confirmez qu'une action AI de test a été effectuée par un utilisateur qui se connecte à Miro via le **tenant configuré** ; attendez **10–30 minutes** ; vérifiez votre **licence Purview** ; et consultez **DSPM pour AI → Explorateur d'activités**.
- **Multiples tenants/IdP** : Un seul **tenant** peut être configuré dans Miro. Les activités des utilisateurs qui se connectent via SSO pour d'autres tenants/IdP ne sont **pas** transférées.

## **Limitations connues**

Pour plus d'informations, consultez la [section des limitations connues dans la documentation d'aperçu](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).
