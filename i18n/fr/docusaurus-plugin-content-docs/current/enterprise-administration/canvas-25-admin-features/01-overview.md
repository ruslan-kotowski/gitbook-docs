---
title: "Aper\xE7u"
article_id: 30969987585938
translation_id: 30969987585938
locale: fr
sidebar_position: 1
created_at: '2025-11-11T12:42:45Z'
updated_at: '2026-01-12T16:04:30Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Lors de Canvas 25, nous avons annoncé l'Espace de travail IA pour l'innovation avec des workflows visuels IA et des agents IA collaboratifs sur le canevas. En plus des fonctionnalités utilisateur, nous introduisons de nouvelles capacités d'administration pour vous offrir plus de visibilité, des contrôles plus intelligents et des moyens simples pour débloquer les outils IA les plus récents de Miro pour vos équipes.

Utilisez cette page pour explorer les capacités d'administration IA disponibles pour les administrateurs sur le niveau Enterprise. Chaque section commence par une brève vue d'ensemble, suivie de FAQ extensibles couvrant différents aspects de chaque capacité.

- [Contrôles admin de Miro IA :](01-overview.md) décidez quelles capacités IA sont disponibles dans votre organisation et gérez qui peut les utiliser.
- Modération IA : définissez les niveaux de filtrage à l'échelle de l'organisation (Strict, Par défaut, Minimal) pour filtrer les prompts susceptibles de conduire à des sorties nuisibles ou inappropriées.
- Analytique admin : utilisez les tableaux de bord intégrés (Vue d'ensemble et Miro IA) pour suivre l'adoption et comprendre l'activité au sein de l'organisation, l'allocation des licences, l'utilisation des modèles, et l'utilisation de Miro IA dans votre organisation.

:::note
Pendant la bêta des AI Workflows, les Conditions d’utilisation personnalisées pour l'IA et les contrôles admin granulaires de Miro IA étaient disponibles pour les clients des AI Workflows. Avec la mise à disposition générale des AI Workflows, ces capacités sont désormais uniquement disponibles dans le cadre de l'Enterprise Guard. Pour plus d'informations, consultez [Gestion avancée de l'IA avec Enterprise Guard](01-overview.md).
:::

## Contrôles admin de Miro IA

Les contrôles admin de Miro IA vous aident à décider quelles capacités IA sont disponibles dans votre organisation et à gérer qui peut les utiliser. Pour plus d'informations, consultez la [documentation des contrôles admin de Miro IA](../managing-enterprise-teams-and-content/01-miro-ai-admin-controls.md).

**Objectif et portée**

**Qu'est-ce que les contrôles d'admin de Miro IA?**

Les contrôles d'admin de Miro IA permettent aux admins de gérer l'accès aux capacités de Miro IA au sein de l'organisation. Selon votre configuration, vous pouvez activer l'accès pour tout le monde, restreindre l'accès à des équipes spécifiques ou désactiver l'accès.

**Quelle est la différence entre une capacité IA et une fonctionnalité IA?**

Une **capacité** est une catégorie de fonctionnalité IA (par exemple, créer du contenu, travailler avec des images ou résumer une activité). Une **fonctionnalité** est une action spécifique au sein d'une capacité (par exemple, *créer des pense-bêtes* ou *supprimer l'arrière-plan*).

Les contrôles au niveau des fonctionnalités (gestion des fonctionnalités individuelles à l'intérieur d'une capacité) sont disponibles avec [Enterprise Guard](01-overview.md).

**Accès et prérequis**

**Où puis-je gérer les contrôles d’admin de Miro IA ?**

Dans la console d’admin, allez à **Miro IA** > **Capacités**. De là, vous pouvez activer, restreindre ou supprimer l’accès à chaque capacité IA (et, si disponible, aux fonctionnalités IA individuelles).

**Qui peut configurer ces paramètres ?**

Les admins d'entreprise peuvent gérer l’accès à Miro IA dans la console d’admin (la disponibilité des fonctionnalités IA dépend de votre forfait et des modules complémentaires activés).

**Options d'accès et comportement**

