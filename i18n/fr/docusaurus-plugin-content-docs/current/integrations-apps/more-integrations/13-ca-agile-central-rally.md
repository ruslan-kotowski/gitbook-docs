---
title: "CA\_Agile Central (Rally)"
article_id: 360017731133
translation_id: 360017731133
locale: fr
sidebar_position: 4
created_at: '2019-02-11T10:13:34Z'
updated_at: '2025-11-25T16:02:49Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: rally-cards
---

Directement sur le tableau, profitez des avantages du logiciel et de la méthodologie agiles et de pointe proposés par CA. Convertissez vos tâches de CA Agile Central en cartes pratiques et profitez de la hiérarchisation des backlogs (arriérés), de la cartographie des récits et d’autres activités de groupe qui aident votre équipe à développer rapidement des projets cohérents et de qualité.

> **Disponible pour :** [le forfait Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)

## Connecter CA Agile

L’autorisation CA Agile est effectuée via le protocole OAuth 2.0 (octroi de code d’autorisation) et toutes les demandes sont transmises par le protocole SSL. Il existe deux niveaux de connexion de vos données Miro et de votre compte CA Agile Central : le niveau de profil utilisateur et le niveau de l’équipe.

Il est important de noter que la connexion à CA Agile est à sens unique : CA Agile --> Miro. Vous pouvez importer les cartes sur un tableau Miro et les modifier via le bouton Source, décrit ci-dessous dans la section Modifier les cartes. Vous ne pouvez pas modifier les cartes CA Agile directement dans Miro.

### Niveau équipe

> **Configuré par :** les admins d’équipe

:::warning
Notez que, pour chaque équipe dans Miro, vous devrez utiliser des comptes d’utilisateurs Rally différents pour connecter la même instance Rally.
:::

