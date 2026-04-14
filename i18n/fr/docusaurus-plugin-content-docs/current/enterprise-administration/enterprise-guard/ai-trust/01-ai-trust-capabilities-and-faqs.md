---
title: "Fonctionnalit\xE9s d\u2019IA et FAQ"
article_id: 30943405232914
translation_id: 30943405232914
locale: fr
sidebar_position: 0
created_at: '2025-11-10T14:17:30Z'
updated_at: '2026-03-11T21:34:47Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Lors de Canvas 25, nous avons annoncé l’espace de travail IA pour l'innovation avec des workflows IA visuels et des agents collaboratifs IA sur le canevas. En plus des fonctionnalités pour les utilisateurs finaux, nous introduisons de nouvelles fonctionnalités d’admin pour vous donner plus de visibilité, des contrôles plus intelligents, et des moyens fluides pour débloquer les outils IA les plus récents de Miro pour vos équipes.

Utilisez cette page pour explorer les fonctionnalités des Trust d’IA disponibles avec le module complémentaire Enterprise Guard. Chaque section commence par un bref aperçu, suivi d'une FAQ extensible couvrant différents aspects de chaque fonctionnalité.

- Contrôles administratifs granulaires de Miro IA : définir l'accès aux fonctionnalités au niveau de la fonctionnalité (Tout le monde/Personne/Équipes spécifiques) dans chaque catégorie de fonctionnalités.
- [Bloquer l'utilisation de Miro IA avec les Garde-fous intelligents](#h_block_ai_with_guardrails) : utilisez les Garde-fous intelligents pour bloquer toutes les interactions basées sur l'IA dans Miro lorsque vous devez protéger des données sensibles ou classifiées.
- [Tableau de bord Vue d'ensemble des analyses administratives](#h_admin_analytics_overview) : suivre les tableaux, utilisateurs, équipes, licences et modèles avec des tendances historiques et une actualisation quotidienne.
- Modération de l'IA (également disponible sur le niveau Enterprise) : définissez des niveaux de filtrage à l'échelle de l'organisation (Strict, Par défaut, Minimal) pour filtrer les prompts susceptibles de conduire à des résultats nuisibles ou inappropriés.
- Blocage des prompts : bloquez les prompts contenant des données sensibles ou du code source lors de la soumission ; affichez un message de politique à la place de l'envoi à un LLM.
- Enterprise Guard et Microsoft Purview DSPM pour intégration IA : transmettez les prompts et les réponses à Purview pour une surveillance, un audit et une gouvernance centralisés.

## Contrôles administratifs granulaire de Miro IA pour le module complémentaire Enterprise Guard

Les contrôles d'admin Miro IA permettent aux responsables d’entreprise de décider des fonctionnalités IA disponibles dans leur organisation et de gérer qui peut les utiliser. Les admins peuvent également consulter les modèles qui alimentent chaque fonctionnalité IA. Avec le module complémentaire Enterprise Guard, les contrôles Miro IA s'étendent au niveau des fonctionnalités dans chaque catégorie de fonctionnalités, ce qui aide à prioriser les fonctionnalités en fonction des besoins organisationnels et des exigences de sécurité. En plus de la catégorie complète des fonctionnalités Miro IA, les admins peuvent également activer, restreindre ou supprimer certaines fonctionnalités IA de Miro. Par exemple, dans la catégorie Images, vous pouvez activer "Créer des images avec IA" et désactiver "Retirer l'arrière-plan". Utilisez ces contrôles pour déployer l'IA en toute sécurité et répondre aux exigences de sécurité tout en favorisant l'adoption des fonctionnalités IA. Pour plus d'informations, consultez la [documentation sur les contrôles d'admin Miro IA granulaires](../../enterprise-guard/ai-trust/02-miro-ai-granular-admin-controls.md).

**Objectif et portée**

**Qu'est-ce que le contrôle granulaire pour Miro IA ?**

Avec le module complémentaire Enterprise Guard, les admins d’entreprise peuvent activer, restreindre ou supprimer l’accès aux fonctionnalités d’IA individuelles comprises dans chaque catégorie de fonctionnalités. Cela vous permet de choisir exactement quelles fonctionnalités les équipes peuvent utiliser.

**Pourquoi utiliser des contrôles granulaires ?**

Pour équilibrer l'adoption avec la sécurité. Par exemple, dans la catégorie Images, vous pouvez autoriser la création d'images tout en désactivant la suppression d'arrière-plan.

**Accès et prérequis**

**Qui peut configurer des contrôles granulaires et sur quels forfaits ?**

Les admins d'entreprise sur les forfaits Enterprise avec le module complémentaire Enterprise Guard, dans le navigateur.

**Où puis-je gérer l'accès aux fonctionnalités ?**

Console d'administration → Miro IA → Fonctionnalités. Développez une fonctionnalité pour voir et définir l'accès à ses fonctionnalités individuelles.

**Contrôles et comportement**

**Contrôles précis : quelle est la différence entre le contrôle au niveau de la fonctionnalité et celui au niveau de ses caractéristiques, et qu’arrive-t-il lorsque je les active ou désactive?**

- **Niveau de la fonctionnalité :** Tout le monde, Personne, ou Équipes spécifiques s’applique à toute la catégorie. Si vous désactivez une fonctionnalité, les utilisateurs perdent l’accès à cette fonctionnalité et à toutes ses caractéristiques sur les tableaux. Si vous désactivez toutes les fonctionnalités, Créer avec l’IA apparaît comme désactivé sur le tableau.
- **Niveau des caractéristiques :** Avec Enterprise Guard, vous pouvez définir Tout le monde, Personne, ou Équipes spécifiques pour chaque caractéristique individuelle. La désactivation d'une caractéristique supprime l'accès uniquement à celle-ci ; les autres caractéristiques de la même fonctionnalité restent disponibles si elles sont activées.

**Quelles options d’accès existent au niveau des fonctionnalités ?**

Pour chaque fonctionnalité, choisissez Tout le monde, Personne ou Équipes spécifiques. Tout le monde active la fonctionnalité à l’échelle de l’organisation et passe outre les restrictions au niveau de l’équipe. Personne supprime l’accès pour tous les utilisateurs. Équipes spécifiques cible uniquement les équipes sélectionnées.

**Que se passe-t-il lorsque je désactive une fonctionnalité individuelle ?**

Les utilisateurs ne peuvent pas accéder à cette fonctionnalité sur aucun tableau, mais les autres fonctionnalités de la même catégorie restent disponibles si activées.

**Référence et exemples**

**Quelles fonctionnalités puis-je contrôler individuellement ?**

Consultez la référence dans le produit pour la liste actuelle. Les exemples dans Créer du contenu incluent Créer des pense-bêtes, Regrouper des pense-bêtes, Créer et modifier des documents, des tables, des diagrammes et des opérations de texte telles que réécrire, raccourcir, ajuster le ton et traduire. Images inclut Créer des images, Supprimer l'arrière-plan et Ajouter des sous-titres. Résumer l'activité inclut Récapitulatif et Résumé de la conversation. Les flux, les partenaires d’IA et les prototypes apparaissent s’ils sont activés pour votre organisation.

**Puis-je voir quels modèles alimentent certaines fonctionnalités ?**

Oui. Les admins peuvent consulter les modèles associés à chaque fonctionnalité d'IA dans l'espace de référence pour soutenir l'examen et la gouvernance.

## Bloquer l'utilisation de Miro IA avec des Garde-fous Intelligents

Utilisez les Garde-fous Intelligents pour bloquer toutes les interactions propulsées par l'IA dans Miro lorsque vous avez besoin de protéger des données sensibles ou classifiées. Lorsqu'un de ces garde-fous est appliqué, tous les outils Miro IA sont désactivés sur les tableaux concernés, tandis que la collaboration sans IA reste disponible. Pour des informations sur le contexte et la configuration, consultez l'aperçu des Garde-fous Intelligents et Définir des garde-fous.

**Objectif et portée**

**Que fait la fonction « Bloquer l'utilisation de Miro IA » ?**

Elle désactive toutes les fonctionnalités Miro IA (par exemple, génération de texte, génération/reconnaissance d'images, suggestions intelligentes) là où ce garde-fou s'applique, empêchant toute interaction pilotée par l'IA avec des contenus sensibles ou classifiés.

**Qu'est-ce qui reste disponible pour les utilisateurs ?**

Les utilisateurs peuvent continuer la collaboration régulière, sans IA. Le contenu généré par l’IA déjà existant reste sur les tableaux et peut être consulté, déplacé ou modifié manuellement, mais les utilisateurs ne peuvent pas utiliser Miro IA pour le modifier ou le régénérer.

**Accès et prérequis**

**Qui peut configurer ce garde-fou et où ?**

Les admins de contenu sensible configurent les garde-fous dans *Enterprise Guard* sous Classification des données → Garde-fous. (Les admins d’entreprise attribuent le rôle d'admin de contenu sensible.)

**Que faut-il avant d'attribuer ce garde-fou ?**

Définissez vos niveaux de classification et (facultativement) la classification automatique pour que le garde-fou puisse être appliqué par classification (par exemple, INTERNE, CONFIDENTIEL).

**Comportement et impact**

**Qui est concerné lorsque la barrière de sécurité s'applique ?**

Tout le monde, y compris les propriétaires et les copropriétaires des tableaux, ne peuvent pas accéder ou invoquer Miro IA sur les tableaux concernés.

**Supprime-t-elle le contenu existant de l’IA ?**

Non. Elle empêche les interactions futures avec l’IA ; le contenu existant de l’IA reste disponible pour consultation et modifications manuelles.

**Quand les changements prennent-ils effet ?**

Après avoir publié vos mises à jour de barrière de sécurité, l'application est immédiate sur les tableaux concernés.

**Configuration et paramétrage**

**Comment activer "Bloquer l'utilisation de Miro IA" pour une classification ?**

1. Allez à *Enterprise Guard* → Classification des données → **Garde-fous**.
2. Cliquez sur l'icône **Modifier** pour un niveau de classification (par exemple, CONFIDENTIEL).
3. Cochez la case **Bloquer l'utilisation de Miro IA** et cliquez sur **Terminé**.
4. Cliquez sur **Suivant** et examinez l'impact, puis cliquez sur **Publier** pour appliquer.

**Devrais-je utiliser le mode Défaut ou Strict ?**

En mode par défaut, les garde-fous ne remplaceront pas les paramètres de partage existants. En mode strict, les garde-fous remplacent le partage actif et appliquent les contrôles les plus stricts. Choisissez en fonction de vos besoins en matière de gestion du changement.

**Expérience utilisateur**

**Que verront les utilisateurs sur les tableaux où l'IA est bloquée ?**

Les points d'entrée de l'IA Miro apparaissent désactivés ou indisponibles, et les utilisateurs ne peuvent pas invoquer les outils d'IA à partir du canevas ou des menus sur ces tableaux.

**Les utilisateurs peuvent-ils demander des exceptions sur un seul tableau ?**

Non. Le garde-fou est appliqué par la politique de classification. Modifiez la classification du tableau (ou la politique pour ce niveau) pour modifier l'application.

**Interactions avec d'autres contrôles**

**Comment cela est-il lié aux contrôles d'administration Miro IA granulaires ?**

Les contrôles granulaires gèrent qui peut utiliser des fonctionnalités IA spécifiques. Le garde-fou est une couche de politique : lorsqu'il est actif, il bloque l'IA quelle que soit l'activation des fonctionnalités.

**En quoi cela diffère-t-il du blocage de prompt ou de la modération IA ?**

- **Blocage de prompt** arrête les prompts sensibles lors de la soumission ; l'IA reste disponible pour des prompts non sensibles.
- **Modération IA** filtre le contenu nuisible ou inapproprié.
- **Blocage de l'utilisation de Miro IA** désactive complètement l'IA sur les tableaux affectés.

**Résolution des problèmes**

**L’IA apparaît toujours sur certains tableaux. Que dois-je vérifier ?**

- Confirmez que la classification du tableau est l'une de celles où le garde-fou est activé et que vous avez cliqué sur **Publier** après avoir modifié les garde-fous.
- Si vous utilisez la classification automatique, vérifiez que la classification du tableau a été mise à jour en fonction des contenus actuels.
- Dans les modes Strict vs Par défaut, assurez-vous que votre attente correspond au mode de déploiement que vous avez sélectionné.

**Nous devons réactiver l'IA pour quelques travaux.**

Ajustez le garde-fou pour la classification concernée ou reclassez les tableaux qui doivent autoriser l'IA, puis publiez la mise à jour.

## Tableau de bord Vue d'ensemble de l'analytique admin

**Périmètre et mesures**

**Que couvre le tableau de bord Vue d'ensemble ?**

Tableaux, Utilisateurs, Équipes, Licences et Modèles, avec tendances historiques le cas échéant.

**Comment est défini "Actif durant cette période" pour les Tableaux, Utilisateurs et Équipes ?**

- **Tableaux :** Tableaux uniques ouverts depuis le début de la période sélectionnée. Inclut les tableaux ensuite déplacés vers la Corbeille.
- **Utilisateurs :** Utilisateurs uniques ayant ouvert un tableau au moins une fois depuis le début de la période. Inclut les utilisateurs actuellement désactivés.
- **Équipes :** Équipes uniques avec au moins un membre ayant ouvert un tableau depuis le début de la période. Peut inclure des équipes déplacées par la suite vers la Corbeille.

**Les totaux excluent-ils les éléments dans la Corbeille ?**

Oui. Les totaux des Tableaux et Équipes excluent les éléments actuellement dans la Corbeille. Les décomptes "actifs" historiques peuvent inclure des éléments qui ont été ensuite placés dans la corbeille.

**Que montre le graphique des Licences ?**

Totaux et historique des allocations pour les licences complètes, Free et licences gratuites restreintes, reflétant combien de licences sont actuellement utilisées.

**Qu'affiche Modèles aujourd'hui ?**

Les modèles les plus populaires utilisés depuis l'intérieur d'un tableau. D'autres sources peuvent être ajoutées dans les futures versions.

**Comportement temporel et historique**

**Comment les valeurs historiques s'affichent-elles sur les graphiques d'aperçu ?**

Les widgets historiques affichent les valeurs à la date du dernier jour de chaque période. Jusqu'à un an d'historique est disponible ou aussi loin que les données existent.

**Fraîcheur des données et contrôles**

**À quelle fréquence les données de l'Aperçu sont-elles rafraîchies et où puis-je les voir ?**

Au moins une fois toutes les 24 heures. Un horodatage "Dernière mise à jour" est disponible dans le tableau de bord.

**Comment modifier la plage de temps ?**

Utilisez le sélecteur de plage de temps en haut à droite de la page d'Analytics.

## Modération de l’IA Miro

Avec la modération de Miro IA, les admins d’entreprise peuvent ajuster les niveaux de filtrage des prompts qui pourraient contenir des textes potentiellement nuisibles ou inappropriés. Vous pouvez définir la sensibilité de la modération de Miro IA au niveau de l’organisation pour filtrer le contenu, y compris la haine, le contenu sexuel, la violence et l’automutilation. Cela vous aide à aligner l’utilisation de Miro IA avec les exigences, politiques et tolérances aux risques de votre organisation. Pour plus d’informations, consultez la [documentation sur la modération de Miro IA](../../enterprise-guard/ai-trust/04-ai-moderation-overview.md).

**Objectif et portée**

**Qu’est-ce que la modération IA dans Miro ?**

La modération IA permet aux admins d’entreprise de définir un niveau de filtrage à l’échelle de l’organisation (Strict, Défaut ou Minimal) qui examine les prompts pouvant entraîner du contenu préjudiciable ou inapproprié (par exemple, haine, contenu sexuel, violence, automutilation).

**Qui peut le configurer et sur quels forfaits ?**

Les admins d’entreprise avec Enterprise Guard peuvent configurer ce paramètre dans les paramètres de l’organisation.

**Est-ce que cela fonctionne si mon organisation connecte son propre LLM (par exemple, une intégration directe avec un fournisseur) ?**

Si un LLM personnalisé est connecté, le sélecteur de modération peut être désactivé pour cette intégration et le niveau précédemment choisi ne s’appliquera pas.

**Accès et prérequis**

**Qui peut l'activer et de quoi ai-je besoin ?**

Les admins d'entreprise sur le plan Enterprise avec le module complémentaire Enterprise Guard peuvent configurer la modération de l'IA dans les paramètres de l'organisation.

**Comment l'activer ?**

Allez dans Paramètres → Miro IA → Modération, choisissez Strict/Par défaut/Minimal, puis cliquez sur **Enregistrer les modifications**. L'application est immédiate à l'échelle de l'organisation.

**Niveaux et comportement**

**Que signifient les niveaux ?**

- **Strict :** Bloque le contenu par défaut + contenu à faible à risque modéré (par exemple, haine subtile/codée, contenu sexuel suggestif, violence non graphique, mentions d'auto-mutilation non explicites).
- **Par défaut (recommandé) :** Bloque les contenus modérément à sévèrement nuisibles.
- **Minimal :** Bloque uniquement les contenus sévèrement nuisibles.

**Quand les modifications prennent-elles effet ?**

Immédiatement pour l'ensemble de l'organisation.

**Les modifications sont-elles suivies ?**

Oui. Les mises à jour sont enregistrées dans le journal d'audit de votre organisation.

**Configuration et mise en place**

**Où puis-je régler ou mettre à jour le niveau de modération ?**

Allez dans Paramètres → Miro IA → Modération, choisissez Strict/Par défaut/Minimal, puis cliquez sur **Enregistrer les modifications**.

**Quel niveau de départ recommandez-vous ?**

Par défaut convient à la plupart des organisations ; ajustez en fonction des retours des pilotes et de la tolérance au risque.

**Interactions avec d'autres contrôles**

**Comment la Modération IA se rapporte-t-elle aux garde-fous et aux contrôles de prompt ?**

- **Garde-fous Intelligents :** Si un tableau est couvert par le garde-fou "Bloquer l'utilisation de Miro IA", l'IA est désactivée, quel que soit le niveau de modération.
- **Blocage des prompts :** Fonctionne en parallèle de la Modération. Le blocage des prompts arrête les prompts sensibles à la soumission; la Modération filtre les catégories nuisibles.
- **Contrôles granuleux d'admin :** Les bascules de fonctionnalités gouvernent qui peut accéder aux fonctionnalités IA lorsque l'IA est disponible.

**Dépannage et meilleures pratiques**

**Nous avons trop de faux positifs.**

Envisagez de passer de Strict à Par défaut (ou de Par défaut à Minimal) et publiez des exemples d'utilisation acceptable. Si les problèmes persistent après l'ajustement des paramètres, contactez votre Customer Success Manager de Miro pour le signaler afin que notre équipe produit puisse examiner la situation.

**Nous voyons des contenus nuisibles passer à travers.**

Passez à Par défaut ou Strict et fournissez des directives internes. Revoyez après les mises à jour des politiques/réglementations. Si les problèmes continuent après ces changements, contactez votre Customer Success Manager de Miro pour le signaler afin que notre équipe produit puisse examiner la situation.

## Blocage des prompts

Le blocage des prompts permet aux admins de contenu sensible d'empêcher les utilisateurs de soumettre des prompts IA contenant des informations délicates, aidant ainsi à garder les données sensibles hors de Miro IA dans toute votre organisation. Miro analyse le texte qu'un utilisateur entre dans le champ prompt ainsi que tout contenu textuel qu'il ajoute depuis le tableau. Si ce contenu correspond aux badges de sensibilité ou aux motifs de code source sélectionnés dans la configuration du blocage des prompts, Miro bloque la soumission du prompt.  Pour plus d'informations, consultez la [documentation sur le blocage des prompts](../../enterprise-guard/ai-trust/06-prompt-blocking-overview.md).

**Objectif et portée**

**Qu’est-ce que le blocage de prompt ?**

Le blocage de prompt empêche les utilisateurs de soumettre des prompts IA contenant des informations sensibles. Miro analyse le texte qu'un utilisateur saisit dans le champ de prompt ainsi que tout contenu textuel qu'il ajoute depuis le tableau ; si cela correspond à des étiquettes de sensibilité ou des modèles de code source sélectionnés, la soumission est bloquée et un message de politique est affiché. Pour le moment, nous ne prenons en charge que le contenu basé sur du texte.

**En quoi le blocage de prompt diffère-t-il de l'analyse des tableaux ?**

L'analyse des tableaux trouve le contenu sensible sur les tableaux et peut auto-classifier les tableaux ; le blocage de prompt vérifie ce que les utilisateurs tentent d'envoyer à Miro IA lors de la soumission.

**Quelles étiquettes de sensibilité sont prises en charge ?**

Utilisez les catégories au niveau de l'organisation listées dans les badges de sensibilité et la référence des infotypes.

**Qu'est-ce que l'analyse du code ?**

L'analyse du code bloque les prompts contenant du code source reconnaissable ; elle exige, par conception, un bloc de code minimal (par exemple, 5+ lignes) pour être déclenchée. Activez/désactivez cette option dans la configuration du blocage de prompts.

**Le contenu non textuel (par exemple, les images) est-il analysé ?**

Non. Pour le moment, le blocage de prompt ne prend en charge que le contenu basé sur du texte.

**Accès et conditions préalables**

**Qui peut l'activer et de quoi ai-je besoin ?**

Les Admins de Contenu Sensible sur Enterprise avec le module complémentaire Enterprise Guard peuvent l'activer dans Paramètres → Enterprise Guard → Découverte de données → Configuration.

**Comment l'activer ?**

Ouvrez le blocage des prompts → Activez, choisissez Sélectionner tout ou des catégories de badge spécifiques, activez éventuellement l'analyse du code, puis Activez. L'application est immédiate à l'échelle de l'organisation.

**Gestion et modifications**

**Comment ajuster les badges ou l'analyse du code par la suite ?**

Allez dans Paramètres → Enterprise Guard → Découverte de données → Configuration → Blocage de prompt → Gérer,

- **Badges :** Cochez la case *Sélectionner tout* pour sélectionner toutes les catégories ou cochez les cases de catégories spécifiques de badges.
- **Analyse du code :** Activez l'analyse du code pour bloquer les prompts qui incluent du code source (minimum 5 lignes). Pour plus d'informations, consultez l'analyse du code.

Les modifications prennent effet immédiatement.

**Que se passe-t-il avec les prompts après avoir modifié les paramètres ?**

Les éléments récemment débloqués passeront. Les éléments qui correspondent toujours aux modèles bloqués restent arrêtés.

**Expérience utilisateur**

**Que voit un utilisateur lorsqu'un prompt est bloqué ?**

Un message de politique apparaît à l'endroit où il a saisi le prompt, et la demande n'est envoyée à aucun LLM.

**Le contenu non textuel (par exemple, les images) est-il scanné ?**

Non. Pour le moment, le blocage des prompts ne prend en charge que le contenu basé sur du texte.

**Interactions avec d'autres contrôles**

**Comment le blocage de prompt fonctionne-t-il avec les garde-fous et la modération ?**

- **Garde-fous intelligents :** Si la directive « Bloquer l'utilisation de Miro IA » s'applique, l'IA est désactivée ; le blocage de prompt ne se déclenche pas car les prompts ne peuvent pas être soumis.
- **Modération IA :** Les deux peuvent s'appliquer lorsque l'IA est disponible—le blocage de prompt arrête les données sensibles ; la modération filtre les catégories nuisibles.
- **Contrôles administratifs granulaires :** L'accès aux fonctionnalités s'applique uniquement lorsque l'IA est disponible et que le prompt n'est pas bloqué.

##

## Enterprise Guard et Microsoft Purview DSPM pour l'intégration IA

Pour les organisations utilisant Microsoft Entra ID (anciennement Azure AD) comme fournisseur d'identité, Enterprise Guard transmet en toute sécurité les prompts IA et les réponses à la gestion de posture de sécurité des données (DSPM) de Microsoft Purview pour l'IA. Les équipes de sécurité et de conformité peuvent alors surveiller, auditer et contrôler l'utilisation de l'IA générative à partir d'une plateforme fiable unique, réduisant ainsi la charge opérationnelle, atténuant les risques tels que les fuites de données et l'utilisation abusive, et renforçant la gouvernance IA de niveau entreprise de Miro. Pour plus d'informations, consultez la [documentation sur l'intégration Enterprise Guard et Microsoft Purview DSPM pour l'IA](../../enterprise-subscription-management/integrations/02-enterprise-guard-and-microsoft-purview-dspm-for-ai-integration-overview.md).

**Objectif et portée**

**Qu'est-ce que l'intégration DSPM de Microsoft Purview pour l'IA dans Miro ?**

Une intégration qui transmet les prompts et réponses de Miro IA au DSPM de Microsoft Purview pour que les équipes de conformité et de sécurité puissent surveiller, auditer et gérer l'activité de l'IA en un seul endroit.

**Qui peut utiliser cette intégration ?**

Les forfaits Enterprise avec Enterprise Guard, gérés par les admins d'entreprise ayant accès aux intégrations Enterprise. Votre organisation Miro doit utiliser Microsoft Entra ID pour l'authentification unique. Une licence Microsoft Purview est requise.

**Quels sont les avantages ?**

Visibilité centralisée de l'utilisation de Miro IA dans le hub IA de Purview, auditabilité des prompts et réponses, et alignement avec vos politiques de gouvernance existantes dans Purview.

**Quelles activités Miro IA sont incluses aujourd’hui ?**

Actuellement, seules les demandes et réponses textuelles via les fonctionnalités de Miro IA sont transférées. Les contenus d'image ne sont pas transférés.

**Toutes les activités des utilisateurs sont-elles enregistrées ?**

Seules les activités des utilisateurs qui se connectent à Miro via le locataire Microsoft Entra configuré sont transférées vers Purview.

**Combien de temps faut-il pour que l'activité apparaisse dans Purview ?**

En général, 10 à 30 minutes après l'action IA dans Miro. Consultez-la dans Microsoft Purview → DSPM pour IA → Explorateur d'activités, ou vérifiez les journaux d'audit.

**Y a-t-il des limitations notables ?**

Actuellement, un seul locataire Entra peut être configuré à la fois. Dans des environnements multi-fournisseurs d'identité ou multi-locataires, seules les activités des utilisateurs authentifiés via le locataire configuré sont enregistrées. Les images ne sont pas incluses.

**Configuration et installation**

**Comment activer l'intégration ?**

Dans Miro : Paramètres Enterprise → Intégrations Enterprise → activer Microsoft Purview DSPM pour IA → entrer votre ID de locataire Entra → Connecter → se connecter avec un compte qui peut accorder un consentement admin à l'échelle du locataire → accepter l'application de gouvernance Miro IA → confirmer Connecté dans Miro.

**Quelles sont les conditions préalables ?**

- **Miro :** forfait Enterprise avec Enterprise Guard, rôle d’admin d’entreprise, ID Entra configuré pour l’authentification unique. Pour activer cette fonctionnalité, contactez votre responsable Customer Success.
- **Microsoft :** licence Microsoft Purview, l’ID de locataire Entra utilisé pour l’authentification unique avec Miro et un rôle Entra qui peut accorder un consentement admin à l’échelle du locataire.

**Comment vérifier que la configuration fonctionne ?**

Effectuez une simple action Miro IA, attendez 10 à 30 minutes, puis vérifiez dans Microsoft Purview → DSPM pour IA → l'Explorateur d'activités pour les nouvelles entrées Miro.

**Comment déconnecter ou changer de locataire ?**

Dans Miro : Intégrations Enterprise → Microsoft Purview pour IA → Déconnecter. Pour changer de locataires, déconnectez-vous d'abord, puis reconnectez-vous en utilisant le nouvel ID de locataire.

**Utilisation et gouvernance**

**Où puis-je voir les données transférées dans Purview ?**

Microsoft Purview → DSPM pour IA → Explorateur d'activités. Vous pouvez également consulter les détails dans les journaux d'audit.

**Puis-je exporter ou archiver les journaux d'activité IA ?**

Utilisez les outils d'export de Microsoft Purview. Miro transfère l'activité à votre espace Microsoft où vos politiques s'appliquent.

**Puis-je appliquer les politiques Purview aux données de Miro IA ?**

Oui. Une fois intégrées, les données suivent le modèle de gouvernance Purview de votre organisation.

**Qu'en est-il des responsabilités en matière de confidentialité et de sécurité ?**

Miro transfère les prompts et réponses à votre espace Microsoft. La gouvernance et les contrôles d'accès sont gérés dans Purview au sein de votre environnement.

**Résolution des problèmes et service d’assistance**

**L’étape de consentement échoue ou se répète. Que dois-je vérifier ?**

Assurez-vous que le compte utilisé pour Connect peut accorder un consentement administrateur à l'échelle du locataire dans Entra, ou impliquez un administrateur global Microsoft.

**Je ne vois aucune activité dans Purview. Que faire maintenant ?**

Confirmez qu'Enterprise Guard est activé et que vous avez accès aux intégrations Enterprise. Vérifiez que l'ID du locataire correspond exactement à celui de votre authentification unique Miro. Assurez-vous qu'une action de test IA a été effectuée par un utilisateur s'authentifiant via ce locataire. Vérifiez les licences et les filtres Purview. Attendez jusqu'à 30 minutes pour l'ingestion.

**Nous utilisons plusieurs fournisseurs d’identité ou locataires. Tous les utilisateurs seront-ils enregistrés ?**

Non. Seule l'activité des utilisateurs se connectant via le locataire Entra configuré unique est transmise.

**Qui supporte quoi ?**

Contactez le service d’assistance Miro pour l'installation ou la connectivité dans Miro. Pour les problèmes à l'intérieur de Microsoft Purview, contactez le service d’assistance Microsoft.