**Que signifient les options d'accès (Tout le monde, Personne, Équipes spécifiques) ?**

Utilisez le menu déroulant à côté d'une capacité (ou d'une fonctionnalité, si disponible) pour choisir comment l'accès est accordé.

| Option | Ce qu'elle fait | Quand l'utiliser |
| --- | --- | --- |
| **Tout le monde** | Permet l'accès à tous les utilisateurs et équipes de votre organisation (y compris les équipes créées ultérieurement). Toute restriction au niveau de l'équipe est supprimée. | Déploiement standard dans toute l'organisation. |
| **Personne** | Supprime l'accès pour tout le monde. Il vous sera demandé de confirmer la suppression. | Restreindre l'utilisation à l'échelle de l'organisation. |
| **Équipes spécifiques** | Permet l'accès uniquement pour les équipes que vous sélectionnez. | Pilote avec un sous-ensemble d'équipes ou déploiement progressif. |

**Que se passe-t-il si je désactive une fonctionnalité ?**

Lorsqu'une fonctionnalité est désactivée, les utilisateurs ne peuvent plus accéder à cette fonctionnalité et à ses caractéristiques associées sur les tableaux. Si toutes les fonctionnalités de Miro IA sont désactivées, l'option **Créer avec l'IA** apparaît comme désactivée sur le tableau.

**Ces paramètres s'appliquent-ils aux équipes créées ultérieurement ?**

Si vous définissez une fonctionnalité (ou une caractéristique) pour **Tous**, cela s'applique à votre organisation, y compris aux équipes créées ultérieurement. Si vous choisissez **Équipes spécifiques**, vous devrez mettre à jour la sélection à mesure que de nouvelles équipes sont créées (si vous souhaitez les inclure).

**Enterprise Guard et contrôle au niveau des fonctionnalités**

**Comment Enterprise Guard modifie-t-il ce que je peux contrôler ?**

Avec [Enterprise Guard](01-overview.md), vous pouvez gérer l'accès au **niveau des fonctionnalités** à l'intérieur de chaque capacité (et non seulement au niveau de la catégorie). Cela vous permet d'autoriser certaines fonctionnalités tout en restreignant d'autres au sein d'une même capacité.

Par exemple : Vous pouvez autoriser la c*réation d'images* et restreindre la s*uppression de l'arrière-plan* (au sein de la capacité Images).

**Visibilité et disponibilité**

**Pourquoi ne puis-je pas voir les paramètres pour Flux, Partenaires d’IA ou Prototypage ?**

Certaines fonctionnalités (comme les **Flux**, les **Partenaires d’IA**, et le **Prototypage**) sont visibles et gérables uniquement si elles sont activées pour votre organisation.

**Puis-je voir quel modèle d’IA alimente une fonctionnalité ?**

Oui. Dans la console d’admin > **Miro IA** > **Fonctionnalités**, les admins peuvent consulter les modèles qui alimentent chaque fonctionnalité d’IA.

**Les invités ou visiteurs peuvent-ils utiliser Miro IA si je l’active ?**

Miro IA est disponible pour les **Membres**. Les invités et les visiteurs ne peuvent pas utiliser Miro IA.

**Dépannage et bonnes pratiques**

**J’ai changé les paramètres d’accès, mais les utilisateurs voient toujours Miro IA. Que devrais-je vérifier ?**

- **Confirmer la portée :** Assurez-vous d’avoir mis à jour la bonne capacité (ou la fonctionnalité spécifique, si des contrôles au niveau de la fonctionnalité s’appliquent).
- **Vérifier le ciblage d’équipe :** Si défini sur *Équipes spécifiques*, confirmez que l’équipe de l’utilisateur est sélectionnée.
- **Permettre le temps de propagation :** Dans certains cas, les modifications peuvent prendre un peu de temps pour être appliquées à travers les sessions.
- **Actualiser la session :** Demandez à l’utilisateur de rafraîchir l’onglet du navigateur, de se déconnecter/se reconnecter, ou de redémarrer l’application de bureau (si applicable).

## Modération Miro IA

