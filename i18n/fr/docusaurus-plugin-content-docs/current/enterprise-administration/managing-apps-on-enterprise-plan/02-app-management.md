---
title: Gestion des applications
article_id: 4404659741458
translation_id: 4404659741458
locale: fr
sidebar_position: 2
created_at: '2021-08-03T15:46:50Z'
updated_at: '2026-01-29T10:00:08Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: apps-management
---

Découvrez comment gérer les applications et les autorisations au niveau de l’organisation et des équipes.

> **Pertinent pour :** Forfait Business, Forfait Enterprise
> **Qui peut le faire :** Admins d’équipe, Admins d’entreprise

### Qui peut gérer les applications ?

La gestion des applications au niveau de l’organisation est uniquement disponible pour les admins d’entreprise sur le plan Enterprise. La gestion des applications au niveau des équipes est disponible pour les admins d’équipe et d’entreprise sur les forfaits Business et Enterprise.

### Ajouter des applications pour une entreprise ou des équipes spécifiques

Ajoutez et autorisez des applications pour tous les utilisateurs d’une organisation ou pour des équipes spécifiques de votre entreprise à partir des contrôles de gestion des applications.
Rendez-vous dans les paramètres de **l'entreprise** > **Applications et intégrations** > **Applications**. Dans cette section, les admins d’entreprise peuvent ajouter des applications pour toutes ou certaines équipes.

![apps-access.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921803476626_apps-access.png)*Contrôle de gestion des applications dans les paramètres de l’entreprise*

Entrez un nom d’application ou un identifiant client dans la barre de recherche. Sélectionnez une application dans la liste déroulante et cliquez sur **Ajouter**.

![add-app.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780909714_add-app.png)*Ajouter une application à partir des paramètres de l’entreprise*

Vous pouvez ajouter l’application pour toutes les équipes de votre entreprise ou pour des équipes spécifiques. Si une application est déjà ajoutée pour certaines équipes, vous verrez l’étiquette correspondante. Si vous ajoutez à nouveau l’application pour une équipe, ses membres devront à nouveau l’autoriser. Cliquez sur **Ajouter** pour terminer.

![add-apps-where.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780917010_add-apps-where.png)
*Sélection de pour qui installer l’application Google Drive*

Si vous ajoutez une application pour toutes les équipes, elle sera également ajoutée à toutes les équipes nouvellement créées.

### Applications pré-ajoutées

Certaines applications sont déjà pré-ajoutées pour les utilisateurs. Elles peuvent exiger une autorisation supplémentaire ou une connexion individuelle. Ces applications pré-ajoutées sont : [Box](../../integrations-apps/more-integrations/05-box-legacy.md), [Dropbox](../../integrations-apps/more-integrations/06-dropbox.md), [Google Drive](../../integrations-apps/google/05-google-drive.md), [OneDrive](../../integrations-apps/microsoft/06-onedrive.md), [Smartsheet](../../integrations-apps/more-integrations/15-smartsheet-app-for-miro.md), [Azure Cards](../../integrations-apps/microsoft/03-azure-cards.md), [Jira Cards](../../integrations-apps/atlassian/03-jira-cards.md), [Brandfetch](https://miro.com/marketplace/brandfetch/), [Google Images](../../integrations-apps/google/06-google-images.md), [Slack](../../integrations-apps/more-integrations/14-slack.md). Ces applications ne seront pas pré-ajoutées si elles ne figurent pas sur la liste approuvée par l’entreprise. Vous pouvez gérer cette liste si vous êtes un admin d’entreprise.

### Préautoriser des applications pour une entreprise

Si vous ajoutez une application, vous pouvez également la pré-autoriser en même temps. Si une application est pré-ajoutée et pré-autorisée par un admin, les utilisateurs au sein de l’organisation pourront commencer à l’utiliser immédiatement. Une connexion individuelle à un service tiers peut toujours être nécessaire pour certaines applications.

Cette fonctionnalité est disponible uniquement pour les applications créées avec le SDK Web Miro. Le SDK Web Miro permet d’étendre la fonctionnalité de Miro. C’est une boîte à outils qui permet de créer des applications puissantes qui s’exécutent à l’intérieur d’un tableau Miro.

### Approuver la gestion des applications par les utilisateurs

Par défaut, les utilisateurs peuvent ajouter n’importe quelle application pour leur équipe. Les admins d’entreprise peuvent toutefois limiter la gestion des applications par les utilisateurs afin de n’autoriser l’ajout par leurs équipes que de certaines applications.

Les admins d’entreprise peuvent permettre ou limiter l’ajout de certaines applications pour leurs utilisateurs en allant dans les paramètres **Entreprise** > **Applications et intégrations** > **Applications** > **Gérer les applications** et en activant l’option **Autoriser les membres à installer les applications de cette liste uniquement**.

![manage-apps.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780921490_manage-apps.png)*Limiter les ajouts aux applications approuvées sur le forfait Enterprise*

Si cette limitation est activée, seules les applications approuvées peuvent être ajoutées par les utilisateurs Enterprise. Pour ajouter une application à la liste des applications approuvées pour les utilisateurs, activez le bouton à bascule à côté de l’application en question ou collez un identifiant client dans le champ correspondant pour approuver une application développée en interne.

Pour restreindre une application précédemment ajoutée, trouvez l’application dans la liste et assurez-vous que le bouton à côté de l’application est désactivé. Veuillez noter que les utilisateurs de toutes les équipes Enterprise ne pourront pas utiliser l’application si elle est restreinte.

Si une application est limitée dans votre entreprise, les utilisateurs pourront envoyer [des demandes d’utilisation aux admins d’entreprise](03-app-request-flow.md).

Les utilisateurs peuvent voir les applications approuvées sur le Marketplace dans les tableaux Miro stockés dans le plan Enterprise.

### Autoriser ou limiter l’utilisation d’applications dans les équipes

Les admins d’équipe et d'entreprise peuvent également gérer l'utilisation des applications au niveau de l'équipe : ils peuvent autoriser ou restreindre la possibilité pour les membres de l'équipe d'ajouter de nouvelles applications pour l’équipe. Ce paramètre est configuré séparément pour chaque équipe.

![add-apps-team.png](../../../../../../docs/enterprise-administration/managing-apps-on-enterprise-plan/images/23921780928914_add-apps-team.png)*Applications et Intégrations dans les paramètres de l'équipe*

En savoir plus sur [les applications et intégrations Miro.](../../integrations-apps/integrations-basics)
