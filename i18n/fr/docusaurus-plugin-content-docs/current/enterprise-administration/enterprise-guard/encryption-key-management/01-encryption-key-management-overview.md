---
title: "Aper\xE7u de la gestion des cl\xE9s de chiffrement"
article_id: 14634334255250
translation_id: 14634334255250
locale: fr
sidebar_position: 0
created_at: '2023-10-24T14:24:53Z'
updated_at: '2026-02-05T15:17:37Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: enterprise-key-management
---

Le module complémentaire Enterprise Guard inclut une option pour la gestion des clés de chiffrement. La gestion des clés de chiffrement offre un contrôle centralisé sur les clés de chiffrement pour protéger vos données. Cette solution basée sur le cloud permet de surveiller les journaux d’activité associés aux clés de chiffrement et de révoquer l’accès des clés à vos données.

Pour un meilleur contrôle et une plus grande visibilité sur l'utilisation des clés de chiffrement dans Miro, vous pouvez également utiliser Bring Your Own Key (BYOK). Avec BYOK, vous gérez le chiffrement des données de votre organisation au sein de la plateforme Miro.

## Découvrez les avantages de la gestion des clés de chiffrement

- **Intégration sans effort :** Intégrez sans effort la gestion des clés de chiffrement à votre système, sans installation matérielle ni maintenance, grâce à une solution 100 % basée sur le cloud.

- **Contrôle total des clés :** Bénéficiez d’un contrôle total sur vos clés de chiffrement. Vous avez la possibilité de révoquer votre clé, ce qui rend toutes les données cryptées inaccessibles à la fois à Miro et aux utilisateurs finaux.

- **Visibilité accrue de l’accès :** Obtenez des informations sur les activités liées aux clés grâce à la visibilité de l’accès. Surveillez et suivez les journaux via AWS CloudTrail pour une compréhension approfondie de l’utilisation de votre clé de chiffrement.

![Enterprise Key Management Diagram](images/21016134839442_EKM.png)

## Comment la gestion des clés de chiffrement protège-t-elle les données de ses clients ?

Miro fournit la gestion des clés de chiffrement en offrant le chiffrement de vos données de production et de sauvegarde au repos avec une clé de chiffrement personnalisée tandis que le client accorde à Miro l’accès à la clé de chiffrement personnalisée. Miro prend en charge la gestion des clés de chiffrement avec une clé hébergée dans votre propre compte AWS via AWS KMS. Avec la gestion des clés de chiffrement, vous bénéficiez d’une plus grande visibilité en matière d’audit et d’un meilleur contrôle d’accès aux données (contenu généré par l’utilisateur), telles que les formes, les widgets et les fichiers téléchargés.

## Chiffrement des données à Miro

Garantir la sécurité maximale de vos données est une préoccupation majeure chez Miro. Par défaut, nous employons des mesures de chiffrement pour les données des clients, à la fois en transit et au repos, quel que soit l’abonnement choisi. Lorsque vous accédez à Miro par Internet, vos données bénéficient d’une protection grâce au chiffrement TLS 1.3 et aux certificats PKI émis par Amazon Web Services (AWS). Lorsqu’elles atteignent nos serveurs, vos données sont davantage protégées par un chiffrement AES-256 au repos, à l’aide de clés gérées par Miro via le service de gestion des clés (KMS) d’AWS. [En savoir plus sur la sécurité chez Miro.](https://miro.com/trust/security/)

> Remarque : Vous êtes seul responsable de la sécurité et de la protection de toutes les données de sauvegarde téléchargées ou transférées par vous sur vos systèmes ou sur les systèmes de tiers. Vous êtes seul responsable de sa clé de chiffrement personnalisée. Si vous perdez votre clé de chiffrement personnalisée, Miro ne peut pas vous aider à récupérer l’accès aux données. Une fois que vos données de production ou de sauvegarde sont en transit ou hors du contrôle de Miro, Miro ne peut pas garantir leur protection.

## Comment activer la gestion des clés de chiffrement

La configuration et le déploiement de la gestion des clés de chiffrement nécessitent l’assistance des équipes internes de Miro. Si vous avez besoin d’aide, contactez votre représentant Miro ou [demandez de l’aide via le service d’assistance de Miro ici](../../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).

## Glossaire

- **Données de sauvegarde :** Un instantané de votre contenu créé dans le service Miro ou soumis à celui-ci, qui est stocké par Miro à des fins de récupération et autres.

- **Clé de chiffrement personnalisée :**  Une clé de sécurité unique, personnalisée et mise en œuvre par vos soins, dont les personnes ont besoin pour accéder à vos données de production et de sauvegarde.

- **Données de production :** Toutes les données auxquelles vous et vos utilisateurs accédez lors de l’utilisation et du fonctionnement quotidien des services Miro.
