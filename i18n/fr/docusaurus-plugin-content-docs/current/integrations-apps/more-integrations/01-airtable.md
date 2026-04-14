---
title: Airtable
article_id: 360012807619
translation_id: 360012807619
locale: fr
sidebar_position: 1
created_at: '2020-03-24T12:09:00Z'
updated_at: '2025-08-05T07:33:41Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Personnes: Tous les utilisateurs de Miro, utilisateurs sur des forfaits
    payants Airtable Forfaits Miro: Tous les forfaits Plateformes: Navigateur'
---

Profitez de la puissance de la visualisation sur tableau blanc dans le cadre de votre travail tout en utilisant Airtable ! Vous pouvez exporter des données de Miro vers Airtable et intégrer des tableaux Miro dans les bases Airtable pour les consulter, les commenter et les modifier directement dans Airtable.

## Exporter des données à partir des tableaux Miro vers Airtable

L'intégration Airtable Sync vous permet d'exporter des données (par exemple, des pense-bêtes, des cartes) de vos tableaux Miro et de les organiser dans Airtable. Pour en savoir plus sur la configuration et l'utilisation de cette fonctionnalité, veuillez consulter [la documentation officielle d'Airtable](https://support.airtable.com/docs/airtable-sync-integration-miro).

## Intégrer des tableaux Miro dans les bases Airtable

### Installez l'application Miro dans Airtable

:::warning
L'application Miro pour Airtable n'est **pas** disponible dans le navigateur **Safari**.
:::

Les éditeurs de bases dans Airtable peuvent installer l'application Miro. Pour ce faire :

1. Ouvrez votre base Airtable et cliquez sur **Extensions** dans le coin supérieur droit.

   ![Airtable extensions button in the top right corner.](../../../../../../docs/integrations-apps/more-integrations/images/21017651877394_Airtable%20extensions.jpg)
   *Bouton des extensions dans le coin supérieur droit d'une base Airtable.*
2. Cliquez sur **Ajouter une extension**.

   ![Add an extension option in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647938834_add%20an%20extension.jpg)
   *L’option permettant d’ajouter une nouvelle extension.*
3. Recherchez "Miro" dans l'Airtable Marketplace et cliquez sur **Ajouter**.

   ![Miro app in Airtable Marketplace.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933714_Miro%20in%20Airtable.jpg)
   *Application Miro sur le Marketplace Airtable.*

### Ajouter des tableaux Miro existants aux bases Airtable

Une fois que l'application Miro est ajoutée à votre base Airtable, cliquez sur **Ajouter un tableau** dans la section de l'application Miro qui apparaît dans votre panneau d'extensions.

![Add a Miro board button in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651876498_add%20a%20Miro%20board.jpg)
*Ajout d'un tableau Miro via l'application Miro dans Airtable.*

Un sélecteur de tableau Miro apparaîtra. Si vous n'êtes pas déjà connecté à Miro dans votre navigateur, vous serez invité à vous connecter ou à créer un compte Miro.

Après avoir sélectionné un tableau, configurez les autorisations de partage pour son apparence dans Airtable à l'aide du menu déroulant. Trois options s'offrent à vous :

- **Toute personne peut consulter :** Toute personne dans Airtable peut [consulter](../../using-miro/sharing-boards/01-board-access-rights.md) le contenu du tableau intégré.
- **Toute personne peut commenter :** Toute personne dans Airtable peut [laisser des commentaires](../../using-miro/sharing-boards/01-board-access-rights.md) sur le tableau intégré. (Remarque : Cette option n'est pas disponible pour les tableaux stockés dans Miro [forfaits Free](../../plans-billing/miro-plans/09-free-plan.md).)
- **Privé :** Le tableau respectera ses paramètres de partage existants tels que configurés du côté de Miro.

  > ✏️ Pour les utilisateurs du [forfait Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) Miro, vos paramètres d’accès suivront les contrôles d’accès à l’échelle de l’organisation, ce qui peut impliquer que certaines options de partage peuvent être restreintes. En savoir plus : [Gestion de la politique de partage Enterprise pour les intégrations intégrées](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md).

![Sharing settings options when adding a Miro board to Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651879826_board%20access%20in%20Airtable.jpg)
*Paramètres de partage lors de l’ajout d’un tableau Miro dans Airtable.*

Le tableau Miro intégré apparaîtra alors dans votre base Airtable, où vous pourrez le consulter, le commenter ou le modifier selon les autorisations définies.

![Embedded Miro board within an Airtable base.](../../../../../../docs/integrations-apps/more-integrations/images/21017651872402_Miro%20board%20in%20Airtable.jpg)
*Un tableau Miro intégré dans Airtable.*

Pour remplacer un tableau intégré par un autre, cliquez sur l'icône d'engrenage (**Paramètres**) pour l'application Miro dans Airtable, sélectionnez **Choisir un tableau**, et choisissez un autre tableau à partir du sélecteur Miro.

![Replacing an embedded Miro board in Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017647932690_replacing%20a%20board.jpg)
*Remplacement d’un tableau Miro intégré dans Airtable.*

### Créer de nouveaux tableaux Miro à partir d'Airtable

Pour créer un nouveau tableau Miro directement depuis Airtable :

1. Dans la section de l'application Miro au sein d'Airtable, cliquez sur **Ajouter un tableau** (ou **Choisir un tableau** si un tableau est déjà intégré et que vous le remplacez).
2. Dans le sélecteur Miro, sélectionnez l'option pour créer un **Nouveau tableau**.

![Creating a new Miro board from the picker within Airtable.](../../../../../../docs/integrations-apps/more-integrations/images/21017651880466_add%20a%20new%20board%20to%20Airtable.jpg)
*Création d'un nouveau tableau Miro depuis le sélecteur dans Airtable.*

Le nouveau tableau sera créé dans votre compte Miro et intégré dans votre base Airtable.

### Supprimer des tableaux Miro d’Airtable

Pour retirer un tableau Miro intégré de votre base Airtable, vous devez supprimer ou reconfigurer l'extension de l'application Miro au sein de cette base. Cliquez sur le menu déroulant de l'application Miro dans le panneau des extensions et choisissez de supprimer ou de gérer l'extension.

![Deleting the Miro app from Airtable extensions panel.](../../../../../../docs/integrations-apps/more-integrations/images/21017647933074_deleting%20the%20app.jpg)
*Suppression de l’application Miro du panneau d’extensions Airtable.*
