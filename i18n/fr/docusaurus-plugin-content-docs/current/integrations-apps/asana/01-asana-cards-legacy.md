---
title: Cartes Asana (Legacy)
article_id: 360039492573
translation_id: 360039492573
locale: fr
sidebar_position: 1
created_at: '2019-11-25T10:03:42Z'
updated_at: '2025-11-25T16:05:44Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: asana-cards
---

:::warning
Cette page décrit notre ancienne intégration Asana. Pour la nouvelle intégration, consultez la [documentation Asana (bêta)](asana).
:::

**Fonctionnalités clés**

- Importez les tâches Asana dans les tableaux Miro pour visualiser les progrès de votre équipe
- Trouvez des tâches spécifiques à importer à partir de Miro en utilisant les filtres Asana ou en cherchant le nom de la tâche
- Synchronisation automatique : toutes les modifications apportées aux tâches Asana sont automatiquement affichées sur les cartes Asana sur Miro

> **Disponible pour** : Starter, Business, Enterprise forfaits. *Les administrateurs peuvent avoir besoin d'autoriser l'utilisation d'Asana pour leur équipe Miro. Les membres de l’équipe peuvent utiliser l’application Asana Cards uniquement si elle est installée au niveau de l’équipe.*

### Comment installer des cartes Asana

1. Premièrement, vous aurez besoin d’un compte Miro actif et d’un compte Asana actif. Si vous n’avez pas de profil Miro, inscrivez-vous [ici](https://miro.com/signup/).
2. Dans le Marketplace de Miro, ouvrez [Asana Cards](https://miro.com/marketplace/asana-cards/?backUrl=%2Fmarketplace%2F)*.* Cliquez sur le bouton **Obtenir l'application**.
   Vous devrez alors sélectionner l'équipe dans laquelle vous souhaitez installer Asana. Sélectionnez une équipe et cliquez sur **Installer et autoriser**.
   > ⚠️ Les utilisateurs qui ne sont pas dotés d’un rôle d’admin ne peuvent pas installer l’application s’ils ne sont pas autorisés à le faire dans les paramètres.

![install_Asana_cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020254087442_install%20Asana%20cards.jpg)
*Autorisation des cartes Asana*

3. L'étape suivante consiste à cliquer sur **Connecter** dans les paramètres de l'application Asana Cards.

![connect_Asana_and_Miro.jpg](../../../../../../docs/integrations-apps/asana/images/21020265147410_connect%20Asana%20and%20Miro.jpg)
*Paramètres de l’application Asana Cards dans les paramètres de l’équipe*
Les autres membres de l’équipe trouveront l’icône Asana Cards dans la barre d’outils de création du tableau et pourront y connecter leur compte Asana.

![Asana_cards_on_the_toolbar.jpg](../../../../../../docs/integrations-apps/asana/images/21020254085010_Asana%20cards%20on%20the%20toolbar.jpg)
*Les cartes Asana dans la barre d’outils*

4. Autorisez Asana Connect à accéder à votre compte Asana. Si vous n’êtes pas connecté à l’application pour le moment, vous devrez vous autoriser dans Asana.

**![grant_permission_to_Asana.jpg](../../../../../../docs/integrations-apps/asana/images/21020254090386_grant%20permission%20to%20Asana.jpg)*****Autoriser Miro à accéder à votre compte Asana***

### Comment importer et utiliser des cartes Asana

1. Une fois que vous avez connecté Miro à votre compte Asana, n’hésitez pas à ajouter des cartes Asana à vos tableaux Miro. Pour obtenir le sélecteur, dans la barre de création, sélectionnez **Outils, Médias et Intégrations** (**+**)**.**Un panneau s'ouvre. Recherchez et sélectionnez Cartes Asana.
2. Le sélecteur vous permettra de filtrer les tâches. Tout d’abord, veuillez choisir un espace de travail, puis filtrez les cartes par Projets, Étiquettes ou Destinataires. La liste des projets est triée par date de création.

   > ⚠️ Le sélecteur affichera uniquement les tâches auxquelles vous avez accès dans Asana. Si un utilisateur Miro ouvre la page source d’une tâche à laquelle il n’a pas accès, un message lui indiquera que cette tâche lui est inaccessible.

   ![Asana_picker.gif](../../../../../../docs/integrations-apps/asana/images/21020254098578_Asana%20picker.gif)
   **Importation de cartes Asana sur un tableau**

Cliquez sur le bouton **source** pour ouvrir la carte dans Asana.
![go_to_source.jpg](../../../../../../docs/integrations-apps/asana/images/21020265150226_go%20to%20source.jpg)
**Le bouton source de la carte**

N'hésitez pas à ajouter vos cartes Asana à [Kanban](../../using-miro/advanced-tools/02-columns-formerly-kanban.md) et à [User story map](../../using-miro/advanced-tools/07-user-story-mapping.md) simplement en les glissant.

:::warning
Bien qu'il n’y ait pas encore d’option pour créer ou modifier des cartes Asana du côté de Miro, toutes les modifications apportées du côté d’Asana sont synchronisées dans Miro (veuillez noter qu’il peut y avoir un léger retard dans la mise à jour de la carte).
:::

![Asana_cards_and_kanban.gif](../../../../../../docs/integrations-apps/asana/images/21020254093074_Asana%20cards%20and%20kanban.gif)
*Ajout des cartes Asana à un tableau Kanban*

### Modifier la couleur d’une carte

Pour modifier la couleur d’une carte, cliquez sur la ou les cartes et choisissez **Couleur de remplissage** dans le menu contextuel. Si vous dupliquez la carte, la nouvelle couleur sera appliquée. ![asana_card_color.png](../../../../../../docs/integrations-apps/asana/images/21020254100242_asana_card_color.png)
*Modifier la couleur de remplissage d’une carte*

### Comment désinstaller l’application Asana Cards

Pour désinstaller l’application Asana Cards au niveau de l’équipe, ouvrez Paramètres de l’équipe **> Applications & Intégrations > Asana Cards**, faites défiler la page vers le bas, et cliquez sur **Désinstaller pour l'équipe.**

**Si vous souhaitez désinstaller l’application au niveau individuel, veuillez cliquer sur** **Désinstaller pour moi.**

![uninstall_Asna_Cards.jpg](../../../../../../docs/integrations-apps/asana/images/21020265153426_uninstall%20Asna%20Cards.jpg)
*Désinstallation de l’application Asana Cards*

### Foire aux questions

1. *Quelles adresses IP doivent être autorisées pour les cartes Asana ?*
   *-*18.203.61.162, 54.220.74.201, 54.216.81.236, 54.73.153.141, 52.215.228.26, 52.16.47.17, 54.217.180.21.
