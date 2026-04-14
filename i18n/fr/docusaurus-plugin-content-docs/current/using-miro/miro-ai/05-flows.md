---
title: Flux
article_id: 29687970855442
translation_id: 29687970855442
locale: fr
sidebar_position: 5
created_at: '2025-09-23T12:18:02Z'
updated_at: '2026-03-16T12:37:03Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: template-picker
availability:
  notes: 'Qui peut le faire: Membres de l''équipe Quels forfaits: Free, Starter, Business,
    Enterprise, Education Quelles plateformes: Navigateur, Bureau, Mobile'
---

Les flux vous permettent d'enchaîner des formats sur le canevas pour créer des workflows alimentés par l'IA. Chaque format sert d'entrée pour le suivant, transformant des processus complexes et multi-étapes, comme la planification de sprint, la rédaction de briefs, ou l'utilisation des données clients, en flux automatisés.

Pour savoir quels formats prennent en charge les flux, voir Formats supportés.

Cet article explique comment utiliser les flux. Pour des informations générales sur les flux, voir [Aperçu des flux](04-flows-overview.md).

:::tip
Obtenez des modèles de flux prêts à l'emploi dans le [sélecteur de modèles](../../getting-started/start-here/your-first-board/04-templates.md).
:::

## Créer et exécuter un flux

La procédure suivante utilise des éléments de base de l'UX des flux pour créer un flux à partir de zéro. Pour vous assurer de pouvoir commencer à créer des flux plus rapidement, voir Éléments UX des flux.

Suivez ces étapes :

1. Ajoutez un format pris en charge ou un bloc instruction IA au canevas.
2. (Facultatif) Connectez tout format existant ou bloc d'instruction au format que vous venez d'ajouter. Utilisez les connecteurs en losange IA pour connecter votre flux.
3. Au-dessus du Format, cliquez sur la barre **TASK**.
   Une barre **TASK** se développe en une boîte où vous pouvez spécifier votre prompt pour cette position dans votre flux.
4. Dans la boîte **TASK**, ajoutez votre prompt. Par exemple, dans un document, vous pouvez générer un Document de spécifications produit (DSP). Vous pouvez utiliser la sortie de tout Format ou bloc d'instruction IA connecté.

   > 💡 La boîte **TASK** vous permet de sélectionner un modèle de langage large (LLM), un fournisseur de connaissances ou une recherche web. En bas à gauche, sélectionnez un modèle d'IA, une base de connaissances ou effectuez une recherche sur le web. Les options varient en fonction du Format.
5. (Facultatif) Pour créer une nouvelle sortie, à droite, cliquez sur le connecteur IA en forme de losange.
   Le menu **Créer une nouvelle sortie** s'ouvre.
6. (Facultatif) Pour créer une nouvelle entrée, cliquez à gauche sur le connecteur en losange de Miro IA.
   Le menu **Créer une nouvelle entrée** s'ouvre.
7. Pour compléter votre flux, répétez les étapes 1-6 selon les besoins.
8. Pour exécuter votre flux, dans la barre **TÂCHE**, cliquez sur **Exécuter**.
   ![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)*Le menu contextuel **Flux sélectionné** vous indique combien d'étapes le flux comprend.*

## Utiliser la connaissance avec les flux

La connaissance s'intègre avec des fournisseurs comme Glean, la recherche sur le web, et Miro Insights, pour récupérer tout ce que votre entreprise sait, à partir de sources internes et externes.

Pour tout format dans votre flux, cliquez sur la barre **TASK**. La barre **TASK** s'agrandit. En bas à gauche, sélectionnez et connectez votre base de connaissances.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Spécifiez une base de connaissances interne pour votre flux*

Vous pouvez convertir les données de vos propres ressources de connaissances en formats comme les documents, les tables, les pense-bêtes et les diapositives. Ensuite, connectez chaque format pour utiliser vos données comme entrée ou sortie d’un flux.

**Plus d'informations :** Voir [Connaissances](09-knowledge.md).

## Annuler le résultat d'un flux

Vous pouvez annuler le résultat pour tout format dans votre flux. Par exemple, vous exécutez un flux par accident et écrasez un document.

