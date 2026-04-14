---
title: "Aper\xE7u de l'int\xE9gration b\xEAta de Microsoft Purview DSPM pour l'IA\
  \ et Enterprise Guard"
article_id: 28617278171154
translation_id: 28617278171154
locale: fr
sidebar_position: 0
created_at: '2025-08-07T15:17:38Z'
updated_at: '2026-01-12T11:27:56Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Pour les organisations utilisant Microsoft Entra ID (anciennement Azure AD) comme fournisseur d’identité, Enterprise Guard transmet en toute sécurité les prompts et réponses d'IA à Microsoft Purview Data Security Posture Management (DSPM) pour permettre aux équipes de sécurité et de conformité de surveiller, auditer et contrôler l’utilisation de l'IA générative depuis une seule plateforme de confiance, réduisant ainsi les frais opérationnels, atténuant les risques tels que les fuites de données et les abus, et renforçant la gouvernance de l'IA à l'échelle de l'entreprise chez Miro.

:::note
La version bêta prend en charge les formats de Miro IA, y compris les diagrammes, cartes mentales, documents, prototypes, pense-bêtes et tables, mais pas les images. Nous travaillons à ajouter la prise en charge des images et de nouvelles fonctionnalités d'IA dans les prochaines versions.
:::

## **À qui cela s'adresse**

Cette fonctionnalité est disponible dans la version bêta pour les clients d'Enterprise Guard qui gèrent Miro et Microsoft Entra ID (anciennement Azure AD)/Microsoft Purview.

## **Ce que vous obtenez**

- **Visibilité centralisée :** Consultez l'utilisation de Miro IA dans le hub IA de Microsoft Purview.
- **Auditabilité :** Les prompts (entrées utilisateur) et les réponses (sorties IA) sont enregistrés pour révision.
- **Alignement de la gouvernance :** Utilisez vos workflows Purview existants pour la surveillance, l'alerte et la conservation.

## **Exigences**

### **Miro**

- Forfait Enterprise avec **Enterprise Guard** activé.
- Vous êtes un **admin d’entreprise**.
- Microsoft **Entra ID** configuré comme fournisseur d'authentification unique dans Miro.
- Accès à la page des **intégrations Enterprise** (si vous ne la voyez pas, demandez à un **admin d’entreprise** d’accorder l’accès).
- Pour activer cette fonctionnalité en version bêta, contactez votre responsable Customer Success.

### **Microsoft**

- Licence **Microsoft Purview** active.
- Votre **ID de client Microsoft Entra ID** (le même client utilisé pour l'authentification unique Miro ; le GUID qui identifie votre organisation/client Microsoft).
- Un rôle Entra qui peut **accorder un consentement administrateur à l'échelle du client** à une application.

## **Fonctionnement**

1. Un admin Miro connecte votre client Microsoft Entra depuis la page des **intégrations Enterprise** dans Miro.
2. Cela installe l'application **Miro IA governance** dans votre client Microsoft (via le consentement de l'admin à l'échelle du client).
3. Lorsque les utilisateurs se connectent à Miro via ce client et utilisent Miro IA, Miro transfère le prompt/réponse vers Microsoft Purview.
4. Les activités apparaissent dans le **DSPM pour l'IA → Explorateur d'activités** (vue Purview qui répertorie les activités IA) dans Microsoft Purview (temps d'ingestion autorisé).

## **Visibilité et latence des données**

- Données enregistrées : **Prompts AI et réponses** générés dans Miro par les utilisateurs qui se connectent via l'authentification unique pour le locataire configuré.
- Où le voir : **Microsoft Purview → DSPM pour l'IA → Explorateur d'activités** (la vue de Purview qui répertorie les activités AI). Vous pouvez également consulter les informations dans les journaux d’audit.
  **Remarque :** Tous les prompts et réponses textuels des fonctionnalités de Miro IA sont transférés à Purview. Actuellement, le contenu d’image n’est pas transféré à Microsoft Purview.
- Latence : Les enregistrements apparaissent généralement **sous 10 à 30 minutes** après l'action de l'IA dans Miro.

## **Limitations connues**

- La version bêta prend en charge les formats Miro IA, notamment les diagrammes, cartes mentales, documents, prototypes, pense-bêtes et tables, mais pas les images. Nous travaillons à ajouter la compatibilité pour les images et plus de fonctionnalités d'IA dans les prochaines versions.
- Vous pouvez configurer **un seul ID de locataire Microsoft Entra** à la fois dans Miro.
- Dans des environnements multi-IdP ou multi-locataires, **seules** les activités des utilisateurs qui se connectent à Miro via le **locataire configuré** sont enregistrées dans Microsoft Purview.

## **Sécurité et confidentialité**

Miro transmet les prompts et les réponses d'IA à **votre locataire Microsoft** afin qu'ils puissent être surveillés dans Purview. **La gouvernance, la conservation et les contrôles d'accès** sont gérés dans votre environnement Microsoft.

##

## **FAQ**

- **Question : Quelles fonctionnalités de Miro IA sont enregistrées ?**
  **Réponse :** Tous les prompts et les réponses basés sur texte des fonctionnalités de Miro IA sont transmis à Purview. Actuellement, le contenu image n'est pas transmis à Microsoft Purview.
- **Question : Cela couvre-t-il tous les utilisateurs ?**
  **Réponse :** Seuls les utilisateurs qui s'authentifient sur Miro en utilisant le locataire Microsoft Entra configuré sont couverts.
- **Question : Puis-je exporter les journaux depuis Miro ?**
  **R :** Utilisez Microsoft Purview pour l'export et la conservation. Miro transmet l'activité à votre locataire Microsoft où elle est régie par vos politiques.
- **Q : Qu'en est-il de la sécurité et de la confidentialité ?**
  **R :** Miro transmet les prompts et les réponses d'IA à **votre locataire Microsoft** afin qu'ils puissent être surveillés dans Purview. **La gouvernance, la conservation et les contrôles d'accès** sont gérés dans votre environnement Microsoft.

## **Service d’assistance et ressources**

- Pour les prérequis de consentement Entra, consultez la documentation Microsoft sur l’octroi d’un **consentement administrateur à l'échelle du locataire** à une application.
- Pour les instructions de configuration d'Enterprise Guard, consultez [cette documentation](../../enterprise-subscription-management/integrations/03-set-up-microsoft-purview-dspm-for-miro-ai.md).