Pour établir la connexion au niveau de l’équipe, l’admin d’équipe devra trouver l’application **CA Agile** dans le [Marketplace de Miro](https://miro.com/marketplace/) et l’installer pour l’équipe : cliquez sur **Obtenir l’application**, puis sélectionnez une équipe et cliquez sur **Installer et autoriser**.

![install_Rally_for_a_team.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416392594_install%20Rally%20for%20a%20team.jpg)
*Installation de Rally pour une équipe*

Vous pouvez également installer l’application à partir d’un tableau :

1. Dans la barre de création, sélectionnez**Outils, médias et intégrations** (**+**).Le panneau **Outils, médias et intégrations** s’ouvre.
2. Dans l’onglet **Outils**, recherchez et sélectionnez CA Agile.
   Le panneau **CA Agile** s’ouvre.

![ca-agile-entry-point.png](../../../../../../docs/integrations-apps/more-integrations/images/21537455155858_ca-agile-entry-point.png)
*Installer l’application à partir d’un tableau*

Ouvrez ensuite les **paramètres de l’équipe > Applications et intégrations** et **connectez**l’intégration à partir de là. Si vous n’avez pas les permissions requises dans Rally, il vous sera proposé de vous connecter à votre compte Rally.

![connect_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416393874_connect%20Rally.jpg)
*Connection de l’intégration au niveau de l’équipe*

Pendant cette configuration, un webhook est créé du côté de Rally, qui envoie ensuite à Miro des mises à jour pour les cartes importées.

Lorsque l’intégration est paramétrée au niveau de l’équipe, tout membre de l’équipe peut voir les cartes Rally importées par d’autres participants sur les tableaux et l’état actuel des cartes.

Notez que le compte Rally utilisé lors de la mise en place de l’intégration au niveau de l’équipe doit avoir accès à tous les projets Rally à partir desquels les cartes seront importées. Si un projet Rally n’est pas accessible pour ce compte Rally, les cartes importées de ce projet ne seront donc pas mises à jour sur le tableau et seront affichées comme figées pour tous les utilisateurs de l’équipe.

### Niveau profil

> **Configuré par :** chaque utilisateur

:::warning
Avant de connecter l’intégration, assurez-vous de vous connecter à Rally dans un onglet séparé du navigateur.
:::

Si un utilisateur ou une utilisatrice a besoin de pouvoir importer soi-même des cartes Rally sur le tableau, cette personne doit configurer l’intégration au niveau de son profil également. Pour connecter votre profil Miro, ouvrez [Profile settings](https://miro.com/app/account/profile/) (Détails du profil), basculez sur **Integrations** (Intégrations), trouvez **CA Agile Central (Rally)** et cliquez sur **Connect** (Se connecter) :

![connect_Rally_on_profile_level.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429433746_connect%20Rally%20on%20profile%20level.jpg)
*Connecter l’intégration au niveau du profil*

Lorsque la connexion au niveau du profil est établie, l’utilisateur ou l’utilisatrice peut utiliser l’icône Rally sur sa barre d’outils et ouvrir le sélecteur de bibliothèque Rally. L’utilisateur ou l’utilisatrice peut voir tous les éléments Rally (user stories, tâches, défauts) disponibles pour le compte Rally utilisé pour configurer l’intégration au niveau du profil. En d’autres termes, en utilisant le sélecteur Rally, l’utilisateur ou utilisatrice ne pourra importer que les éléments qui sont à sa disposition dans Rally.

## Ajouter des cartes CA Agile au tableau

Pour ajouter une carte sur le tableau, il suffit de copier l’adresse URL de la tâche et de la coller sur le tableau (les [combinaisons de raccourcis](https://help.realtimeboard.com/support/solutions/articles/1000206698-shortcuts-hotkeys) standard fonctionnent également).

Pour filtrer les tâches ou ajouter plusieurs cartes, choisissez**CA Agile**dans la barre d’outils de création.

Vous verrez le sélecteur de CA Agile Central, où vous pouvez définir les filtres de recherche tels que projet, type, itération, parution, etc. Choisissez-en un ou plusieurs et cliquez sur **Exporter** :

![Rally_picker.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416397714_Rally%20picker.jpg)
*Sélecteur de CA Agile Central*

Les tâches seront ajoutées au tableau automatiquement. Si le nom de la tâche est long, faites glisser le bas de la carte pour le voir en entier.

*![Rally_cards_on_the_board.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398482_Rally%20cards%20on%20the%20board.jpg)
Cartes Rally sur le tableau*

> À noter que l’intégration Rally de Miro n’offre pas la possibilité de créer ni de modifier directement les cartes Rally dans Miro.

## Modifier des cartes

Pour modifier le contenu d’une carte, veuillez cliquer sur le lien source de la carte :

![Rally_card_source.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017416398866_Rally%20card%20source.jpg)
*L’icône de modification sur la carte*

La tâche source sera ouverte dans un nouvel onglet où elle pourra être modifiée. Toutes les modifications sont appliquées à la carte instantanément.

## Désactiver l’intégration

Pour supprimer la connexion à vos itérations Rally, vous devez cliquer sur **Disable** (Désactiver) puis sur **Uninstall** (Désinstaller) pour cette application dans **Team settings > Apps & Integrations** (Paramètres de l’équipe > Applications et intégrations).

![uninstall_Rally.jpg](../../../../../../docs/integrations-apps/more-integrations/images/21017429436562_uninstall%20Rally.jpg)
*L’option permettant de désactiver l’intégration*

## Problèmes possibles et comment les résoudre

1. *Le sélecteur Miro-Rally n’affiche pas certains de mes projets.*
   - Notre intégration Rally utilise [le sélecteur SDK Rally](https://rally1.rallydev.com/docs/saas/apps/2.1/doc/index.html#!/api/Rally.ui.picker.project.ProjectPicker) pour remplir les données, qui ne fonctionne qu’avec les projets à l’état ouvert et n’est malheureusement pas personnalisable. Pour afficher un projet du côté de Miro, veuillez changer son état en Ouvert.
2. *Les mises à jour des cartes ou de certains champs des cartes ne passent pas par Miro*- Si vous utilisez l’intégration des cartes Rally avec plusieurs équipes Miro, vérifiez que toutes les équipes sont connectées à votre instance Rally à l’aide d’un *autre* compte utilisateur Rally. Il est possible que le problème des mises à jour dans l’équipe choisie se produise parce que les identifiants de connexion sont déjà utilisés dans Miro pour une autre équipe. Reconnectez l’intégration à l’aide de différents identifiants Rally si nécessaire.
3. *Chargement interminable lors d’une tentative d’ouverture du sélecteur Rally dans Miro.*- Suivez les étapes de dépannage ci-dessous.

   1. Ouvrez le menu Abonnement (`https://rally1.rallydev.com/#/subscription`).

   2. Cliquez sur le menu déroulant **Actions** et choisissez **Modifier**.

   3. Faites défiler vers le bas jusqu’au champ **CORS Allowed Origins**.

   4. Saisissez `https://miro.com,https://*.miro.com` (`http://miro.com`) dans le champ.

   5. Cliquez sur **Enregistrer et fermer**.