Pour rétablir un Format dans votre flux à un état antérieur, cliquez sur la barre **TASK**. La barre **TASK** s'agrandit. En bas à droite, cliquez sur l'icône dans le sens inverse des aiguilles d'une montre. Sélectionnez n'importe quelle version des dernières 24 heures pour la restaurer.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *La fonctionnalité de rétablissement vous permet de restaurer n'importe quelle version de votre Format des dernières 24 heures.*

## Éléments d’UX des flux

Comprendre les éléments d’UX suivants des flux vous aidera à commencer à créer des flux plus rapidement.

### Connecteur Miro IA

Les formats pris en charge et les blocs d'instructions possèdent un connecteur en losange Miro IA à gauche pour connecter les entrées, et à droite pour les sorties.

Cliquez sur le connecteur Miro IA de chaque côté pour ouvrir les menus **Créer une nouvelle entrée** ou **Créer une nouvelle sortie**.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png)

*Cliquez sur le connecteur Miro IA pour ouvrir les menus des entrées et des sorties.*

:::tip
Vous pouvez également faire glisser le connecteur Miro IA vers du contenu existant.
:::

### Mise en évidence intelligente des connecteurs

Cliquez sur n'importe quel objet de votre flux pour voir uniquement ces connexions mises en évidence.

### Masquer les connecteurs de flux

Pour des flux complexes avec de nombreuses connexions, vous pouvez masquer tous les connecteurs de flux pour simplifier votre vue.

Dans la barre de votre [tableau](../working-on-the-board/02-miro's-new-simplified-user-interface.md), cliquez sur les trois points verticaux. Ensuite, sélectionnez **Consulter**. Basculez **Afficher/Masquer les connecteurs de flux** sur la position arrêt. Pour afficher tous les connecteurs de flux, basculez sur la position marche.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Afficher ou masquer tous les connecteurs de flux sur votre tableau.*

:::note
**Afficher/Masquer les connecteurs de flux** impacte uniquement votre vue de tableau. Les collaborateurs peuvent ajuster leur propre bascule.
:::

### Invit de format

Vous pouvez utiliser un prompt sur n’importe quel format ou bloc d’instructions dans votre flux, ce qui garantit que chaque format de la chaîne peut effectuer une tâche spécialisée du flux.

Cliquez sur la barre **TASK** au-dessus d’un format dans votre flux. La barre **TASK** s'agrandit. Ajoutez votre prompt et décrivez comment vous souhaitez que le format lise le contenu d'entrée, ou tout contenu sur le tableau, et précisez les règles et la sortie pour le prochain format dans votre flux.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *La boîte de prompt sur-format apparaît dans la barre **TASK** au-dessus de chaque format dans votre flux.*

### Bloc d’instructions pour l’IA

Vous pouvez sélectionner un modèle de langage étendu (LLM) ou un [fournisseur de connaissances](09-knowledge.md) disponible pour exécuter un prompt dans un bloc autonome, n'importe où dans votre flux.

Pour un Format donné, cliquez sur le connecteur Miro IA en forme de losange. Dans le menu d'entrée ou de sortie, sélectionnez **Instruction** **IA**.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Les blocs d'instructions vous permettent de chaîner des instructions, d'accepter des entrées et de transmettre des sorties au prochain Format.*

### Bouton de lancement global

Vous pouvez commencer votre exécution depuis n'importe quel format ou bloc d'instructions IA dans votre flux. Cliquez pour sélectionner le format ou le bloc. Le menu contextuel **Flux sélectionné** apparaît à côté de la barre de collaboration.

![](../../../../../../docs/using-miro/miro-ai/images/33531917801618_image.png) *Le menu contextuel Flux sélectionné*

Le menu **Flux sélectionné** affiche combien d'étapes restent à exécuter. Pour exécuter le flux, cliquez sur **Exécuter**.

## Formats pris en charge

Les flux prennent en charge les formats Miro suivants.

- Diagrammes
- Documents
- Images
- Intégrer du code iFrame
- Kanban
- Prototypes
- Diapositives
- Tables
- Planning
