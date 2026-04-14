---
title: "Journaux d\u2019interaction avec l\u2019IA (b\xEAta)"
article_id: 34049604547858
translation_id: 34049604547858
locale: fr
sidebar_position: 1
created_at: '2026-03-15T21:28:41Z'
updated_at: '2026-03-16T09:09:18Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Les journaux d'interaction IA permettent aux admins disposant du module complémentaire Enterprise Guard de collecter et d'examiner les enregistrements de l'utilisation de Miro IA au sein de leur organisation. En activant les journaux d'interaction IA, les admins peuvent offrir aux équipes de sécurité, de conformité et de gouvernance une meilleure visibilité sur la façon dont les fonctionnalités IA sont utilisées et quelles informations sont traitées par les systèmes IA.

Les journaux d'interaction IA aident les organisations à :

- Surveiller comment les fonctionnalités IA sont utilisées dans toute l'organisation
- Apporter un soutien aux examens de gouvernance, de conformité et de sécurité
- Fournir une visibilité sur les informations partagées avec les systèmes IA
- Renforcer la confiance et l'adoption responsable des outils IA

Les journaux d’interaction IA capturent les enregistrements des interactions entre les utilisateurs et les fonctionnalités alimentées par l’IA dans Miro. Ces enregistrements aident les organisations à examiner comment l’IA est utilisée au sein de l’organisation et soutiennent les processus d’audit interne, de gouvernance et de conformité.

Lorsqu'activés, les journaux d'interaction IA capturent :

- Les prompts des utilisateurs soumis aux fonctionnalités IA
- Les réponses générées par l’IA retournées par le système
- Le contexte du système associé à l’interaction

## Avant de commencer

- Vous devez être un admin pour activer ou configurer les journaux d'interaction avec l'IA.
- Le module complémentaire Enterprise Guard est requis pour utiliser cette fonctionnalité.
- Les journaux d'interaction avec l'IA doivent être activés avant que la collecte de données ne commence.
- Seules les interactions qui se produisent après l'activation de la journalisation sont enregistrées.

## Activer les journaux d'interaction avec l'IA

1. Accédez à la **console d'administration**.
2. Sélectionnez **Sécurité**.
3. Cliquez sur **Journaux d'audit**.
4. Ouvrez l'onglet **Paramètres**.
5. Dans la section **Journaux d'interaction IA**, activez **Collecter les journaux d'interaction IA**.
6. Sélectionnez la **période de conservation des journaux**.
7. Enregistrez vos modifications.

Une fois ce paramètre activé, Miro commence à collecter les journaux d'interaction IA pour les nouvelles interactions avec l'IA.

## Configurer la conservation des journaux

Les administrateurs peuvent configurer la durée de stockage des journaux d’interaction avec l’IA.

1. Accédez à la **console d’administration > Sécurité > Journaux d’audit**.
2. Dans la section **Journaux d’interaction avec l’IA**, sélectionnez la **période de conservation** souhaitée.
3. Sauvegardez vos modifications.

Les journaux sont automatiquement supprimés lorsque la période de conservation configurée expire.

## Accéder aux journaux d’interaction avec l’IA via des API

Les journaux d’interaction avec l’IA peuvent être récupérés en utilisant l’API des journaux d’interaction avec l’IA.

Cela permet aux organisations d’exporter et d’analyser les données d’interaction avec l’IA en utilisant leurs systèmes de gouvernance, de conformité ou de surveillance de sécurité existants.

Les cas d’utilisation courants incluent :

- Gouvernance et surveillance de l'IA
- Surveillance de la sécurité
- Audit de conformité
- Enquêtes internes

Pour plus d'informations, consultez la [documentation pour les développeurs](https://developers.miro.com/reference/enterprise-get-ai-interaction-logs).

## Restrictions

La version actuelle inclut la version initiale de l'enregistrement des interactions de l'IA. Les restrictions suivantes s'appliquent :

- Les invocations d'outils à partir des fonctionnalités IA ne sont pas actuellement enregistrées.
- Les interactions liées aux intégrations Miro MCP ne sont pas actuellement enregistrées.
- Les événements de modération et les blocages de prompt sensibles ne sont pas actuellement enregistrés.
- Les images ne sont pas incluses dans les journaux d'interaction IA.
