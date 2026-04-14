---
title: "Aper\xE7u des conditions d\u2019utilisation personnalis\xE9es"
article_id: 27375760557330
translation_id: 27375760557330
locale: fr
sidebar_position: 2
created_at: '2025-06-13T08:24:28Z'
updated_at: '2025-11-04T14:10:39Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: roles-permissions
---

La fonctionnalité des conditions d’utilisation personnalisées permet aux admins d’afficher un dialogue personnalisé des Conditions d’utilisation pour tous les membres internes de leur organisation Miro. Cela garantit que les utilisateurs examinent et reconnaissent les conditions et politiques de votre organisation avant d'utiliser Miro. Utilisez cette fonctionnalité pour informer les utilisateurs sur les politiques d'utilisation acceptable des fonctionnalités de Miro, y compris Miro IA. Les admins peuvent ajouter plusieurs liens vers des politiques hébergées en externe et configurer la récurrence afin que les utilisateurs soient sollicités selon un calendrier qui correspond aux exigences internes. Toutes les actions liées aux conditions d’utilisation personnalisées sont enregistrées dans les journaux d’audit pour assurer la traçabilité.

:::note
Les Conditions d’utilisation personnalisées sont actuellement disponibles uniquement sur l’application Web et les navigateurs.
:::

## Avantages clés

- Afficher les conditions d’utilisation dans l’ensemble de votre organisation.
- Présenter le dialogue des conditions d’utilisation personnalisées aux points d’utilisation pertinents : après une connexion réussie ou lors d’une interaction avec Miro IA.
- Imposer l’acceptation par l’utilisateur selon un calendrier que vous configurez (jours, semaines ou mois), ou lors de mises à jour.
- Lier jusqu'à trois politiques hébergées en interne ou en externe, dans la langue ou le format de votre choix.
- Maintenir l’auditabilité dans les journaux d’audit.

## Portée

- S'applique à : utilisateurs internes uniquement, tous les membres et admins de l’organisation.
- Exclus : invités et collaborateurs externes.
- Déclencheurs :
  - Connexion réussie : affiché immédiatement après une connexion.
  - Utilisation de Miro IA : affiché lorsqu'un utilisateur interagit avec Miro IA (par exemple, en basculant la disposition de l'IA, en ouvrant le panneau latéral de l'IA, ou en lançant une action d'IA comme le partenaire d’IA).
- Récurrence : configurable par l'admin en jours, semaines ou mois. Chaque condition d’utilisation personnalisée a son propre état et récurrence. Par défaut : deux semaines.
- Format des conditions : le contenu doit être hébergé à l'extérieur. Miro fait référence aux liens et ne stocke pas le texte intégral de la politique.
- Liens : jusqu'à trois liens vers des politiques, chacun avec un libellé clair.
- Configuration : vous pouvez configurer une condition d’utilisation personnalisée pour chaque déclencheur (connexion réussie et utilisation de Miro IA). Chaque condition d’utilisation personnalisée a son propre état et sa récurrence.

## Qui peut utiliser cette fonctionnalité ?

Les admins doivent avoir les privilèges Enterprise Guard suivants pour consulter et gérer les conditions d’utilisation personnalisées :

- **Admin du contenu sensible :** dispose de permissions intégrées.
- **Rôles d'admin personnalisés**, doivent inclure :
  - Consulter les conditions d’utilisation personnalisées
  - Gérer les conditions d’utilisation personnalisées

## Fonctionnement

1. **Configurer les conditions :** choisissez le déclencheur (connexion réussie ou utilisation de l'IA), la portée (membres internes) et la récurrence.
2. **Ajouter du contenu :** fournissez un titre concis, une courte description et jusqu'à trois liens étiquetés vers des politiques hébergées à l'externe.
3. **Examiner et activer :** prévisualisez le dialogue utilisateur final et activez la configuration.
4. **Application :**

- **Connexion réussie :** la fenêtre de dialogue ne peut pas être fermée. Les utilisateurs doivent accepter pour continuer ou se déconnecter.
- **Utilisation de l'IA :** la fenêtre de dialogue permet **Continuer** ou **Annuler**. Annuler maintient l'utilisateur connecté avec les fonctionnalités IA désactivées.

5. **Enregistrement :** les modifications de configuration et les acceptations des utilisateurs sont consignées dans les journaux d'audit.

### Expérience utilisateur

- **Connexion réussie**

  - La fenêtre de dialogue apparaît immédiatement après la connexion.
  - Les utilisateurs peuvent cliquer sur **Continuer** pour accepter et continuer, ou **Se déconnecter**.
- **Utilisation de l'IA**

  - Le dialogue apparaît lorsque l'utilisateur interagit avec Miro IA, par exemple en basculant la mise en page IA, en ouvrant le panneau latéral IA, ou en démarrant un outil ou une action IA (par exemple, partenaire d’IA).
  - Les utilisateurs peuvent cliquer sur **Continuer** pour accepter et utiliser les fonctionnalités IA. Si les utilisateurs cliquent sur **Annuler**, ils restent connectés et peuvent continuer à utiliser toutes les fonctionnalités non-IA.
- Les utilisateurs ne sont pas de nouveau invités à accepter tant que la période de récurrence n’est pas terminée ou que les conditions ne sont pas mises à jour.

## Comportement d'acceptation

- **Déclencheur de connexion :** les utilisateurs doivent accepter selon le calendrier configuré ou se déconnecter. La boîte de dialogue ne peut pas être contournée.
- **Déclencheur d'utilisation de l'IA :** les utilisateurs peuvent accepter pour activer les fonctionnalités d'IA ou annuler pour garder les fonctionnalités d'IA désactivées. L'annulation garde l'utilisateur connecté et capable d'utiliser les fonctionnalités non liées à l'IA.
- **Récurrence et versions :** les utilisateurs ne sont pas invités de nouveau avant la fin de la période de récurrence ou qu'une nouvelle version soit publiée, selon le déclencheur configuré.

##

###
