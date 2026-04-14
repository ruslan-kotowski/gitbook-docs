---
title: Miro for Jira Cloud
article_id: 360017572414
translation_id: 7699094498322
locale: fr
sidebar_position: 4
created_at: '2022-09-19T09:27:17Z'
updated_at: '2024-09-05T14:48:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Accédez à tout ce dont vous avez besoin avec votre équipe : travaillez sur le backlog de produit avec des pense-bêtes numériques, et créez des organigrammes, des diagrammes et des wireframes. Joignez des tableaux aux tickets Jira et collaborez avec votre équipe en temps réel, comme lors d’une réunion avec un tableau blanc.

> **Disponible sur :** les forfaits Starter, Business et Enterprise
> Jira Cloud uniquement

:::note
Vous pouvez également intégrer des tableaux de Miro grâce à la fonctionnalité Atlassian Smart link.
:::

:::note
Notez que Miro propose deux types d’intégration à Jira : **Miro pour Jira Cloud** (qui permet d’intégrer des tableaux Miro du côté de Jira) et **Jira Cards**. Pour en savoir plus sur les cartes Jira, consultez [cet article.](https://help.miro.com/hc/articles/360017572434)
:::

## Comment l’installer

Le processus d’installation est le même pour tous les modules complémentaires Jira. Tout d’abord, connectez-vous à votre Jira avec des droits d’administrateur, puis téléchargez le module complémentaire [ici](https://marketplace.atlassian.com/apps/1215456/miro-for-jira-cloud?tab=overview&hosting=cloud) (l’application peut également être trouvée sur **la Marketplace Atlassian** > **Find new apps** > **Miro for Jira Cloud**) : cliquez sur **Get app**et **Get it now (Obtenir l’application maintenant)**.
Et c’est tout ! L’installation est terminée.

![Miro_pour_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134089234_Miro%20for%20Jira.jpg)
*Notification Jira sur la réussite de l’installation*

Veuillez noter qu’en tant qu’admin, vous n’avez pas besoin de relier les utilisateurs Miro aux utilisateurs Jira lors de la configuration. Chaque utilisateur devra s’autoriser dans Miro depuis Jira.

## Comment utiliser le module complémentaire

### Associer des tableaux aux tickets Jira

Pour associer un tableau à un ticket Jira, ouvrez le ticket dans Jira. Cliquez sur **Ajouter un tableau** dans la section **Tableaux Miro**.
![add_Miro_boards_in_Jira.jpg](https://help.miro.com/hc/article_attachments/21016134121362)
*Le bouton du module complémentaire apparaît après l’installation*

:::tip
S i vous n’avez pas la section des tableaux Miro, trouvez-la dans le menu contextuel du problème.
:::

![Section des tableaux Miro.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134091026_Miro%20boards%20section.jpg)
*Ajout de la section des tableaux Miro à un ticket Jira*

Un écran de sélection des tableaux Miro s’affiche. Choisissez le tableau que vous souhaitez ajouter (n’hésitez pas à changer l’équipe depuis l’écran de sélection). Si vous ne disposez pas d’une autorisation dans Miro, vous devez d’abord vous connecter.

Définissez les paramètres de partage du tableau dans le menu déroulant. Vous pouvez rendre le tableau disponible pour consultation et commentaires afin que les utilisateurs qui n’ont pas de profil dans Miro puissent également y accéder.

:::note
Pour les  utilisateurs du[forfait Enterprise](https://help.miro.com/hc/articles/360017571534) Miro, vos paramètres d’accès suivront les contrôles d’accès à l’échelle de l’organisation, ce qui peut impliquer que certaines options de partage peuvent être restreintes. En savoir plus : [Gestion de la politique de partage de l’entreprise pour les intégrations embarquées](https://help.miro.com/hc/articles/4405088016274).
:::

![embed_a_board_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134091922_embed%20a%20board%20in%20Jira.jpg)
*Partage des tableaux lors de l’attachement d’un tableau à un ticket Jira*

Notez que vous ne pouvez intégrer que des tableaux pour lesquels vous avez des droits d’édition.

Votre tableau est maintenant associé au ticket Jira que vous avez choisi :

![Miro_board_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120705810_Miro%20board%20in%20Jira.jpg)
 *Tableau Miro attaché à un ticket Jira*

### Créer des tableaux depuis Jira

Pour créer un tableau directement à partir d’un ticket Jira, cliquez sur **Add board** (Ajouter un tableau) et cliquez sur **New board** (Nouveau tableau) dans le sélecteur.

![create_a_new_board_from_the_picker.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120706322_create%20a%20new%20board%20from%20the%20picker.jpg)
*Création d’un tableau à partir du sélecteur*

### Consulter, commenter et modifier les tableaux

Cliquez simplement sur un tableau pour le visualiser, le commenter ou le modifier en fonction des droits d’accès dont vous disposez. La fenêtre du tableau s’ouvre en superposition, ce qui vous permet de travailler et de collaborer comme si vous étiez dans Miro.

![Miro_embed_in_Jira.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016120699410_Miro%20embed%20in%20Jira.jpg)
*Superposition du tableau dans Jira*

 Vous pouvez également cliquer sur le bouton source pour ouvrir le tableau dans Miro dans un nouvel onglet.

![source_button.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134094738_source%20button.jpg)
*Le bouton pour accéder à l’application Miro*

### Détacher les tableaux

Pour détacher un tableau, cliquez simplement sur l’icône en forme de croix et l’association est instantanément retirée (le tableau n’est pas modifié dans Miro).

![remove_an_attached_board.jpg](https://help.miro.com/hc/article_attachments/21016134131986)
*L’option de retirer le tableau attaché*

## Comment désactiver le module complémentaire

Pour désactiver l’intégration, ouvrez **Atlassian Marketplace** > **Manage apps** (Gérer les applications), puis ouvrez la page du module complémentaire et cliquez sur **Uninstall** (Désinstaller) :

![uninstall_Jira_add-on.jpg](../../../../../../docs/integrations-apps/atlassian/images/21016134096274_uninstall%20Jira%20add-on.jpg)
*L’option de **désinstallation** dans la section des modules complémentaires de Jira*

## Smart link d’Atlassian pour Miro

Vous pouvez intégrer des tableaux Miro dans des tickets Jira à l’aide de la fonctionnalité de lien intelligent d’Atlassian. Cette fonctionnalité vous permet d’intégrer un tableau sans avoir à installer un plugin.

:::note
Veuillez noter que seuls les utilisateurs ayant accès au tableau intégré du côté de Miro seront en mesure de travailler sur l’aperçu après avoir connecté leurs comptes Miro et Atlassian. Si vous souhaitez rendre l’aperçu disponible pour tous les utilisateurs de Jira, veuillez utiliser le module complémentaire Jira.
:::

Accédez à un ticket Jira et collez simplement un lien vers le tableau ou tapez /link pour l’insérer. Si vous utilisez la fonction pour la première fois, il vous sera demandé de connecter votre équipe Miro. Cliquez sur **Connect to preview,**autorisez dans Miro, et choisissez une équipe dans laquelle vous intègrerez vos tableaux.

![install_Atllassian_links.jpg](https://help.miro.com/hc/article_attachments/21016134134418)
*Choix d’une équipe pour l’intégration des tableaux*

Lorsque vous collez le lien d’un tableau Miro dans un ticket Jira, il se transforme automatiquement en widget Jira. Cliquez sur le lien pour afficher les options permettant d’afficher le lien sous forme de carte ou d’intégration.

![display_as_link.gif](https://help.miro.com/hc/article_attachments/21016134135570)
*Les options permettant d’afficher un tableau Miro sous la forme d’un lien, d’une carte ou d’un élément incorporé.*

Si vous choisissez d’afficher le tableau sous forme d’intégration, vous pouvez modifier ses dimensions en faisant glisser ses côtés.

![changer_la_taille_des_embed_dans_Jira.gif](https://help.miro.com/hc/article_attachments/21016134118418)
*Modifier la taille de l’intégration de Miro dans Jira*

:::warning
Si les cookies tiers sont bloqués dans votre navigateur, des problèmes pourraient survenir lors de l’affichage des tableaux intégrés.
:::

## Foire aux questions

Puis-je masquer la section des tableaux Miro dans les tickets Jira ?

Oui, cliquez sur les trois points dans le coin supérieur droit de la section et choisissez **Masquer les tableaux Miro**.
![hide_Miro_boards.jpg](https://help.miro.com/hc/article_attachments/21016134136722)
*Masquer les tableaux Miro dans Jira*

Le module complémentaire fonctionne-t-il dans les projets Jira Next-gen ?

Oui, vous pouvez joindre vos tableaux à ces projets.

Le module complémentaire Jira coûte-t-il plus cher ?

Miro pour Jira Cloud est disponible pour tous les forfaits payants sans frais supplémentaires (forfaits Starter, Business et Enterprise).

Nous allons migrer Jira d’une instance de cloud à une autre. Les tableaux Miro intégrés dans des tickets Jira seront-ils affectés ?

Il ne devrait pas y avoir de problème avec les tableaux Miro intégrés si le contenu est déplacé sans modification.
