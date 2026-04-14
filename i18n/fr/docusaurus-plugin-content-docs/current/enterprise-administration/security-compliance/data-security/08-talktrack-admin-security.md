---
title: "S\xE9curit\xE9 de l\u2019administration de la fonctionnalit\xE9 Enregistrement"
article_id: 11148211487378
translation_id: 11148211487378
locale: fr
sidebar_position: 8
created_at: '2023-04-24T08:12:36Z'
updated_at: '2025-11-25T16:22:19Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

La fonctionnalité Enregistrement permet aux utilisateurs d’enregistrer des tutoriels interactifs vidéo ou audio de leur tableau Miro afin qu’ils puissent partager leurs idées sans passer par des réunions à rallonge. Découvrez comment Miro garantit un niveau de sécurité et de conformité exceptionnel pour la fonctionnalité Enregistrement.

> ***Mises à jour de l'interface utilisateur de Miro en déploiement progressif***
> Miro améliore l’interface utilisateur du tableau pour la rendre plus inclusive et intuitive, et introduit une évolution des projets, maintenant appelés Espaces. Le déploiement se fera progressivement pour tous les comptes Miro sur plusieurs semaines.
>
> Si vous disposez déjà de l’interface utilisateur améliorée et de la présentation des espaces, cet article peut décrire les points d’entrée qui ont changé.
>
> Pour consulter la documentation la plus récente, voir [la nouvelle interface utilisateur simplifiée de Miro](../../../using-miro/working-on-the-board/02-miro's-new-simplified-user-interface.md).
>
> Cet article sera mis à jour lorsque le déploiement sera terminé.

:::note
Accordez l'accès à [l'enregistrement](../../../using-miro/facilitation-tools/asynchronous-tools/02-talktrack-board-recordings.md) pour votre organisation dans vos paramètres d'[accès aux fonctionnalités](../../managing-enterprise-teams-and-content/06-feature-activation.md).
:::

:::note
Vous pouvez en apprendre davantage sur la confidentialité et la sécurité de l'enregistrement dans le [Miro Talktrack whitepaper for Enterprises](https://go2.miro.com/rs/228-GPV-835/images/Talktrack_WhitePaper.pdf).
:::

## Sécurité de qualité professionnelle

Miro est l’espace de travail en ligne conçu pour favoriser l’innovation au sein de l’entreprise, qui permet aux équipes distribuées de toutes tailles de rêver, de concevoir et de construire l’avenir ensemble. Que ce soit au bureau, à distance ou dans un environnement hybride, vos équipes peuvent utiliser Miro pour tous les cas d’utilisation de l’entreprise.

Mais tout cela implique de grandes responsabilités, et c’est pourquoi nous accordons autant d’importance à la sécurité qu’à la collaboration, afin de protéger vos idées.

|  |  |  |
| --- | --- | --- |
| **Checkmark.png**  **Approuvé et certifié** | **Security_lock.png**  **Protection de confiance** | **Fingerprint.png**  **Gestion sécurisée de l’accès** |
| Meilleures pratiques de l'industrie et exigences réglementaires | Protégez et gérez votre propriété intellectuelle | Contrôlez qui peut accéder et gérer votre contenu Miro |

## Approuvé et certifié

Miro suit les bonnes pratiques de l'industrie et les exigences réglementaires, y compris [ISO 27001, SOC2 Type II et SOC3](https://miro.com/trust/compliance/). Nous veillons également à ce que votre infrastructure et vos services soient conformes aux normes GDPR — y compris les enregistrements Talktrack.

**Gestion du cycle de vie du contenu**

**Suppression d'un enregistrement**
**Suppression d'un enregistrement :** Lorsqu'un enregistrement est supprimé, il ne peut pas être restauré.

**Suppression d'un tableau :** Les enregistrements sont des calques qui fournissent un contexte à un tableau. Si un tableau est supprimé, ses enregistrements seront également supprimés. Toutefois, si un admin restaure un tableau supprimé dans les 90 jours, les enregistrements du tableau seront également restaurés. En savoir plus sur la [suppression de tableau](../../../using-miro/managing-boards/07-how-to-delete-a-board.md).

**Confidentialité**

**Données capturées lors de l'enregistrement d'un enregistrement :** Les mouvements du curseur de la personne qui enregistre et la vue du tableau Miro, le contenu du tableau au moment où l'enregistrement est créé, la vidéo de la personne qui enregistre, soit la vue de sa caméra, soit son avatar, selon que la caméra est activée ou désactivée, l'audio de la personne qui enregistre à partir de la source audio sélectionnée, et tout autre son présent dans le même espace physique que celui de la personne qui présente.

**Données non capturées lors de l'enregistrement d'un enregistrement :** Le curseur ou les informations des autres utilisateurs qui accèdent au tableau au moment de l'enregistrement, l'écran de la personne qui enregistre ou les sons de son ordinateur.

**Avis de confidentialité**

La base juridique du traitement des données à caractère personnel liées à la fonctionnalité Enregistrement, pour lesquelles Miro est le responsable du traitement (essentiellement des métadonnées), est l’exécution d’un contrat (utilisateurs en libre-service) et/ou les intérêts légitimes (tous les utilisateurs). Le client est le responsable du traitement des données enregistrées avec la fonctionnalité Enregistrement. La base juridique du client est à évaluer par ce dernier et il est probable qu’il s’agisse de ses intérêts légitimes.

**Accessibilité**

La fonctionnalité Enregistrement prend en charge la navigation au clavier et la transcription/création de sous-titres automatique.

**Observabilité**