Avec la modération Miro IA, les admins d’entreprise peuvent ajuster les niveaux de filtrage des prompts qui pourraient contenir des textes potentiellement nuisibles ou inappropriés. Vous pouvez définir une sensibilité de modération de Miro IA à l'échelle de l'organisation pour filtrer le contenu, y compris la haine, le contenu sexuel, la violence et l'automutilation. Cela vous aide à aligner l'utilisation de Miro IA avec les exigences, politiques et tolérances de risque de votre organisation. Pour plus d'informations, consultez la [documentation sur la modération Miro IA](../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**But et portée**

**Qu’est-ce que la modération IA dans Miro ?**

La modération IA permet aux admins d’entreprise de définir un niveau de filtrage à l’échelle de l’organisation (Strict, Défaut ou Minimal) qui examine les prompts pouvant entraîner du contenu préjudiciable ou inapproprié (par exemple, haine, contenu sexuel, violence, automutilation).

**Qui peut le configurer et sur quels forfaits ?**

Les admins d’entreprise sur le forfait Enterprise avec le module complémentaire AI Workflows peuvent configurer ce paramètre dans les paramètres de l'organisation.

**Cela fonctionne-t-il si mon entreprise connecte son propre LLM (par exemple, une intégration directe avec un fournisseur) ?**

Si un LLM personnalisé est connecté, le sélecteur de modération peut être désactivé pour cette intégration et tout niveau précédemment choisi ne s'appliquera pas à celle-ci.

**Accès et prérequis**

**Qui peut l'activer et de quoi ai-je besoin ?**

Les admins d’entreprise sur le forfait Enterprise avec le module complémentaire AI Workflows peuvent configurer la modération IA dans les paramètres de l'organisation.

**Comment l'activer ?**

Allez dans Paramètres → Miro IA → Modération, choisissez Strict/Default/Minimal, puis cliquez sur **Enregistrer les modifications**. L'application est immédiate à l'échelle de l'organisation.

**Niveaux et comportement**

**Que signifient les niveaux ?**

