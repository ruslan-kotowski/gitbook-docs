---
title: "Fonctionnalit\xE9s de Confiance pour l'IA et FAQ"
article_id: 30943405198994
translation_id: 30943405198994
locale: fr
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:32:10Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: ai-granular-admin-settings
---

Lors de Canvas 25, nous avons annoncé l’espace de travail IA pour l’innovation avec des workflows IA visuels et des agents collaboratifs IA sur le canevas. En plus des fonctionnalités destinées aux utilisateurs, nous introduisons de nouvelles capacités d'administration pour vous offrir plus de visibilité, des contrôles plus intelligents et des moyens harmonieux de débloquer les nouveaux outils IA de Miro pour vos équipes.

Utilisez cette page pour explorer les fonctionnalités de confiance IA disponibles avec le module complémentaire Enterprise Guard. Chaque section commence par un court aperçu, suivi d'une FAQ extensible couvrant différents aspects de chaque fonctionnalité.

- Contrôles d'administration granulaires de Miro IA : définir l'accès au niveau des fonctionnalités (Tout le monde/Personne/Équipes spécifiques) dans chaque catégorie de fonctionnalités.
- [Bloquer l'utilisation de Miro IA avec les Garde-fous Intelligents](#h_block_ai_with_guardrails) : utilisez les Garde-fous Intelligents pour bloquer toutes les interactions alimentées par l'IA dans Miro lorsque vous devez protéger des données sensibles ou classifiées.
- [Tableau de bord de l'Aperçu des Analyses d'Administration](#h_admin_analytics_overview) : suivre les tableaux, utilisateurs, équipes, licences et modèles avec des tendances historiques et une actualisation quotidienne.
- Modération de l'IA (également disponible sur le niveau Enterprise) : définissez des niveaux de filtrage pour l'ensemble de l'organisation (Strict, Par défaut, Minimal) pour filtrer les prompts qui pourraient conduire à des résultats nuisibles ou inappropriés.
- Blocage des prompts : bloquez les prompts contenant des données sensibles ou du code source au moment de la soumission ; affichez un message de politique à la place de l'envoi à un LLM.
- Enterprise Guard et intégration Microsoft Purview DSPM pour l'IA : transférez les prompts et les réponses à Purview pour une centralisation de la surveillance, des audits et de la gouvernance.

## Contrôles d'admin granulaires de Miro IA pour le module complémentaire Enterprise Guard

Les contrôles administrateurs de Miro IA permettent aux admins d’entreprise de décider quelles fonctionnalités IA sont disponibles dans leur organisation et de gérer qui peut les utiliser. Les admins peuvent également consulter les modèles qui alimentent chaque fonctionnalité IA. Avec le module complémentaire Enterprise Guard, les contrôles de Miro IA s'étendent au niveau des fonctionnalités au sein de chaque catégorie de fonctionnalités, ce qui aide à prioriser les fonctionnalités en fonction des besoins organisationnels et des exigences de sécurité. En plus de la catégorie complète de fonctionnalités Miro IA, les admins peuvent également activer, restreindre ou supprimer des fonctionnalités IA Miro spécifiques. Par exemple, dans la catégorie Images, vous pouvez activer Créer des images avec l'IA et désactiver Supprimer l'arrière-plan. Utilisez ces contrôles pour déployer l'IA en toute sécurité et répondre aux exigences de sécurité tout en favorisant l'adoption des fonctionnalités IA. Pour plus d'informations, consultez la [documentation sur les contrôles administrateurs granulaire de Miro IA](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Objectif et portée**

**Qu'est-ce que le contrôle granulaire pour Miro IA ?**

Avec le module complémentaire Enterprise Guard, les admins d’entreprise peuvent activer, restreindre ou supprimer l’accès aux fonctionnalités d’IA individuelles comprises dans chaque catégorie. Cela vous permet de choisir exactement quelles fonctionnalités les équipes peuvent utiliser.

**Pourquoi utiliser des contrôles granulaires ?**

Pour équilibrer l'adoption et la sécurité. Par exemple, dans Images, vous pouvez autoriser Créer des images tout en désactivant Supprimer l'arrière-plan.

**Accès et prérequis**

**Qui peut configurer les contrôles granulaires et sur quels forfaits ?**

Les admins d'entreprise bénéficiant du module complémentaire Enterprise Guard, via le navigateur.

**Où puis-je gérer l'accès au niveau des fonctionnalités ?**

Console admin → Miro IA → Fonctionnalités. Développez une fonctionnalité pour voir et définir l'accès à ses fonctionnalités individuelles.

**Contrôles et comportement**

**Contrôles précis : quelle est la différence entre un contrôle au niveau des fonctionnalités et un contrôle au niveau de la fonctionnalité, et que se passe-t-il lorsque je les active ou désactive ?**

- **Niveau des fonctionnalités :** Tout le monde, Personne ou Équipes spécifiques s'applique à toute la catégorie. Si vous désactivez une fonctionnalité, les utilisateurs perdent l’accès à cette fonctionnalité et à toutes ses fonctionnalités sur les tableaux. Si vous désactivez toutes les fonctionnalités, Créer avec l’IA apparaît désactivé sur le tableau.
- **Niveau de la fonctionnalité :** Avec Enterprise Guard, vous pouvez définir Tout le monde, Personne ou Équipes spécifiques pour chaque fonctionnalité individuelle. Désactiver une fonctionnalité supprime l’accès uniquement à cette fonctionnalité ; les autres fonctionnalités de la même fonctionnalité restent disponibles si elles sont activées.

**Quelles options d'accès existent au niveau fonctionnel ?**

Pour chaque fonctionnalité, choisissez Tous, Aucun, ou Équipes spécifiques. L'option Tous active la fonctionnalité au niveau de l'organisation et remplace les restrictions au niveau de l'équipe. L'option Aucun supprime l'accès à tous les utilisateurs. L'option Équipes spécifiques cible uniquement les équipes sélectionnées.

**Que se passe-t-il lorsque je désactive une fonctionnalité individuelle ?**

Les utilisateurs ne peuvent pas accéder à cette fonctionnalité sur aucun tableau, mais les autres fonctionnalités de la même catégorie restent disponibles si elles sont activées.

**Référence et exemples**

**Quelles fonctionnalités puis-je contrôler individuellement ?**

Consultez la référence dans le produit pour voir la liste actuelle. Les exemples sous Créer du contenu incluent Créer des pense-bêtes, Regrouper des pense-bêtes, Créer et modifier des documents, tables, diagrammes, et opérations de texte comme réécrire, raccourcir, tonifier et traduire. Les images incluent Créer des images, Supprimer l'arrière-plan et Ajouter des légendes. Résumer l'activité inclut Récapitulatif et Synthèse de conversation. Les flux, les partenaires d’IA et les prototypes apparaissent s’ils sont activés pour votre organisation.

**Puis-je voir quels modèles alimentent des fonctionnalités spécifiques ?**

Oui. Les admins peuvent consulter les modèles associés à chaque fonctionnalité IA dans la zone de référence pour faciliter la révision et la gouvernance.

## Bloquer l'utilisation de Miro IA avec des Garde-fous Intelligents

Utilisez les Garde-fous Intelligents pour bloquer toutes les interactions alimentées par l'IA dans Miro lorsque vous devez protéger des données sensibles ou classifiées. Lorsque ce garde-fou est appliqué, tous les outils Miro IA sont désactivés sur les tableaux concernés, tandis que la collaboration sans IA reste disponible. Pour en savoir plus et configurer cette fonctionnalité, consultez l'aperçu des Garde-fous Intelligents et la section Définir les garde-fous.

**Objectif et portée**

**Qu'est-ce que l'option "Bloquer l'utilisation de Miro IA" ?**

Elle désactive toutes les fonctionnalités Miro IA (par exemple, génération de texte, génération/reconnaissance d'images, suggestions intelligentes) partout où cette garde-fou s'applique, empêchant ainsi toute interaction assistée par IA avec du contenu sensible ou classifié.

**Qu'est-ce qui reste disponible pour les utilisateurs ?**

Les utilisateurs peuvent continuer à collaborer normalement sans IA. Le contenu déjà généré par IA reste sur les tableaux et peut être consulté, déplacé ou modifié manuellement—mais les utilisateurs ne peuvent pas utiliser Miro IA pour le modifier ou le régénérer.

**Accès et prérequis**

**Qui peut configurer cette barrière de protection et où ?**

Les admins de contenu sensible configurent les barrières de protection dans *Enterprise Guard* sous Classification des données → Barrières de protection. (Les admins d'entreprise attribuent le rôle d'admin de contenu sensible.)

**Que faut-il avant d'attribuer cette barrière de protection ?**

Définissez vos niveaux de classification et, éventuellement, l'auto-classification pour que la barrière de protection puisse être appliquée selon la classification (par exemple, INTERNE, CONFIDENTIEL).

**Comportement et impact**

**Qui est affecté lorsque la barrière s'applique ?**

Tous les utilisateurs, y compris les propriétaires et copropriétaires de tableaux, ne peuvent pas accéder à Miro IA ni l’invoquer sur les tableaux concernés.

**Supprime-t-elle le contenu IA existant ?**

Non. Elle empêche de nouvelles interactions avec l’IA ; le contenu IA existant reste disponible pour consultation et modifications manuelles.

**Quand les modifications prennent-elles effet ?**

Une fois vos mises à jour de la barrière publiées, l’application est immédiate sur les tableaux concernés.

**Configuration et paramétrage**

**Comment activer "Bloquer l'utilisation de Miro IA" pour une classification ?**

1. Allez à *Enterprise Guard* → Classification des données → **Garde-fous**.
2. Cliquez sur l'icône **Modifier** pour un niveau de classification (par exemple, CONFIDENTIEL).
3. Cochez la case **Bloquer l'utilisation de Miro IA** et cliquez sur **Terminé**.
4. Cliquez sur **Suivant** et examinez l'impact, puis cliquez sur **Publier** pour appliquer.

**Devrais-je utiliser le mode par défaut ou strict ?**

En mode par défaut, les garde-fous n'outrepassent pas les paramètres de partage existants. En mode strict, les garde-fous prennent le pas sur le partage actif et appliquent les contrôles les plus stricts. Choisissez selon vos besoins en gestion du changement.

**Expérience utilisateur**

**Que verront les utilisateurs sur les tableaux où l'IA est bloquée ?**

Les points d'entrée de l'IA de Miro apparaissent désactivés ou indisponibles, et les utilisateurs ne peuvent pas invoquer les outils d'IA depuis le canevas ou les menus sur ces tableaux.

**Les utilisateurs peuvent-ils demander des exceptions sur un seul tableau ?**

Non. Le garde-fou est appliqué par la politique de classification. Modifiez la classification du tableau (ou la politique pour ce niveau) pour changer l'application.

**Interactions avec d'autres contrôles**

**Comment cela se rapporte-t-il aux contrôles d'admin granulaires de Miro IA ?**

Les contrôles granulaires déterminent qui peut utiliser des fonctionnalités IA spécifiques. Le garde-fou est une couche de politique : lorsqu'il est actif, il bloque l'IA indépendamment des basculements de fonctionnalités.

**En quoi cela diffère-t-il du blocage de prompt ou de la modération de l'IA ?**

- **Blocage de prompt** arrête les prompts sensibles lors de la soumission ; l'IA reste disponible pour les prompts non sensibles.
- **Modération de l'IA** filtre le contenu nuisible ou inapproprié.
- **Bloquer l'utilisation de Miro IA** désactive totalement l'IA sur les tableaux affectés.

**Résolution des problèmes**

**L'IA apparaît encore sur certains tableaux. Que vérifier ?**

- Confirmez que la classification du tableau est celle où le garde-fou est activé et que vous avez cliqué sur **Publier** après avoir modifié les garde-fous.
- Si vous utilisez la classification automatique, vérifiez que la classification des tableaux a été mise à jour en fonction du contenu actuel.
- En mode Strict par rapport au mode par défaut, assurez-vous que votre attente correspond au mode de déploiement sélectionné.

**Nous devons réactiver l'IA pour un sous-ensemble de travaux.**

Ajustez le garde-fou pour la classification concernée ou reclassifiez les tableaux qui devraient permettre l'IA, puis publiez la mise à jour.

## Tableau de bord d'aperçu des analyses administratives

**Portée et mesures**

**Que couvre le tableau de bord d'aperçu ?**

Tableaux, Utilisateurs, Équipes, Licences et Modèles, avec des tendances historiques lorsque cela est applicable.

**Comment est défini « Actif pendant cette période » pour les Tableaux, Utilisateurs et Équipes ?**

- **Tableaux :** Tableaux uniques ouverts depuis le début de la période sélectionnée. Inclut les tableaux ensuite déplacés dans la corbeille.
- **Utilisateurs :** Utilisateurs uniques ayant ouvert un tableau au moins une fois depuis le début de la période. Inclut les utilisateurs désormais désactivés.
- **Équipes :** Équipes uniques avec au moins un membre ayant ouvert un tableau depuis le début de la période. Peut inclure des équipes ensuite déplacées dans la corbeille.

**Les totaux excluent-ils les éléments dans la corbeille ?**

Oui. Les totaux pour les tableaux et les équipes excluent les éléments actuellement dans la corbeille. Les comptes "actifs" historiques peuvent inclure des éléments qui ont été ensuite mis à la corbeille.

**Que montre le graphique des licences ?**

Totaux et historique pour les licences complètes, Free et licences gratuites restreintes, reflétant le nombre de licences actuellement utilisées.

**Que montrent les modèles aujourd'hui ?**

Les modèles les plus populaires utilisés dans un tableau. D'autres sources pourront être ajoutées dans les prochaines versions.

**Comportement temporel et historique**

**Comment les valeurs historiques s'affichent-elles sur les graphiques de synthèse ?**

Les widgets historiques montrent les valeurs au dernier jour de chaque période. Jusqu'à un an d'historique est disponible, ou remontant aussi loin que les données existent.

**Actualité des données et contrôles**

**À quelle fréquence les données de l’aperçu sont-elles actualisées et où puis-je le voir ?**

Au moins une fois toutes les 24 heures. Un horodatage « Dernière mise à jour » est disponible dans le tableau de bord.

**Comment puis-je changer la plage temporelle ?**

Utilisez le sélecteur de plage temporelle en haut à droite de la page Analytics.

## Modération Miro IA

Avec Miro IA, les admins d’entreprise peuvent ajuster les niveaux de filtres des prompts susceptibles de contenir du texte potentiellement nuisible ou inapproprié. Vous pouvez définir une sensibilité de modération Miro IA à l'échelle de l'organisation pour filtrer le contenu, y compris la haine, le contenu sexuel, la violence et l'automutilation. Cela vous aide à aligner l'utilisation de Miro IA avec les exigences, les politiques et la tolérance au risque de votre organisation. Pour plus d'informations, voir la [documentation sur la modération de Miro IA](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**But et portée**

**Qu'est-ce que la modération IA dans Miro ?**

La modération IA permet aux admins d’entreprise de définir un niveau de filtrage à l'échelle de l'organisation (Strict, Défaut ou Minimal) qui examine les prompts pouvant entraîner du contenu préjudiciable ou inapproprié (par exemple, haine, contenu sexuel, violence, automutilation).

**Qui peut le configurer et sur quels forfaits ?**

Les admins d’entreprise sur Enterprise avec Enterprise Guard peuvent configurer le paramètre dans les paramètres de l'organisation.

**Est-ce que cela fonctionne si mon organisation connecte son propre LLM (par exemple, une intégration directe avec un fournisseur) ?**

Si un LLM personnalisé est connecté, le sélecteur de modération peut être désactivé pour cette intégration et tout niveau précédemment choisi ne s’appliquera pas.

**Accès et prérequis**

**Qui peut l'activer et de quoi ai-je besoin ?**

Les admins d’entreprise sur Enterprise avec le module complémentaire Enterprise Guard peuvent configurer la modération IA dans les paramètres de l’organisation.

**Comment l'activer ?**

Accédez à Paramètres → Miro IA → Modération, choisissez Strict/Défaut/Minimal, puis cliquez sur **Enregistrer les modifications**. L'application est immédiate dans toute l'organisation.

**Niveaux et comportement**

**Que signifient les niveaux ?**

- **Strict :** Bloque le contenu par défaut + contenu à risque faible à modéré (par exemple, haine subtile/codée, contenu sexuel suggestif, violence non graphique, mentions non explicites d’automutilation).
- **Par défaut (recommandé) :** Bloque le contenu modérément à gravement nuisible.
- **Minimal :** Bloque uniquement le contenu gravement nuisible.

**Quand les changements prennent-ils effet ?**

Immédiatement pour l’ensemble de l’organisation.

**Les changements sont-ils suivis ?**

Oui. Les mises à jour sont enregistrées dans le journal d’audit de votre organisation.

**Configuration et Paramétrage**

**Où puis-je définir ou mettre à jour le niveau de modération ?**

Allez dans Paramètres → Miro IA → Modération, choisissez Strict/Par défaut/Minimal, puis cliquez sur **Enregistrer les modifications**.

**Quel niveau de départ recommandez-vous ?**

Le niveau par défaut convient à la plupart des organisations ; ajustez-le en fonction des retours pilotes et de la tolérance au risque.

**Interactions avec d'autres contrôles**

**Comment l'IA de modération se rapporte-t-elle aux garde-fous et aux contrôles de prompt ?**

- **Garde-fous intelligents :** Si un tableau est couvert par le garde-fou « Bloquer l'utilisation de Miro IA », l'IA est désactivée quel que soit le niveau de modération.
- **Blocage de prompt :** Fonctionne en complément de la modération. Le blocage de prompt arrête les prompts sensibles lors de la soumission ; la modération filtre les catégories nuisibles.
- **Contrôles d'admin granulaires :** Les bascules de fonctionnalités déterminent qui peut accéder aux fonctionnalités de l'IA lorsque celle-ci est disponible.

**Résolution des problèmes et meilleures pratiques**

**Nous constatons trop de faux positifs.**

Envisagez de passer de Strict à Par défaut (ou de Par défaut à Minimal) et publiez des exemples d'utilisation acceptable. Si les problèmes persistent après l'ajustement des paramètres, contactez votre Customer Success Manager de Miro pour signaler cela afin que notre équipe produit puisse examiner la situation.

**Nous constatons que du contenu nuisible passe à travers.**

Passez à Par défaut ou Strict et fournissez des directives internes. Révisez après les mises à jour des politiques/réglementations. Si les problèmes persistent après ces changements, contactez votre Customer Success Manager de Miro pour signaler cela afin que notre équipe produit puisse examiner la situation.

## Blocage des prompts

Le blocage des prompt permet aux admins de contenu sensible d'empêcher les utilisateurs de soumettre des prompt IA incluant des informations sensibles, vous aidant ainsi à empêcher que des données sensibles ne soient présentes dans Miro IA à travers votre organisation. Miro analyse le texte qu'un utilisateur saisit dans le champ de prompt, ainsi que tout contenu textuel qu'il ajoute depuis le tableau. Si ce contenu correspond aux badges de sensibilité ou aux motifs de code source sélectionnés dans la configuration du blocage de prompt, Miro bloque la soumission du prompt.  Pour plus d'informations, consultez la [documentation sur le blocage des prompt](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Objectif et portée**

**Qu'est-ce que le Blockage de Prompts ?**

Le Blockage de Prompts empêche les utilisateurs de soumettre des prompts IA qui incluent des informations sensibles. Miro analyse le texte qu’un utilisateur saisit dans le champ de prompt et tout contenu textuel qu'il ajoute depuis le tableau ; si cela correspond aux badges de sensibilité ou aux modèles de code source sélectionnés, la soumission est bloquée et un message de politique est affiché. Pour le moment, nous ne supportons que le contenu basé sur du texte.

**En quoi le Blockage de Prompts est-il différent de la vérification de tableau ?**

La vérification de tableau détecte le contenu sensible sur les tableaux et peut classifier les tableaux automatiquement ; le Blockage de Prompts vérifie ce que les utilisateurs tentent d'envoyer à Miro IA au moment de la soumission.

**Quels badges de sensibilité sont pris en charge ?**

Utilisez les catégories au niveau de l'organisation répertoriées dans la référence des badges et des infotypes de sensibilité.

**Qu'est-ce que l'Analyse du Code ?**

L'Analyse du Code bloque les prompts contenant du code source reconnaissable ; par conception, elle nécessite un minimum de code (par exemple, 5 lignes ou plus) pour se déclencher. Activez/désactivez-la dans la configuration du blocage de prompt.

**Le contenu non textuel (par exemple, les images) est-il analysé ?**

Non. Pour le moment, le blocage de prompt ne prend en charge que le contenu textuel.

**Accès et prérequis**

**Qui peut l’activer et que me faut-il ?**

Les admins de contenu sensible liés à Enterprise avec le module complémentaire Enterprise Guard peuvent l'activer dans Paramètres → Enterprise Guard → Découverte de données → Configuration.

**Comment l’activer ?**

Ouvrez le blocage de prompt → Activer, choisissez Sélectionner tout ou des catégories de badges spécifiques, activez facultativement l'analyse du code, puis Activer. L'application est immédiate au niveau de l'organisation.

**Gestion et modifications**

**Comment ajuster les badges ou l'analyse du code par la suite ?**

Allez dans Paramètres → Enterprise Guard → Découverte de données → Configuration → Blocage des prompts → Gérer,

- **Badges :** Cochez la case *Sélectionner tout* pour sélectionner toutes les catégories ou sélectionnez des cases de catégorie de badge spécifiques.
- **Analyse du code :** Activez l'analyse du code pour bloquer les prompts qui incluent du code source (minimum 5 lignes). Pour plus d'informations, consultez Analyse du code.

Les modifications prennent effet immédiatement.

**Que se passe-t-il pour les prompts après avoir modifié les paramètres ?**

Les éléments nouvellement débloqués passeront. Les éléments qui correspondent encore aux motifs bloqués restent stoppés.

**Expérience utilisateur**

**Que voit un utilisateur lorsqu'un prompt est bloqué ?**

Un message de politique apparaît à l'endroit où il a entré le prompt, et la demande n'est pas envoyée à un LLM.

**Le contenu non textuel (par exemple, les images) est-il analysé ?**

Non. Pour le moment, le blocage de prompt prend uniquement en charge le contenu textuel.

**Interactions avec d'autres contrôles**

**Comment fonctionne le blocage de prompts avec les garde-fous et la modération ?**

- **Garde-fous intelligents :** Si "Désactiver l'utilisation de Miro IA" s'applique, l'IA est désactivée ; le blocage de prompts ne se déclenche pas car les prompts ne peuvent pas être soumis.
- **Modération de l'IA :** Les deux peuvent s'appliquer lorsque l'IA est disponible : le blocage de prompts arrête les données sensibles ; la modération filtre les catégories nuisibles.
- **Contrôles d'admin granulaires :** L'accès aux fonctionnalités s'applique seulement lorsque l'IA est disponible et que le prompt n'est pas bloqué.

##

## Intégration de l'Enterprise Guard et de Microsoft Purview DSPM pour l'IA

Pour les organisations utilisant Microsoft Entra ID (anciennement Azure AD) comme fournisseur d’identité, Enterprise Guard transfère de manière sécurisée les prompts et les réponses de l'IA vers la gestion de la posture de sécurité des données (DSPM) de Microsoft Purview pour l'IA. Les équipes de sécurité et de conformité peuvent alors surveiller, auditer et contrôler l'utilisation de l'IA générative depuis une plateforme unique et fiable, réduisant ainsi les frais opérationnels, atténuant les risques tels que les fuites de données et les utilisations abusives, et renforçant la gouvernance de l'IA de niveau entreprise de Miro. Pour plus d'informations, consultez la [documentation sur l'intégration de l'Enterprise Guard et de Microsoft Purview DSPM pour l'IA](../integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Objet et portée**

**Qu'est-ce que l'intégration de Microsoft Purview DSPM pour IA dans Miro ?**

Une intégration qui transfère les prompts et les réponses de Miro IA vers le DSPM pour IA de Microsoft Purview, permettant ainsi aux équipes de sécurité et de conformité de surveiller, auditer et gérer l'activité IA en un seul endroit.

**Qui peut utiliser cette intégration ?**

Les forfaits Enterprise comprenant l'Enterprise Guard, gérés par les admins d’entreprise ayant accès aux intégrations Enterprise. Votre organisation Miro doit utiliser Microsoft Entra ID pour l'authentification unique. Une licence Microsoft Purview est requise.

**Quels sont les avantages ?**

Visibilité centralisée de l'utilisation de Miro IA dans le hub IA de Purview, traçabilité des prompts et des réponses, et alignement avec vos politiques de gouvernance existantes dans Purview.

**Quelles activités Miro IA sont incluses aujourd'hui ?**

Pour l'instant, les prompts et réponses textuels dans toutes les fonctionnalités de Miro IA sont transmis. Le contenu image n'est pas transmis.

**Toutes les activités des utilisateurs sont-elles enregistrées?**

Seules les activités des utilisateurs qui se connectent à Miro via le tenant Microsoft Entra configuré sont transmises à Purview.

**Quel est le délai avant que l'activité apparaisse dans Purview?**

Généralement, 10 à 30 minutes après l'action IA dans Miro. Consultez-la dans Microsoft Purview → DSPM pour IA → Explorateur d'activité, ou vérifiez les journaux d'audit.

**Y a-t-il des limitations notables?**

Pour l'instant, un seul tenant Entra peut être configuré à la fois. Dans les environnements multi-fournisseurs d'identité ou multi-tenants, seuls les utilisateurs authentifiés via le tenant configuré sont enregistrés. Les images ne sont pas incluses.

**Configuration et paramétrage**

**Comment activer l’intégration ?**

Dans Miro : Paramètres Enterprise → Intégrations Enterprise → activez Microsoft Purview DSPM pour IA → saisissez votre ID de locataire Entra → Connecter → connectez-vous avec un compte capable d'accorder un consentement administrateur à l’échelle du locataire → acceptez l'application de gouvernance Miro IA → confirmez Connecté dans Miro.

**Quels sont les prérequis ?**

- **Miro :** Forfait Enterprise avec Enterprise Guard, rôle d’admin d’entreprise, ID Entra configuré pour l’authentification unique. Pour activer cette fonctionnalité, contactez votre responsable Customer Success.
- **Microsoft :** Licence Microsoft Purview, l’ID de locataire Entra utilisé pour SSO Miro, et un rôle Entra capable d'accorder un consentement administrateur à l’échelle du locataire.

**Comment vérifier que la configuration fonctionne ?**

Effectuez une action simple avec Miro IA, attendez 10 à 30 minutes, puis consultez Microsoft Purview → DSPM pour IA → Explorateur d'activités pour de nouvelles entrées Miro.

**Comment déconnecter ou changer de locataire ?**

Dans Miro : Intégrations d'enterprise → Microsoft Purview pour IA → Déconnecter. Pour changer de locataire, déconnectez d'abord, puis reconnectez avec le nouvel ID de locataire.

**Utilisation et gouvernance**

**Où puis-je voir les données transférées dans Purview ?**

Microsoft Purview → DSPM pour IA → Explorateur d'activités. Vous pouvez également consulter les détails dans les journaux d'audit.

**Puis-je exporter ou archiver les journaux d'activités IA ?**

Utilisez les outils d'exportation de Microsoft Purview. Miro transfère l'activité vers votre tenant Microsoft où vos politiques s'appliquent.

**Puis-je appliquer des politiques Purview aux données de Miro IA ?**

Oui. Une fois intégrées, les données suivent le modèle de gouvernance Purview de votre organisation.

**Qu'en est-il des responsabilités en matière de confidentialité et de sécurité ?**

Miro transfère les prompts et les réponses vers votre tenant Microsoft. La gouvernance et les contrôles d'accès sont gérés dans Purview au sein de votre environnement.

**Résolution des problèmes et service d’assistance**

**L'étape de consentement échoue ou boucle. Que dois-je vérifier ?**

Assurez-vous que le compte utilisé pour Connect peut accorder des autorisations administratives globales dans Entra, ou faites appel à un admin global de Microsoft.

**Je ne vois aucune activité dans Purview. Que faire ?**

Vérifiez qu'Enterprise Guard est activé et que vous avez accès aux intégrations Enterprise. Assurez-vous que l'identifiant de locataire correspond exactement à votre locataire SSO Miro. Vérifiez qu'un test d'action IA a été effectué par un utilisateur s'authentifiant via ce locataire. Vérifiez les licences et filtres Purview. Accordez jusqu'à 30 minutes pour l'ingestion.

**Nous utilisons plusieurs IdP ou locataires. Tous les utilisateurs seront-ils enregistrés ?**

Non. Seule l'activité des utilisateurs se connectant via le locataire Entra configuré est transférée.

**Qui supporte quoi ?**

Contactez le service d’assistance Miro pour la configuration ou la connectivité dans Miro. Pour les problèmes à l'intérieur de Microsoft Purview, contactez le service d’assistance Microsoft.