[Les journaux d'audit](../../security-integrations/security-management/01-audit-logs.md) sont disponibles pour l'Enregistrement dans les paramètres d'admin. Nous disposons d’intégrations avec les systèmes SIEM (gestion des événements et des informations de sécurité) suivants :
[Splunk](../../security-integrations/security-information-and-event-management-siem/01-miro-app-for-splunk.md)
[IBM QRadar](../../security-integrations/security-information-and-event-management-siem/02-miro-connector-for-ibm-qradar.md)

**Audits externes**

Miro fait appel aux meilleures sociétés de conseil externes pour réaliser des audits annuels. Notre certification ISO 27001 actuelle est signée par la BSI (British Standard Institution) du Royaume-Uni et nos rapports SOC2 et SOC3 par KirkpatrickPrice aux États-Unis. Lisez-en davantage sur la [conformité chez Miro](https://miro.com/trust/compliance/).

## Protection de confiance

Protégez et gérez la propriété intellectuelle créée ou ajoutée à notre plateforme. Vos données en transit sont chiffrées à l’aide du protocole TLS 1.3 et vos données au repos avec le protocole AES 256.

**Chiffrement**

Dans Miro, les données — y compris celles de la fonctionnalité Enregistrement — au repos sont par défaut chiffrées avec l'algorithme AES256, tandis que les données en transit le sont avec le protocole TLS1.3. Lisez plus dans notre [Livre blanc sur le chiffrement Miro](https://go2.miro.com/rs/228-GPV-835/images/Encryption%20Whitepaper.pdf).

**Classification des données**

Le badge [Classification du tableau](../../canvas-25-admin-features/data-security/02-data-classification.md) n'est pas visible lors du visionnage ou de la réalisation d’un enregistrement.

**Gestion des clés de chiffrement**

Si votre organisation a configuré et déployé la [gestion des clés de chiffrement](../../canvas-25-admin-features/encryption-key-management/01-encryption-key-management-overview.md) (EKM), les admins peuvent demander que Miro utilise la clé de chiffrement de votre organisation pour le contenu des enregistrements.

**Résidence des données**

Par défaut, les données des Enregistrements sont stockées au même endroit que les autres données de contenu client dans Miro : sur les serveurs AWS situés dans l'UE. Miro offre un niveau plus élevé de contrôle et de conformité sur les données de votre entreprise en garantissant que tout votre contenu client est hébergé en Europe. Pour les clients qui ont demandé la [résidence des données aux États-Unis](../../canvas-25-admin-features/data-security/09-us-data-center-residency.md), les données des Enregistrements sont stockées dans notre centre de données principal en Ohio et dans notre centre de données de sauvegarde en Virginie.

## Gestion sécurisée de l’accès

Contrôlez qui peut accéder à Miro grâce à une fonctionnalité de qualité professionnelle, en tirant parti de capacités avancées de gestion des identités et d’administration. En savoir plus sur les fonctionnalités de sécurité et de conformité de l'Enterprise Plan [ici](../../../administration/security-compliance).

**Contrôle de l’accès de votre organisation à la fonctionnalité Enregistrement**

Les admins d’entreprise peuvent accorder ou révoquer l’accès à la fonctionnalité Enregistrement pour toute l’entreprise ou pour certaines équipes dans leurs paramètres [Accès aux fonctionnalités](../../managing-enterprise-teams-and-content/06-feature-activation.md).

**Accès pour réaliser un enregistrement**

L'option pour [réaliser un enregistrement](../../../using-miro/facilitation-tools/asynchronous-tools/02-talktrack-board-recordings.md) est disponible pour les utilisateurs ayant un accès de commentaire ou de modification sur un tableau, ou étant propriétaires ou co-propriétaires de ce tableau.

**Accès pour consulter un enregistrement**

La lecture de l'enregistrement est disponible pour tous les utilisateurs ayant [accès au tableau](../../canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

## Foire aux questions

Un admin d’entreprise peut-il voir quels tableaux contiennent un enregistrement ?

Pour savoir si un tableau dispose d’un enregistrement, vous devez l’ouvrir. Si le tableau ne vous est pas partagé, vous pouvez utiliser les [autorisations d’admin de contenu](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md) pour obtenir l'accès et voir l'enregistrement.

Comment désactiver la fonctionnalité Enregistrement pour mon entreprise ou mon équipe ?

Pour désactiver la fonctionnalité Enregistrement, rendez-vous dans vos paramètres [Accès aux fonctionnalités](../../managing-enterprise-teams-and-content/06-feature-activation.md) et sélectionnez **Personne ne peut l’utiliser**, ou supprimez l’accès pour certaines équipes en cliquant sur **X** en regard de leur nom.

Qu’arrive-t-il aux enregistrements existants lorsqu’un admin révoque l’accès à la fonctionnalité Enregistrement ?

Les enregistrements existants resteront disponibles, mais aucun nouvel enregistrement ne pourra être réalisé.

Les admins peuvent-ils supprimer des enregistrements ?

Les admins peuvent partager un tableau avec eux-mêmes dans les [autorisations de contenu admin](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), puis supprimer l’enregistrement du tableau.

Les noms des utilisateurs s’affichent-ils dans l’application et/ou sont-ils enregistrés avec les données des enregistrements ?

La fonctionnalité Enregistrement affiche le nom (soit le prénom et le nom de famille, soit le nom d’affichage, selon la disponibilité) pendant la lecture comme « nom de la personne qui enregistre ». Cependant, Enregistrement ne sauvegarde que les IDs des utilisateurs, donc aucune information personnelle n'est sauvegardée avec l'enregistrement. Si l’utilisateur ne fait pas partie de l’organisation pendant la lecture, le nom d’affichage sera « Utilisateur inconnu ».
