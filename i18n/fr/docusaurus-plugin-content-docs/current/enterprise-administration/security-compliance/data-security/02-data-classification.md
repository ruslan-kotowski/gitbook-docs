---
title: "Classification des donn\xE9es"
article_id: 4417739162258
translation_id: 4417739162258
locale: fr
sidebar_position: 2
created_at: '2022-02-07T10:01:21Z'
updated_at: '2025-02-26T12:17:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

La classification des données permet aux utilisateurs des forfaits Enterprise d’ajouter des badges à leurs tableaux pour spécifier leur degré de confidentialité.

> **Disponible pour** : Forfait Enterprise
> **Disponible sur** : version de bureau, tablette
> **Qui peut le faire ?** les admins d’entreprise

Vous trouverez les paramètres de classification des données dans la console d'administration Enterprise. Allez dans **Paramètres** et sélectionnez **Classification**.

:::note
Pour les clients disposant d'Enterprise Guard, vous trouverez la **classification** dans la console d'administration sous **Enterprise Guard**. Allez dans **Paramètres** > Enterprise Guard > Classification.
:::

Assurez-vous de bien comprendre les points clés suivants concernant la classification des données :

- La classification des données est un label interne et n'a aucun impact sur les paramètres de partage des tableaux, ce qui signifie que les tableaux peuvent être partagés au-delà de leur classification.
- Les tableaux créés avant l’activation de la fonctionnalité seront marqués comme non classés.
- [Dupliquer un tableau](../../../using-miro/managing-boards/03-how-to-duplicate-a-board.md) copiera le badge de classification des données actuel sur la nouvelle copie du tableau.
- Les badges ne sont actuellement pas affichés en [mode présentation](https://help.miro.com/hc/articles/360017731073), en [mode Smart meetings](https://help.miro.com/hc/articles/4408834812690) ni sur mobile.

## Comment mettre en place des étiquettes de classification ?

Dans **Paramètres**, sélectionnez **Classification**. Pour activer les étiquettes de classification pour votre organisation Enterprise, sélectionnez **Configurer la classification.**

## Comment ajouter de nouvelles étiquettes de classification ?

Les administrateurs d'entreprise peuvent créer et personnaliser jusqu'à 30 étiquettes de classification et définir une étiquette par défaut pour tous les nouveaux tableaux de l'entreprise.

Dans les paramètres de **classification**, quatre étiquettes sont déjà créées, que vous pouvez personnaliser. Vous pouvez également créer de nouvelles étiquettes pour répondre à vos besoins d'organisation.

Pour créer une nouvelle classification :

1. Sélectionnez **Modifier les niveaux de classification**.
2. Cliquez sur **Ajouter un niveau**.
3. **Définissez le **niveau** de classification, ajoutez un **nom**, ajoutez une **description** et modifiez la couleur du badge.**
4. **Si vous souhaitez ajouter une référence pour les utilisateurs du tableau, ajoutez un lien vers des directives.**
5. (Facultatif) Sélectionnez **Aperçu** pour voir comment votre étiquette apparaîtra en production.
6. Sélectionnez **Terminé**.
7. (Facultatif) Pour réorganiser vos étiquettes de classification, cliquez sur les flèches vers le haut**(Ʌ)** ou vers le bas**(V**).
8. **Cliquez sur Publier pour finaliser les modifications.**

:::note
Lorsque vous créez ou modifiez une étiquette de classification, vos modifications sont enregistrées en tant que projet et ne sont pas publiées tant que vous n'avez pas cliqué sur le bouton **Publier**. Cela signifie que vous pouvez quitter la configuration de la classification et y revenir à tout moment.
:::

Vous pouvez également ajouter un lien vers les lignes directrices de votre organisation en matière de classification qui permettront à vos collaborateurs d’en apprendre davantage sur vos politiques de classification des données existantes.

![](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921802487570_image.png)

*Lien vers les lignes directrices en matière de classification*

## Comment personnaliser les projets de classification

Pour modifier une classification **sans qu'** un brouillon ait été enregistré :

1. Cliquez sur le bouton **Modifier les niveaux de classification** .
2. Cliquez sur l'icône du crayon d'**édition.**
3. Effectuez vos modifications et cliquez sur **Terminé**.
4. **Cliquez sur Publier pour finaliser les modifications.**

Pour modifier une classification **dont le** brouillon a été enregistré :

1. Dans le panneau Classification des données, cliquez sur **Reprendre la configuration**.
2. Cliquez sur l'icône du crayon d'**édition.**
3. Effectuez vos modifications et cliquez sur **Terminé**.
4. **Cliquez sur Publier pour finaliser les modifications.**

## Comment supprimer une étiquette de classification ?

Pour supprimer une étiquette, cliquez sur l'icône de la corbeille. Notez que vous ne pouvez pas supprimer le badge par défaut.

![data_classification_delete_label.pngSupprimer](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017013528978_data_classification_delete_label.png)
*une étiquette*

### Ajouter le badge par défaut au niveau de l’entreprise

Choisissez une étiquette de classification par défaut pour les tableaux nouvellement créés. Chaque nouveau tableau créé dans l'organisation Enterprise se voit attribuer l'étiquette par défaut.

Pour définir une étiquette par défaut pour votre organisation, cochez **Étiquette de classification par défaut** lorsque vous ajoutez ou modifiez une étiquette de classification.

![Configuration de l'étiquette par défaut de la classification des données](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/23921802487570_image.png)

Configuration du badge de classification par défaut

### Ajouter le badge par défaut au niveau de l’équipe

> **Installation par :** Administrateurs d'entreprise, Administrateurs d'équipe

Les admins d’équipe et d’entreprise peuvent activer l’option **Remplacer le badge par défaut** et définir un badge par défaut au niveau de l’équipe : chaque nouveau tableau créé dans l’équipe en question se verra assigner ce nouveau badge par défaut qui viendra remplacer le badge par défaut configuré au niveau de l’entreprise.

Pour activer ce paramètre, rendez-vous dans les Paramètres de l’équipe > **Autorisations** et défilez vers le bas de la page.

Notez que vous pouvez définir cette fonctionnalité au niveau de l’équipe seulement si le paramètre de classification des données est activé au niveau de l’entreprise.

Pour les [équipes nouvellement créées,](../../managing-enterprise-teams-and-content/09-create-a-new-team-on-enterprise-plan.md) ce paramètre est désactivé si vous choisissez les paramètres par défaut lors de la création d’une équipe.

### Ajouter des badges de classification aux tableaux

> **Configuré par :** les [propriétaires du tableau](../../../using-miro/sharing-boards/01-board-access-rights.md), les [copropriétaires de tableau](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md), les éditeurs membres de l’équipe, les admins d’entreprise dotés des [autorisations d’admin de contenu](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md)

Si la classification des données est activée dans vos paramètres d’entreprise, les utilisateurs peuvent voir et modifier les badges des tableaux. Le badge de classification des données apparaît comme un badge en regard du nom du tableau. Lorsqu’ils survolent ce badge, les collaborateurs voient une infobulle contenant le nom du badge et sa description.

[Le propriétaire du tableau, les](../../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) [copropriétaires du tableau](../../managing-enterprise-teams-and-content/12-content-admin-permissions.md), les éditeurs membres de l’équipe et les admins d’entreprise dotés des autorisations d’admins de contenu peuvent mettre à jour le badge de classification soit en cliquant dessus, soit à partir des détails du tableau. Sélectionnez un badge et cliquez sur Mettre à jour. Si l’admin d’entreprise a ajouté un lien vers des lignes directrices dans les paramètres, l’utilisateur peut suivre ce lien dans la fenêtre contextuelle pour obtenir plus de détails.

![data_classification_adding_labels_to_boards.gifChangement de](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017043043090_data_classification_adding_labels_to_boards.gif)
*l'étiquette de classification des données sur le tableau*

### Filtre de classification des données sur le tableau de bord

Les utilisateurs des forfaits Enterprise dans lesquels la classification des données est activée peuvent filtrer leurs tableaux par badges sur le tableau de bord. Le filtre **Toute classification** est sélectionné par défaut.

![data_classification_classification_filter.pngFiltre](../../../../../../../docs/enterprise-administration/security-compliance/data-security/images/21017043043986_data_classification_classification_filter.png)
*de classification sur le tableau de bord*