- **Strict :** Bloque le contenu par défaut + contenu à faible ou modéré risque (par exemple, haine subtile/codée, contenu sexuel suggestif, violence non graphique, mentions de l'automutilation non explicites).
- **Défaut (recommandé) :** Bloque le contenu modérément à sévèrement nuisible.
- **Minimal :** Bloque uniquement le contenu sévèrement nuisible.

**Quand les modifications prennent-elles effet ?**

Immédiatement pour l'ensemble de l'organisation.

**Les modifications sont-elles suivies ?**

Oui. Les mises à jour sont enregistrées dans le journal d'audit de votre organisation.

**Configuration et paramétrage**

**Où puis-je définir ou mettre à jour le niveau de modération ?**

Accédez à Paramètres → Miro IA → Modération, choisissez Strict/Par défaut/Minimal, puis cliquez sur **Enregistrer les modifications**.

**Quel niveau de départ recommandez-vous ?**

Le niveau Par défaut convient à la plupart des organisations ; ajustez-le en fonction des retours des pilotes et de la tolérance au risque.

**Interactions avec d'autres contrôles**

**Comment la modération IA est-elle liée aux garde-fous et aux contrôles de prompt ?**

- **Garde-fous intelligents :** Si un tableau est couvert par le garde-fou « Bloquer l'utilisation de Miro IA », l'IA est désactivée quel que soit le niveau de modération.
- **Blocage de prompt :** Fonctionne en parallèle avec la modération. Le blocage de prompt arrête les prompts sensibles lors de la soumission; la modération filtre les catégories nuisibles.
- **Contrôles administratifs granulaires :** Les commutateurs de fonctionnalités régissent qui peut accéder aux fonctionnalités IA lorsque l'IA est disponible.

**Dépannage et meilleures pratiques**

**Nous constatons trop de faux positifs.**

Envisagez de passer de Strict à Par défaut (ou de Par défaut à Minimal) et publiez des exemples d'utilisation acceptable. Si les problèmes persistent après avoir ajusté les paramètres, contactez votre Customer Success Manager Miro pour signaler cela afin que notre équipe produit puisse examiner.

**Nous voyons du contenu nuisible passer à travers.**

Passez à Par défaut ou Strict et fournissez des directives internes. Réévaluez après les mises à jour des politiques/régulations. Si les problèmes continuent après ces changements, contactez votre Customer Success Manager Miro pour le signaler afin que notre équipe produit puisse examiner.

## Analytique Admin

Les analyses Admin fournissent aux admins d’entreprise des insights exploitables et basés sur des données concernant l'adoption, l'utilisation et la gestion de Miro à grande échelle. Cela inclut deux tableaux de bord : **Vue d'ensemble** et **Miro IA**. Pour plus d'informations, consultez [Vue d'ensemble des analyses](../getting-started/admin-analytics/01-analytics-overview.md), [Tableau de bord Vue d'ensemble](../getting-started/admin-analytics/02-overview-dashboard.md) et [Tableau de bord Miro IA](../getting-started/admin-analytics/03-miro-ai-dashboard.md).

**Objectif et portée**

**Qu'est-ce qu'Admin Analytics ?**

Admin Analytics fournit des métriques fiables intégrées au produit pour vous aider à comprendre comment Miro est utilisé, à gérer votre organisation, à stimuler l'adoption et à répondre aux besoins de sécurité et de conformité.

**Quels tableaux de bord sont inclus ?**

Admin Analytics inclut deux tableaux de bord : **Aperçu** (activité et adoption au sein de l'organisation sur les tableaux, utilisateurs, équipes, licences et modèles) et **Miro IA** (adoption et utilisation de Miro AI dans l'ensemble de l'organisation).

**Tableaux de bord et navigation**

**Comment changer de tableau de bord ?**

Utilisez les onglets en haut de la page Analytics pour passer de l'**Aperçu** à **Miro IA**.

**Comment changer la plage de dates ?**

Utilisez le **sélécteur de période** en haut à droite de la page Analytics pour ajuster l'intervalle de temps affiché (**journalier**, **hebdomadaire**, **mensuel** ou **trimestriel**).

**Quand les données sont-elles actualisées ?**

Les indicateurs sont actualisés **quotidiennement**. Chaque tableau de bord affiche un horodatage **Dernière mise à jour**.

**Tableau de bord d'aperçu**

**Que puis-je suivre dans le tableau de bord d'aperçu ?**

Le tableau de bord d'aperçu vous aide à suivre l'adoption et à comprendre l'activité de l'organisation à l'aide de ces groupes de métriques :

- **Tableaux :** totaux de tableaux, tableaux actifs et tendances historiques.
- **Utilisateurs :** tendances des utilisateurs actifs. Vous pouvez également suivre par rôle, comme membres, admins d’entreprise, invités ou invités d’équipe.
- **Équipes :** nombres d’équipes et niveaux d’activité.
- **Licences :** types de licences attribuées et comment l’attribution évolue au fil du temps.
- **Modèles :** quels modèles sont les plus utilisés dans votre organisation.

**Comment devrais-je interpréter les graphiques historiques ?**

- Dans les widgets qui affichent des données historiques, les valeurs représentent les données du **dernier jour de chaque période**.
- La **période en cours** n'est pas affichée dans les graphiques historiques.
- Les données historiques sont disponibles jusqu'à **un an** ou aussi loin que les données existent.

**Tableau de bord Miro IA**

**Que puis-je suivre dans le tableau de bord Miro IA ?**

Le tableau de bord Miro IA vous aide à suivre l'adoption et à comprendre comment Miro IA est utilisé dans votre organisation grâce à ces indicateurs :

- **Équipes utilisant l'IA :** équipes utilisant activement les fonctionnalités d'IA, y compris le total des équipes utilisant ou non l'IA. Vous pouvez filtrer l'utilisation par cas d’utilisation.
- **Personnes utilisant l'IA :** totaux d'adoption pour les personnes utilisant ou non l'IA, avec un historique d'utilisation mensuel.
- **IA par cas d'utilisation :** utilisation au fil du temps répartie entre **création IA** et **automatisation IA**.
- **Collaborations avec les partenaires d’IA :** la fréquence à laquelle les équipes interagissent avec les partenaires d’IA via des sessions de chat (prompts, questions de suivi et réponses). Les analyses affichent le nombre de sessions démarrées.
- **Flux d’IA exécutés :** le nombre de fois que les utilisateurs ont lancé un flux d’IA comptant au moins deux étapes ou nœuds consécutifs. L'exécution est comptée à l'heure marquée du premier événement associé au flux.

**Comment les cas d’utilisation de l'IA sont-ils définis ?**

- **Création par IA :** actions telles que la création à partir de prompts et la création à partir d'un contexte visuel.
- **Automatisation par IA :** actions telles que l’itération via le chat ou le menu contextuel, la modification de texte, la catégorisation et la suppression des arrière-plans d’images.

**L'utilisation des crédits d'IA est-elle la même que les métriques d'utilisation de l'IA ?**

Non. **Les crédits d’IA ne sont pas directement corrélés** avec les métriques d'utilisation de l'IA affichées dans ce tableau de bord.

**Considérations sur les données**

**Pourquoi est-ce que je vois des données partielles ?**

Si une fonctionnalité a été désactivée pendant une partie de la période sélectionnée, vous pourriez voir des données partielles dans l'historique des mesures (par exemple, si une fonctionnalité a été activée au milieu du mois).

**Pourquoi les graphiques n'affichent-ils pas de données pour une certaine période ?**

Si aucune activité n'a été enregistrée pendant une période donnée (jour, semaine ou mois), le graphique n'affichera pas de données pour cette période.

**Les données plus anciennes semblent manquer. Que dois-je faire ?**

Les données historiques sont disponibles jusqu'à un an ou aussi loin que les données existent. Si les données plus anciennes semblent manquer, contactez le service d’assistance de Miro pour demander une vérification de remplissage rétroactif.

**Dépannage et bonnes pratiques**

**Nos chiffres sont inférieurs à nos attentes. Que dois-je vérifier ?**

- Vérifiez la **plage temporelle** et le type de période (quotidienne, hebdomadaire, mensuelle, trimestrielle).
- Gardez à l'esprit que les **graphiques historiques montrent les périodes complétées**, non pas la période en cours.
- Si une fonctionnalité a été activée en cours de période, attendez-vous à des **données partielles** pour cette période.

**Comment utiliser efficacement ces insights ?**

Utilisez les métriques de synthèse pour détecter les équipes, modèles ou tendances de licences sous-utilisés, puis lancez des initiatives d'activation ciblées. Utilisez les métriques de Miro IA pour identifier où l'adoption de l'IA progresse, soutenir les champions et guider le déploiement responsable.

## Gouvernance avancée de l'IA avec Enterprise Guard

Enterprise Guard offre des fonctionnalités avancées supplémentaires de gouvernance de l'IA pour les admins Enterprise. Utilisez ces contrôles pour affiner l'accès, protéger les informations sensibles et renforcer la surveillance et la conformité de l'utilisation de l'IA dans Miro. Pour plus d'informations, consultez [Fonctionnalités de confiance de l'IA d'Enterprise Guard et FAQs](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md).

- [Contrôles administratifs granulaire de Miro IA](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md) : définissez l'accès par fonctionnalité (Tout le monde/Personne/Équipes spécifiques) au sein de chaque catégorie de capacités.
- [Bloquez l'utilisation de Miro IA avec des Garde-fous Intelligents](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md) : utilisez des Garde-fous Intelligents pour bloquer toutes les interactions pilotées par l'IA dans Miro lorsque vous devez protéger des données sensibles ou classifiées.
- [Blocage de prompt](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md) : bloquez les prompts contenant des données sensibles ou du code source au moment de la soumission ; affichez un message de politique à la place d'envoyer à un LLM.
- [Enterprise Guard et Microsoft Purview DSPM pour intégration IA](../enterprise-subscription-management/enterprise-guard-overview/01-ai-trust-capabilities-and-faqs.md) : transmettez les prompts et réponses à Purview pour une surveillance centralisée, un audit et une gouvernance.
