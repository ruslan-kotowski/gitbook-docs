---
title: Cartes Azure
article_id: 360033799934
translation_id: 360033799934
locale: fr
sidebar_position: 4
created_at: '2019-08-13T10:01:30Z'
updated_at: '2025-11-25T16:05:13Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: azure-cards
availability:
  notes: 'Personnes: Tous les utilisateurs Forfaits: Business, Enterprise Plateformes:
    Navigateur, Bureau, Mobile'
---

Les cartes Azure vous permettent d'importer des éléments de travail depuis Azure Boards (une branche des services Azure DevOps, anciennement VSTS - solution cloud) vers vos tableaux Miro. Elles peuvent se révéler essentielles pour vos rétrospectives à distance, l'évaluation des histoires, la priorisation du backlog, la cartographie de récits et d'autres activités d'équipe. Vous pouvez également les utiliser dans les frameworks Miro Kanban et User story mapping.

Les cartes Azure enrichissent votre expérience Miro en s'intégrant directement avec Azure Boards, permettant une gestion fluide des flux de travail pour diverses activités d'équipe.

## Fonctionnalités clés

L'intégration Azure Cards offre plusieurs fonctionnalités clés :

- Importation des cartes Azure à l’aide de l’outil de sélection d’éléments de travail Azure Boards intégré à l’application. Cela inclut diverses options de tri.
- Recherche d’éléments de travail Azure Boards dans le sélecteur intégré à l’application.
- Modifications d’affichage des cartes faciles à lire en zoomant et en dézoomant.

:::note
Garantissez que vos cartes Azure sont toujours mises à jour avec le card polling, ce qui assure que les utilisateurs reçoivent toujours les mises à jour des cartes même si les [webhooks](../atlassian/14-how-to-set-up-webhooks-for-jira-data-center.md) échouent.
:::

## Configurer l’intégration des cartes Azure

Le paramétrage est nécessaire à deux niveaux :

1. L'application doit être ajoutée soit au niveau de l'organisation pour toutes les équipes, soit au niveau d'une équipe pour des équipes spécifiques.
2. Une fois l'application ajoutée, l'intégration doit être connectée et autorisée à un niveau personnel pour importer des cartes Azure.

Ce processus nécessite des autorisations administratives spécifiques à la fois dans Miro et Azure DevOps.

:::note
Pour configurer avec succès les cartes Azure avec Miro, **le même compte doit être admin Azure et admin Miro**.

Bien que l’ajout de cartes Azure nécessite des autorisations d'admin d'équipe ou d'entreprise Miro **et** des autorisations de groupe d'admin de la collection de projets dans Azure Boards, ces autorisations peuvent être rétrogradées une fois la connexion terminée. L'administrateur ne peut cependant pas être supprimé et doit conserver l'accès au projet Azure.
:::

### Ajouter des cartes Azure pour votre organisation ou équipe

Les admins d’entreprise Miro peuvent ajouter des cartes Azure pour toutes les équipes, tandis que les admins d’équipe peuvent les ajouter pour des équipes spécifiques qu’ils gèrent. Cette étape rend l'application Cartes Azure disponible pour la connexion.

:::note
Pour connecter les cartes Azure au niveau de l’équipe, vous devez être un admin d’équipe.
:::

