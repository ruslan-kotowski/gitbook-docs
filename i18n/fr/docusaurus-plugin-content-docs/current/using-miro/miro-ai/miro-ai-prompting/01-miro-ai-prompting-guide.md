---
title: Guide de prompt Miro IA
article_id: 30226743358226
translation_id: 30226743358226
locale: fr
sidebar_position: 1
created_at: '2025-10-14T17:24:22Z'
updated_at: '2025-11-25T15:54:58Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

De meilleurs prompts produisent de meilleurs résultats lorsqu'on travaille avec n'importe quel modèle d'IA. Des prompts plus détaillés permettent généralement de créer des sorties qui correspondent plus étroitement à ce que vous avez en tête. Les prompts plus courts et moins détaillés donnent au modèle d'IA plus de liberté pour interpréter ce que vous souhaitez, ce qui peut produire des résultats surprenants.

Ce guide de prompt vous assistera dans la création de meilleurs prompts lorsque vous travaillez avec les fonctionnalités de Miro IA.

## Cadre RISEN

Le cadre RISEN pour les prompts d'IA est une approche structurée pour générer de meilleurs résultats dès le départ. Il comprend :

- **Rôle :** L'IA est-elle un créateur, un conseiller ou un résolveur de problèmes ? Elle joue un rôle particulier dans votre équipe ? *Exemples : « Vous êtes un concepteur de produits senior créant… » ou « Vous êtes un rédacteur technique expert conseillant… »*
- **Entrée :** C'est là que vous fournissez les informations dont l'IA aura besoin pour accomplir sa tâche. Dans Miro, cela peut inclure des informations écrites ou du contexte à partir du tableau. Par exemple, lors de la création d'un prototype, vous pourriez inclure les fonctionnalités du produit ou quelles pages devraient être incluses.
- **Étapes :** C'est ici que vous indiquez à l'IA ce que vous voulez qu'elle fasse. Bien que vous puissiez donner des instructions générales ici, détailler précisément ce que vous attendez aura de meilleurs résultats. *Exemple : « 1. Résumer le contenu fourni dans le contexte du tableau. 2. Créer un pense-bête pour chaque point important du contenu. 3. Organiser les pense-bêtes en fonction de leur probable impact. »*
- **Attentes :** Si vous ne précisez pas ce que vous attendez en sortie, l'IA prendra cette décision pour vous et ne réussira pas toujours. Soyez précis ici ; au lieu de dire « créer un diaporama », dites-lui de « créer un diaporama de douze diapositives » et indiquez-lui ensuite quels sujets chaque diapositive doit aborder.
- **Restriction :** Si vous souhaitez que certains éléments *ne* soient pas inclus dans le résultat, précisez-le à la fin. Par exemple, vous pourriez créer un prototype IA pour un processus de paiement en ligne qui *n’*inclut pas une page de connexion dans le flux.

En définissant chacun de ces paramètres, l'IA de Miro saura exactement quel résultat vous attendez, produisant ainsi des sorties globalement meilleures.

## Ajouter du contexte depuis votre tableau Miro

Une des fonctionnalités les plus puissantes de [Miro IA](../01-miro-ai-overview.md) est la capacité d'ajouter du contexte depuis le tableau en cours. Cela vous permet d'ajouter un grand volume d'informations de manière structurée pour améliorer le résultat de votre IA.

Voici quelques conseils pour tirer le meilleur parti du contexte du tableau :

- **Ne sélectionnez pas tout sur le tableau.** Bien qu'il puisse être tentant de tout sélectionner comme contexte, réduire la sélection aux informations les plus pertinentes donnera de meilleurs résultats.
- **Ajoutez un contexte spécifique à l'industrie sur le tableau.** Bien que Miro IA soit puissant, il est également basé sur un modèle de langage général (LLM) comme la plupart des autres modèles d'IA. Ajouter de la documentation spécifique à l'industrie pertinente à votre prompt l'aide à produire de meilleurs résultats dès la première utilisation. Cela peut inclure des éléments tels qu'un glossaire de termes de l'industrie, un exemple de résultat spécifique que vous souhaitez qu'il génère, ou d'autres connaissances sectorielles que quelqu'un extérieur à votre industrie ne connaîtrait probablement pas.
- **Utilisez Miro IA pour créer un contexte.** Si vous avez besoin de quelque chose comme une fiche de conception produit basée sur des notes de réunion, vous pouvez utiliser Miro IA pour créer cela dans un document Miro sur votre tableau. Apportez les modifications nécessaires, puis incluez cela comme contexte plutôt qu'en incluant des notes de réunion éparses qui peuvent être confuses.

## Prompts de démarrage Miro IA

Vous débutez sur Miro IA ? Ne vous inquiétez pas. Nous avons créé des prompts prêts à l'emploi pour les workflows populaires. Remplacez simplement les espaces réservés entre crochets (par exemple, [rôle], [artéfact], [ton]) par votre contexte, puis exécutez le prompt. Explorez nos prompts de démarrage par workflow :

