---
title: "Surveiller l'\xE9tat de la gestion des cl\xE9s de chiffrement"
article_id: 31325531757970
translation_id: 31325531757970
locale: fr
sidebar_position: 1
created_at: '2025-11-24T17:59:06Z'
updated_at: '2026-02-04T20:46:28Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

Les administrateurs peuvent surveiller et suivre l'état de leur configuration de gestion des clés de chiffrement (EKM) dans la console d’admin de Miro. Cela apporte une plus grande transparence dans l’onboarding des clés et l’avancement du chiffrement, vous permettant de rester informé sans avoir besoin de support supplémentaire.

## Vérifier l'état de l'EKM

1. Dans la console d'admin de Miro, allez à **Enterprise Guard**.
2. Sélectionnez **Gestion des clés de chiffrement**.
3. Dans la section **État**, examinez l'état actuel et le message.

## Comprendre l'état de l'EKM

La section **État** montre où vous en êtes dans la configuration de l'EKM et le processus de chiffrement.

| Statut | Signification |
| --- | --- |
| **Clés personnalisées ajoutées** | Miro configure le chiffrement avec vos clés personnalisées. Une fois prêtes, vos clés commencent automatiquement à chiffrer le contenu. |
| **Activation des clés en cours** | Les nouveaux contenus sont chiffrés avec vos clés personnalisées. Le re-chiffrement des contenus existants est en cours. |
| **Clés personnalisées actives** | Tout le contenu est chiffré avec vos clés personnalisées. |
| **Retour aux clés par défaut** | Miro remplace votre chiffrement par les clés par défaut de Miro. Vos clés personnalisées seront supprimées. |

## Révision des clés configurées

Dans la section Clés, vous pouvez consulter les identifiants des clés actuellement configurées pour la gestion des clés de chiffrement. Si Miro gère vos clés personnalisées, vous pourriez voir une notification au lieu d'un ARN de clé.

- **Clé primaire**

  Chiffre les tableaux, commentaires et autres contenus de votre organisation.
- **Clé de stockage de sauvegarde**

  Chiffre les versions archivées et les sauvegardes.
- **ARN de clé**

  Identifiant de clé dans [AWS KMS](https://aws.amazon.com/kms/). Si Miro gère vos clés personnalisées, vous pourriez voir une notification au lieu d'un ARN de clé.

(Optionnel) Pour apporter des modifications à vos clés (par exemple, si vous voyez la mauvaise clé ou si vous souhaitez revenir au chiffrement par défaut), vous pouvez contacter votre Customer Success Manager ou le [support@miro.com](mailto:support@miro.com).