1. Rendez-vous dans vos **Paramètres du profil** (cliquez sur l'icône de hamburger du menu principal et choisissez **Paramètres du profil**, ou depuis le tableau de bord, cliquez sur votre avatar dans le coin supérieur droit et choisissez **Paramètres**).
2. Cliquez sur **Applications**, puis naviguez jusqu’à l’onglet **Ajouter des applications** sur le côté droit.
3. Saisissez « Azure Cards » et sélectionnez-le dans la liste déroulante. Cliquez sur **Ajouter**.
4. Dans la boîte de dialogue suivante, choisissez soit **Toutes les équipes**, soit **Dans les équipes spécifiques** (choisissez votre équipe si nécessaire), puis cliquez sur **Étape suivante**.
5. Sur l'écran « Vérifiez et ajoutez Cartes Azure », cliquez sur **Ajouter**. L’application sera ajoutée pour votre entreprise ou votre équipe.
6. Rendez-vous dans l’onglet **Gérer les applications**, recherchez Azure Cards et cliquez sur **Approuver**. L’application sera maintenant approuvée au niveau de l’entreprise ou de l’équipe.
7. Ensuite, connectez votre organisation Azure à Miro. Dans le panneau Applications, allez dans **Gérer les applications.**
8. Recherchez « Azure Cards » dans votre liste d’applications et cliquez sur **Paramètres.**
9. Dans le panneau des paramètres pour les cartes Azure, ajoutez l'URL de votre **instance Azure** et cliquez sur **Connecter**. Saisissez vos identifiants de connexion Microsoft Azure.
10. Dans la boîte de dialogue d’autorisation, cliquez sur **Accepter** pour terminer la connexion d’Azure à Miro.

### Appliquer des paramètres personnalisés pour Cartes Azure à des équipes spécifiques

Si vous avez besoin de paramètres différents pour des équipes spécifiques par rapport à la configuration globale au niveau de l'entreprise, les admins d'équipe peuvent configurer cela dans la zone **Applications et intégrations** de l'équipe.

1. À partir de la page de paramètres de votre profil, cliquez sur **Équipes**.
2. Cliquez sur l’équipe à laquelle vous souhaitez appliquer les paramètres personnalisés.
3. Dans le panneau Équipes, cliquez sur **Applications et intégrations**.
4. Trouvez **Cartes Azure** et cliquez dessus.
5. Dans le panneau des paramètres de l'application, choisissez **Appliquer des paramètres personnalisés** dans le menu déroulant à droite, puis connectez le compte Azure dont vous souhaitez personnaliser les paramètres.
6. Autorisez Miro dans Azure DevOps avec votre compte Microsoft : cliquez sur **Connecter** à côté de « Compte Microsoft » et connectez-vous à votre compte Microsoft, ce qui permet à Miro de l’utiliser.
7. Saisissez votre **URL d’organisation Azure** (qui peut être copiée à partir d’Azure DevOps) et cliquez sur **Se connecter.** Miro acceptera soit l'URL personnalisée de votre instance, soit l'adresse générale `https://dev.azure.com/` se terminant par le nom de votre instance.
   ![Animation montrant comment appliquer des paramètres personnalisés pour Cartes Azure à une équipe spécifique.](../../../../../../docs/integrations-apps/microsoft/images/21017013136658_azure_cards_custom_team_settings.gif)
   *Ajout de paramètres personnalisés pour Cartes Azure à des équipes spécifiques*

### Connectez votre compte Azure personnel pour utiliser les cartes Azure.

Après qu'un administrateur Miro ait installé et approuvé l'application, chaque membre de l'équipe qui souhaite utiliser les cartes Azure doit personnellement autoriser la connexion à son compte Azure. Ceci personnalise le sélecteur de cartes et permet l'importation de tous les éléments de travail Azure auxquels l'utilisateur peut accéder.

Vous pouvez trouver l’icône Azure Cards dans la barre d’outils de création. Si l'icône n'est pas là, il se peut que vous deviez la rechercher :

1. Dans la barre de création, sélectionnez **Outils, médias et intégrations** (**+**).
   Le panneau **Outils, médias et intégrations** s’ouvre.
2. Dans l’onglet **Outils**, recherchez et sélectionnez Cartes Azure.

Pour connecter votre compte :

1. Cliquez sur l'icône Cartes Azure dans la barre d’outils. Une fenêtre contextuelle vous demandera d'**Autoriser**.
2. Cliquez sur le bouton **Autoriser** et cliquez sur **Continuer**. Vous serez amené à la page Paramètres de l’équipe > Applications et intégrations.
3. Utilisez le panneau des paramètres de l’application pour connecter votre compte Microsoft à Miro et indiquer l’instance Azure que vous souhaitez utiliser. Cette URL peut être copiée à partir d’Azure DevOps ; Miro accepte soit l’URL personnalisée de votre instance, soit l’adresse générale `https://dev.azure.com/` se terminant par le nom de votre instance.
   ![Spécification de l'URL de l'organisation Azure dans les paramètres de l'application Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017013107730_org%20URL.jpg)

:::note
Notez que seuls les admins d’équipe peuvent configurer les paramètres initiaux au niveau de l’équipe ou de l’entreprise. Si vous ne voyez pas le bouton **Connecter** pour l'URL de l'organisation Azure lors de la configuration de l'administration, assurez-vous de disposer des [droits d'admin d'équipe pour l'équipe](../../administration/user-management/06-how-to-manage-admin-roles.md).
:::

## Importer des éléments de travail Azure dans un tableau Miro

Une fois que l'application Azure Cards est configurée et que vous avez connecté votre compte personnel, vous pouvez importer les éléments de travail Azure vers n'importe quel tableau Miro associé à l'équipe connectée. Il existe deux façons principales de procéder :

- Copiez l'URL de l'élément de travail Azure et collez-la directement sur le tableau Miro. L'élément se transformera automatiquement en carte Azure.
- Utiliser le sélecteur de cartes Azure : Cliquez sur l'icône **Cartes Azure** dans la barre d'outils pour ouvrir le sélecteur.

  ![Azure Cards picker interface in Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017013109010_Azure%20cards%20picker.jpg)*Sélecteur de cartes Azure*

  Le sélecteur prend en charge la recherche dans tous les champs, ce qui vous permet de trouver une carte par son titre, son type, son état, etc. Vous pouvez également utiliser la [recherche par mots-clés](https://docs.microsoft.com/azure/devops/project/search/get-started-search?view=azure-devops#start-your-search-with-a-keyword) robuste fournie par Microsoft.

  ![Animation showing search functionality within the Azure Cards picker.](../../../../../../docs/integrations-apps/microsoft/images/21017013114002_Azure%20Cards%20picker.gif)*Rechercher des cartes Azure dans le sélecteur*

  Vous pouvez filtrer les cartes par projet, destinataire, type, zone et état, ce qui déverrouille le filtrage avancé des éléments de travail Azure directement dans Miro.

  ![Filtering options within the Azure Cards picker.](../../../../../../docs/integrations-apps/microsoft/images/21017013116306_filter.jpg)*Filtre des cartes Azure dans le sélecteur*

  Pour naviguer vers l'élément de travail Azure original, sélectionnez une carte sur le tableau et cliquez sur le bouton **Source** dans son menu contextuel.

  ![Source button on an Azure Card linking to the item in Azure DevOps.](../../../../../../docs/integrations-apps/microsoft/images/21017042632338_card%20spurce.jpg)*Le bouton source de la carte*

  Les cartes Azure peuvent être utilisées comme widgets autonomes de tableau ou comme composants des structures interactives [Kanban](../../using-miro/advanced-tools/02-columns-formerly-kanban.md) et [User Story Map](../../using-miro/advanced-tools/07-user-story-mapping.md). Vous pouvez ajouter des cartes Azure à ces structures en les faisant glisser à l’intérieur.

  ![Animation showing Azure Cards being used within a Miro Kanban board.](../../../../../../docs/integrations-apps/microsoft/images/21017042632850_Azure%20cards%20and%20kanban.gif)*Travailler avec les cartes Azure dans Kanban*

## Créez et modifiez des cartes Azure directement dans Miro

L’intégration bidirectionnelle entre Miro et Azure DevOps permet aux équipes de créer de nouveaux éléments de travail Azure et de modifier les existants directement depuis un tableau Miro. Vous pouvez également convertir les cartes Miro et les pense-bêtes existants en cartes Azure.

### Créer une nouvelle carte Azure

Pour créer un nouvel élément de travail Azure depuis Miro :

1. Sélectionnez **Cartes Azure** dans la barre d’outils de création et choisissez **Créer un élément de travail** en haut à droite de l’outil de sélection.
2. Remplissez les champs de la carte, choisissez un projet, un type d'objet, un destinataire et cliquez sur **Créer**. Le nouvel élément sera créé dans votre répertoire Azure DevOps ainsi que sur votre tableau Miro.

![Animation showing the process of creating a new Azure Card from Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017042635282_create%20an%20Azure%20Card.gif)*Création d’une carte Azure dans Miro*

### Convertir les cartes ou pense-bêtes Miro en cartes Azure

Pour convertir une carte Miro ou un pense-bête existant en carte Azure :

1. Sélectionnez le pense-bête ou la carte sur le tableau.
2. Cliquez sur l'option de conversion (généralement une icône Azure DevOps ou "Convertir en élément de travail Azure") dans le menu contextuel de l'objet.
3. Définissez les paramètres de la carte (comme le projet, le type d’objet) dans la boîte de dialogue et cliquez sur **Convertir**. Le texte figurant sur le pense-bête/la carte deviendra le titre de la carte.

> **💡** Gagnez du temps en convertissant en bloc des pense-bêtes ou des cartes Miro en cartes Azure. Cliquez et faites glisser pour sélectionner tous les objets que vous souhaitez convertir, puis dans le menu contextuel, sélectionnez **Convertir en éléments de travail Azure**.

![Converting a Miro sticky note into an Azure Card.](../../../../../../docs/integrations-apps/microsoft/images/21017013125650_convert%20a%20sticky%20into%20an%20Azure%20Card.jpg)*Conversion d’un pense-bête en carte Azure*

### Modifier une carte Azure

L’option permettant de modifier les cartes Azure dans Miro vous évite de devoir passer d’un outil à l’autre. Pour modifier une carte :

1. Cliquez sur la carte Azure sur votre tableau Miro.
2. Cliquez sur l'**icône du stylo (modifier)** dans le menu contextuel de la carte. Une fenêtre contextuelle s'ouvrira, vous permettant de modifier les champs de l'élément.
3. Cliquez sur **Mettre à jour** pour enregistrer les modifications. Les changements seront également répercutés dans Azure DevOps.

![Editing an Azure Card's details directly within Miro.](../../../../../../docs/integrations-apps/microsoft/images/21017042639890_edit%20an%20Azure%20card.jpg)*L’option pour éditer une carte Azure dans Miro*

### Modifier la couleur de la carte Azure

Pour personnaliser l'apparence de vos cartes Azure sur le tableau :

Pour modifier la couleur de remplissage d’une carte, cliquez sur la ou les cartes et choisissez **Couleur de remplissage** dans le menu contextuel. Si vous dupliquez la ou les cartes, toutes les copies suivantes auront la même couleur de remplissage.

## Désinstaller l’intégration des cartes Azure

Si vous n’avez plus besoin de l’intégration des cartes Azure, vous pouvez la désinstaller. La désinstallation au niveau de l’équipe nécessite des autorisations d’admin d’équipe.

1. Rendez-vous sur **Paramètres de l’équipe > Applications et intégrations > Cartes Azure**.
2. Faites défiler vers le bas et cliquez sur **Désinstaller pour l’équipe.**
3. Pour désinstaller les cartes Azure uniquement pour votre compte personnel, cliquez sur **Désinstaller pour moi.**

![Options to uninstall Azure Cards for the team or for an individual user.](../../../../../../docs/integrations-apps/microsoft/images/21017042628370_uninstall%20Azure%20cards.jpg)*Désinstaller l'application pour toute l'équipe ou seulement pour vous*

## Champs pris en charge pour la carte Azure

Les champs suivants sont pris en charge pour les cartes Azure dans Miro :

- Titre
- Projet
- Type
- État
- Description (la modification n'est pas prise en charge)
- WI parent
- Responsable
- Priorité
- Story Points
- Zone
- Itération
- Critères d’acceptation

Les champs personnalisés ne sont pas pris en charge.

## Résolution des problèmes des cartes Azure

Si vous rencontrez des problèmes avec l’intégration des cartes Azure, consultez les problèmes courants et leurs solutions ci-dessous.

L’URL n’est pas valide.

L’URL que vous avez utilisée n’est pas correcte. Vérifiez l’orthographe et la mise en forme. L’adresse de l’organisation Azure doit, par exemple, se terminer par une barre oblique.

L’URL de l’organisation Azure n’est pas accessible.

L’URL saisie n’existe pas. Veuillez entrer l’URL existante ou vérifier si vous n’avez pas fait de faute de frappe. Vérifiez également ce qui suit :

- Assurez-vous que votre organisation peut accepter l’autorisation de tiers : dans **Paramètres de l'organisation > Stratégies (Sécurité)** **>** assurez-vous que l'option "Accès d’applications tierces via OAuth" est activée.
- Votre organisation Azure se trouve sur un réseau privé/le pare-feu de votre entreprise bloque les connexions réseau externes. Veuillez effectuer les modifications nécessaires dans la configuration de votre pare-feu et de votre VPN en ajoutant nos domaines à votre liste d'autorisations : miro.com*, *.miro.com, mirostatic.com*, *.mirostatic.com, realtimeboard.com*, *.realtimeboard.com, *static.miro-apps.com. Si vous utilisez un proxy, configurez un proxy inverse pour nous octroyer un accès. Veillez à remplir le champ **URL Azure DevOps** dans les paramètres avec l'adresse à laquelle nous pouvons accéder (l'adresse peut différer de l'adresse réelle de votre Azure DevOps restreint). Vous pouvez également prolonger la valeur du délai d’expiration sur votre serveur proxy.
- Toutes les demandes d’intégration passent par un équilibreur de charge Amazon, donc il n’est pas possible de fournir des informations réseau spécifiques depuis Miro.

Échec de la création de l’abonnement au hook de service.

L’utilisateur Azure dont la session est actuellement ouverte ne dispose pas des autorisations nécessaires. L’utilisateur Azure pour lequel l’instance Azure sera connectée à Miro doit avoir accès à ces méthodes d’API REST :

- [*Création d’un abonnement au hook de service*](https://docs.microsoft.com/rest/api/azure/devops/hooks/subscriptions/create?view=azure-devops-rest-6.0) (portée « *vso.serviceendpoint_manage* » [portée](https://docs.microsoft.com/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes) requise)
- [*Réception des métadonnées des projets (ces informations sont utilisées pour spécifier correctement les éléments de travail dans les événements d’abonnement)*](https://docs.microsoft.com/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0)
- *Les méthodes suivantes doivent également être accessibles à tous les utilisateurs de l’intégration :*
  - [*Obtenir les éléments*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/get%20work%20item?view=azure-devops-rest-6.0)
  - [*Lister les éléments*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20items/list?view=azure-devops-rest-6.0)
  - [*Obtenir les types d'éléments*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/get?view=azure-devops-rest-6.0)
  - [*Énumérer les types d'éléments*](https://docs.microsoft.com/rest/api/azure/devops/wit/work%20item%20types/list?view=azure-devops-rest-6.0)

L’utilisateur **username@microsoft.com** n’a accès à aucun projet dans l’URL de l’organisation Azure spécifiée.

Vous ne pouvez accéder à aucun projet dans l’organisation Azure utilisée. Pour importer des cartes, vous devez avoir accès aux cartes du côté d’Azure Boards. Contactez le propriétaire de l’organisation Azure et demandez-lui de vous inviter dans l’organisation Azure. [Cet article](https://docs.microsoft.com/azure/devops/organizations/security/look-up-organization-owner?view=azure-devops) peut vous aider à découvrir le nom du propriétaire de l’organisation.

Échec de la création de l’abonnement au crochet de service : l’utilisateur **username@microsoft.com** n’est pas un propriétaire d’organisation. Demandez à votre propriétaire de l’organisation de paramétrer cette étape.

Vous devez être à la fois propriétaire de l’organisation Azure et admin d’entreprise Miro pour paramétrer les cartes Azure dans Miro.

L’autorisation a expiré. Reconnectez l’intégration dans les paramètres de votre équipe.

L’autorisation Azure a expiré. Reconnectez l'intégration au niveau personnel, comme décrit dans la section « Connectez votre compte Azure personnel pour utiliser les cartes Azure » ci-dessus.

La carte avec laquelle vous travaillez présente un comportement inattendu.

Cela peut se produire si la carte a été désynchronisée de l’organisation Azure. Par exemple, si vous avez copié la carte à partir d’un autre tableau ou si vous travaillez sur un tableau qui a été déplacé entre des équipes. Pour résoudre ce problème, ajoutez à nouveau l’élément Azure dans le tableau.

Le nombre d’éléments de travail renvoyés dépasse la limite de 200. Modifiez la requête pour obtenir moins d’éléments.

Si vous recevez ce message d’erreur, cela signifie que vous avez sélectionné trop de tâches à ajouter au tableau sous forme de cartes. Limitez le nombre de tâches en utilisant la barre de recherche. Pour le moment, lorsque vous ouvrez le sélecteur, aucun filtre n’est appliqué et toutes les tâches des trois derniers mois sont affichées. Chaque fois que l'outil de sélection essaie d'afficher plus de 200 tâches, vous recevrez ce message d’erreur.

Je n’obtiens pas le bouton **Connecter** lorsque j’essaie de connecter mon organisation Azure avec Miro dans les paramètres de Miro.

Vérifiez que vous disposez des droits d’admin d’équipe. Rendez-vous dans l’onglet **Utilisateurs actifs** des paramètres de l’équipe et [octroyez-vous le rôle d’admin d’équipe](../../administration/user-management/06-how-to-manage-admin-roles.md) si nécessaire. Cela s'applique à la configuration initiale de la connexion à l'organisation Azure par un administrateur.

:::note
Si vous rencontrez d’autres problèmes, contactez le [service d’assistance de Miro](../../using-miro/tools/troubleshooting/06-contacting-miro-support.md).
:::

## Foire aux questions sur les cartes Azure

Voici des réponses aux questions les plus fréquentes sur l'intégration des cartes Azure.

Quelles adresses IP doivent être autorisées pour les cartes Azure ?

Pour que l'intégration des cartes Azure fonctionne correctement, surtout dans des environnements réseau restreints, vous devrez peut-être ajouter à la liste d’autorisations les adresses IP suivantes :

- 18.203.61.162
- 54.220.74.201
- 54.216.81.236
- 54.73.153.141
- 52.215.228.26
- 52.16.47.17
- 54.217.180.21

Qu’arrive-t-il aux cartes Azure existantes lorsque vous déconnectez et désinstallez l’application Cartes Azure ?

Les cartes restent intactes sur les tableaux Miro sans perte de données ; cependant, elles cessent de se synchroniser avec Azure et le bouton source disparaît.