- [Prompts de démarrage pour la génération de contenu et l'idéation](02-content-generation-and-ideation-starter-prompts.md)
- [Prompts de démarrage pour l'analyse et l'organisation de contenu](03-content-analysis-and-organization-starter-prompts.md)
- [Prompts de démarrage pour l'optimisation des workflows](04-workflow-optimization-starter-prompts.md)

## Conseils de prompt spécifiques aux fonctionnalités

Miro IA propose des partenaires d’IA généraux et spécialisés, le mode IA, des flux et des outils d’IA spécifiques aux formats pour mieux cibler le résultat que vous souhaitez. Si vous essayez de créer un prototype, par exemple, ouvrez Miro Prototypes au lieu d'essayer de le créer depuis le partenaire d'IA à usage général.

### Miro Prototypes

[Miro Prototypes](../../miroverse/prototyping/07-miro-prototypes-add-on.md) vous permet de créer des flux de prototypes à écran unique ou multiple avec l'IA. Suivez ces conseils pour obtenir de meilleurs résultats de prototypage :

- Précisez les écrans que vous souhaitez inclure dans le prototype, surtout s'il y en a qui ne suivent pas un schéma d'UX typique pour le parcours utilisateur que vous concevez.
- Si vous avez des exigences de produit ou de design (c’est-à-dire des codes hexadécimaux pour des couleurs spécifiques), incluez-les comme contexte sur votre tableau.
- Incluez des captures d'écran de pages ou de designs similaires que vous souhaitez utiliser comme inspiration comme contexte sur votre tableau.
- Ajoutez des informations sur votre utilisateur cible dans le prompt (par exemple, « étudiants universitaires » ou « responsables d'équipe de design »).

### Diapositives Miro

Utilisez l'IA pour créer des [diapositives](../../formats/02-create-miro-slides-with-ai.md) et accélérer la préparation de vos présentations. Suivez ces conseils pour générer de meilleures présentations :

- Définissez la palette de couleurs ou d'autres aspects stylistiques dans votre prompt. Si vous avez spécifié une palette de couleurs dans le Centre de marque Miro, incluez-la dans votre prompt.
- Incluez le contenu des diapositives spécifiques sous forme de documents ou de pense-bêtes comme contexte sur le tableau.
- Précisez qui est votre audience dans le prompt (par exemple, « cadres dirigeants » ou « capital-risqueurs »).

### Images

Utilisez Miro IA pour créer des images sur vos tableaux. Voici quelques conseils pour créer de meilleures images :

- Spécifiez le style de l'image (c'est-à-dire "photorealiste", "peinture numérique", "impressionniste").
- Incluez le contexte pertinent du tableau, comme une description de ce que l'image doit inclure (vous pouvez également inclure cela dans le prompt, mais s'il existe déjà sur le tableau, incluez-le comme contexte à la place).
- Ajoutez tous les détails spécifiques que l'image doit inclure (c'est-à-dire "la personne porte un ordinateur portable" ou "une pile de livres est sur le bureau").
- Plus votre prompt est précis, meilleur sera votre résultat initial.

## Modification et itération avec Miro IA

Miro IA est un outil pour vous assister dans votre travail, et non un substitut aux insights et connaissances humaines. La modification et l'itération sont une étape importante pour créer de meilleurs résultats, tant en utilisant l'IA que manuellement.

En créant des formats avec Miro IA, vous aurez la possibilité de modifier avant d'ajouter le contenu à votre tableau. Dans les Miro Prototypes et les diapositives Miro, vous pouvez modifier un écran ou une diapositive à la fois, mais vous pouvez effectuer autant de tours de modification que nécessaire. Vous pouvez également revenir à des versions antérieures à tout moment avant d'ajouter le contenu au tableau.

Voici quelques conseils pour modifier avec Miro IA :

- Spécifiez une modification à la fois lors de l'ajustement des résultats. Donner trop d'instructions à la fois peut produire des résultats inattendus.
- Concentrez-vous sur le contenu plutôt que sur le style, car vous ne pouvez modifier qu'un écran ou une diapositive à la fois.
- Essayez différentes formulations ou mots-clés si le résultat n'est pas celui que vous attendiez.

Si vous avez créé un format sur lequel vous souhaitez itérer, mais que vous l'avez déjà ajouté au tableau, vous pouvez utiliser cet objet comme contexte pour la prochaine itération. C'est une bonne option si vous décidez de faire quelque chose d'aussi simple que de changer le style d'un diaporama ou si vous voulez ajouter des écrans supplémentaires dans un flux de prototype.

:::note
Même si utiliser un travail généré par l'IA comme contexte pour itérer de nouvelles versions est un bon point de départ, l'IA peut modifier des aspects du travail en fonction d'autres éléments de prompt ou de contexte supplémentaire. Assurez-vous de vérifier tous les résultats.
:::
