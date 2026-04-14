---
title: Vue d'ensemble de la mise en suspens juridique
article_id: 21922434361618
translation_id: 21922434361618
locale: fr
sidebar_position: 1
created_at: '2024-10-11T12:20:34Z'
updated_at: '2025-11-25T15:48:02Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ediscovery-legal-hold
---

La fonctionnalité de mise en suspens juridique est conçue pour soutenir les processus de conformité et d'eDiscovery en préservant les tableaux soumis à enquête ou pertinents pour des affaires juridiques en cours.

[Les admins eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) peuvent empêcher la suppression définitive de contenu en créant des rétentions légales basées sur des utilisateurs spécifiques et leurs actions dans Miro. Cette fonctionnalité est essentielle pour garantir que les informations pertinentes soient conservées et sécurisées pendant les procédures judiciaires.

Par exemple, lorsqu'un utilisateur soumis à un ordre de préservation légale interagit avec un tableau, ce tableau est automatiquement mis en attente pour éviter sa suppression définitive.

De plus, toutes les versions du tableau sont également conservées, assurant que le contenu du tableau est préservé à des fins légales.

![legalholdoverview.png](images/22388722731538_legalholdoverview.png)

:::note
Vous devez avoir le rôle d'[administrateur eDiscovery](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) pour effectuer les tâches de conservation légale.</span> Pour demander le rôle d’administrateur de l'eDiscovery, contactez l’admin de votre entreprise.
:::

## Principaux avantages de la mise en suspens juridique

- **Préservation de l’information :** La mise en suspens juridique garantit que toutes les données pertinentes sont préservées, empêchant leur suppression définitive. Ceci est crucial pour la conformité et les enquêtes légales, car cela garantit que les données présentées dans les affaires judiciaires restent exactes et inchangées.
- **Respect des exigences légales :** Legal Hold aide les organisations à respecter les obligations légales et réglementaires en veillant à ce que les informations nécessaires soient conservées et disponibles lorsque cela est requis, contribuant ainsi à éviter des sanctions ou des litiges.
- **Atténuation des risques :** En protégeant les données importantes, Legal Hold réduit le risque de perte de données pouvant entraîner des conséquences juridiques ou financières significatives.
- **Audit et Surveillance :** Chaque fois qu'un blocage légal est créé ou modifié, un journal d'audit est généré, offrant une visibilité et une traçabilité complètes. Tous les journaux d'audit d'une organisation sont conservés indéfiniment lorsqu'au moins une conservation légale est active. Cela garantit la responsabilité et la transparence dans la gestion des mises en suspens juridiques.

## Comment fonctionne la mise en suspens juridique

- **Interactions avec l'utilisateur ou le tableau :** Lorsqu'un utilisateur sous mise en suspens juridique ouvre, modifie ou interagit de quelque manière que ce soit avec un tableau (en le renommant ou en ajoutant du contenu), ce tableau est signalé et conservé. Par exemple, si le nom du tableau est modifié ou si le contenu est mis à jour, il sera automatiquement placé en conservation légale. De plus, la propriété des tableaux et la création de tableaux sont mises en attente.

  Lorsqu'une mise en suspens juridique est créée, elle s'applique aux tableaux que les dépositaires ont créés, possédés ou copossédés au moment de la mise en suspens. En outre, tous les tableaux que les responsables accèdent et modifient après la mise en place de la rétention sont également inclus. Les détails d'accès et de mise à jour historiques des tableaux ne sont pas disponibles dans cette version.
- **Actions des utilisateurs finaux et suppression de tableaux :** Bien que les utilisateurs finaux puissent supprimer des tableaux, ces tableaux sont conservés si une suspension légale est en place. Ils restent inaccessibles à l'utilisateur final mais sont conservés à des fins légales et administratives.
- **Contrôle Administratif :** les admins eDiscovery peuvent créer et supprimer des mises en suspens juridiques dans la section eDiscovery des paramètres. Les blocages légaux peuvent être appliqués à tous les tableaux qu'un utilisateur a créés, possédés, copossédés, édités ou consultés. Pour gérer plusieurs mises en suspens juridiques, les administrateurs peuvent d'abord créer un dossier sous lequel ces mises en suspens sont regroupées.
- **Suppression d’équipe :** Si un tableau est mis en suspens dans une équipe, cette équipe ne peut pas être supprimée définitivement jusqu'à ce que la suspension soit levée. Cela empêche toute perte de données non intentionnelle, garantissant ainsi que tout le contenu pertinent est préservé. Dans les cas où une équipe est supprimée mais contient un tableau sous conservation légale, l'équipe sera marquée comme préservée sur la page des équipes supprimées, et sa suppression permanente sera désactivée jusqu'à ce que la conservation légale soit levée.
- **Point de vue de l’administrateur et d’eDiscovery :** Bien que les utilisateurs finaux ne puissent pas accéder ou récupérer un tableau supprimé qui est en attente, les administrateurs et les équipes eDiscovery peuvent toujours interagir avec celui-ci. Le tableau est conservé jusqu'à la clôture du dossier juridique, moment auquel la mise en suspens légale peut être levée, et le tableau peut être définitivement supprimé.
- **Fonctionnalité d'exportation du tableau :** Les tableaux en cours de blocage juridique peuvent encore être exportés en utilisant la fonctionnalité d'exportation de tableau, permettant ainsi de collecter facilement les données pertinentes pour les affaires juridiques.
- **Déplacement des tableaux :** Les tableaux mis en suspens ne peuvent pas être déplacés en dehors de l'organisation. Si un tableau est sous "legal hold", les équipes externes sont automatiquement exclues de la liste des équipes vers lesquelles le tableau peut être déplacé.
