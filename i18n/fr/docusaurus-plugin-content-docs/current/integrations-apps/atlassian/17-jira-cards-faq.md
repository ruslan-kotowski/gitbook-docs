---
title: FAQ sur les cartes Jira
article_id: 360013463739
translation_id: 8249416498962
locale: fr
sidebar_position: 17
created_at: '2022-10-24T16:52:55Z'
updated_at: '2025-10-14T19:23:32Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
---

Cet article répond aux questions les plus fréquentes sur le fonctionnement de notre intégration des cartes Jira.

**Sécurité**

**Comment l’authentification Jira-Miro fonctionne-t-elle ?**

Consultez les articles du Centre d’assistance pour

- **Jira Server sur site**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Tiers) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Data Center sur site**
  - [OAuth 2.0](https://help.miro.com/hc/articles/25753304280466)
  - (Tierce partie) [OAuth 2.0](https://help.miro.com/hc/articles/25692796700306)
- **Jira Cloud**
  Sélectionnez depuis la page des paramètres des cartes Jira.
  - [OAuth 2.0](https://help.miro.com/hc/articles/8588617184402) (3LO)

**Les données sont-elles sécurisées lors de leur transit entre Jira et Miro ?**

Nous utilisons le protocole de sécurité TLS. Il crypte les messages HTTP avant leur transmission et décode les messages à leur arrivée. Nous prenons également en charge le TLS mutuel pour le [forfait Enterprise](https://help.miro.com/hc/articles/360017730433).

**Prenez-vous en charge le TLS mutuel ?**

Oui, [en savoir plus](https://help.miro.com/hc/articles/4410562720658).

**Miro conservera-t-il les données de Jira du client ?**

Oui, Miro conserve les données des cartes qui sont ajoutées au tableau.

**Combien de temps dure la période de conservation et comment les données seront-elles sécurisées ?**

Pour OAuth 1.0, (Jira Server ou Data Center), les données sont également mises à jour si les webhooks sont paramétrés pendant la configuration du plugin des cartes Jira. La période de conservation est illimitée. Seuls les protocoles de sécurité généraux de Miro sont appliqués.

**Pouvons-nous restreindre les informations récupérées à partir de Miro ?**

Nous n’avons trouvé aucune mention dans la [documentation d’Atlassian](https://developer.atlassian.com/server/jira/platform/webhooks/) expliquant comment limiter le partage des informations à certains champs seulement.

**Pouvons-nous avoir un diagramme montrant le flux de données entre Jira et Miro ?**

Des informations détaillées se trouvent dans [cet article destiné aux développeurs Jira](https://developer.atlassian.com/server/jira/platform/oauth/). Nous mettons en œuvre notre intégration conformément à la documentation d’Atlassian.

**Comment le jeton est-il géré ?**

Oauth 1.0 : seul le jeton d’accès est utilisé. Le jeton d’accès est conservé [pendant 5 ans sauf s’il est révoqué](https://developer.atlassian.com/server/jira/platform/oauth) (aucune option de personnalisation, cette politique étant définie du côté d’Atlassian. Vous pouvez révoquer le jeton du côté de Jira à partir de l’interface utilisateur Web). N’oubliez pas que chaque nouveau jeton empêche l’intégration de fonctionner et nécessite de [relancer la connexion](https://help.miro.com/hc/articles/360019501754#Step_2_-_Connection).

OAuth 2.0 : le jeton d’accès dure 1 heure. Le jeton de rafraichissement dure 90 jours (si vous passez 90 jours sans utiliser l’intégration, vous devrez vous ré-authentifier).

**Un jeton d’accès unique est-il utilisé pour l’ensemble des accès clients à Jira ?**

Chaque utilisateur Miro qui souhaite importer, créer ou modifier des cartes Jira doit se connecter avec ses propres identifiants Jira. Toutes les actions citées ci-dessus ne peuvent être accomplies que pour le compte d’identifiants Jira individuels.

**Comment les jetons de requêtes, les jetons d’accès, les clés privées et les autres secrets/identifiants OAuth sont-ils sécurisés ?**

Au cours de l’intégration, seuls les jetons d’accès sont utilisés. Ils sont stockés de manière sécurisée dans la base de données et ne sont utilisés que du côté du serveur.

Pour OAuth 1.0. (Jira Server et Data Center), l’authToken n’est utilisé que pour le webhook. Il ne s’agit pas du jeton d’authentification utilisé par OAuth. Les requêtes sont envoyées par l’intermédiaire d’une connexion cryptée. La clé secrète est générée automatiquement et est associée par équipe.

**Quels points d’extrémité votre intégration utilise-t-elle ?**

```
POST /rest/api/2/issue - créer un nouveau ticket
```

```
PUT /rest/api/2/issue/id - mettre à jour le ticket
```

```
GET /rest/api/2/user/picker?query=xx
```

```
GET /rest/api/2/myself
```

```
GET /rest/api/2/filter/favourite
```

```
GET /rest/api/2/issue/picker
```

```
GET /rest/api/2/serverInfo
```

```
GET /rest/api/2/issue/$key
```

```
GET /rest/api/2/issue/createmeta
```

```
GET /rest/api/2/issue/$key/editmeta
```

```
GET /rest/api/2/priority
```

```
GET /rest/api/2/issuetype
```

```
GET /rest/api/2/mypermissions
```

Pour OAuth 1.0 (Jira Server et Data Center), nous utilisons en plus :

```
POST /rest/webhooks/1.0/webhook
```

**Les cartes fonctionneront-elles avec Jira Data Center ?**

Oui. Nous sommes approuvés par Atlassian et une grande partie de notre clientèle utilise déjà les cartes Jira avec Data Center avec succès. La procédure d’installation est la même.

**Quelles adresses IP utilisez-vous pour communiquer avec le système Jira ?**

La liste de nos adresses IP statiques se trouve [ici](https://help.miro.com/hc/articles/360017572694).

Notez que ces adresses ne sont utilisées que pour communiquer avec le système Jira. Les adresses IP de l’application Miro sont dynamiques et pour garantir l’efficacité des fonctionnalités des tableaux de Miro (dont certaines concernent les cartes Jira), nous vous demandons d’[ajouter nos domaines à votre liste d’autorisations](https://help.miro.com/hc/articles/360017572694).

**Pouvons-nous intégrer Jira à Miro, mais bloquer dans Miro les tickets Jira dont le niveau de sécurité est défini sur « Privé » ?**

Non, ce n'est pas une option. Les niveaux de sécurité de Jira ne correspondent pas à ceux de Miro.

**Général**

**Pouvons-nous connecter Miro à Jira si nous utilisons un serveur Jira ?**

Étant donné que Miro est un outil en ligne, vous ne pouvez vous connecter à Jira que lorsque votre instance est ouverte à l'Internet public.

**Pouvons-nous connecter plusieurs instances Jira en même temps ?**

Oui. Cependant, gardez à l'esprit que connecter une instance Jira consiste à établir le lien initial, tandis qu'une connexion active se réfère à l'instance liée actuellement en cours d'utilisation. Une connexion active définit d'où les cartes Jira sont importées lorsque vous ouvrez l'application Jira Cards, et pour quelle instance les utilisateurs sont autorisés. Pour un utilisateur donné, il ne peut y avoir qu'une (1) connexion active à la fois. Avec OAuth 2.0, un utilisateur peut modifier n'importe quelle carte Jira associée à n'importe quelle instance liée pour laquelle il est déjà authentifié. Pour tout autre protocole d'authentification, toute l'équipe partage une instance active et ne peut qu'importer et interagir avec les cartes de cette instance. Vous pouvez définir plusieurs paramètres au niveau de l'organisation et passer d'une connexion active à une autre au niveau de l'équipe.

**Quel est le processus de migration de Server vers Cloud ?**

Comme votre URL de base Jira changera inévitablement lors de la migration vers Cloud, l’intégration cessera de fonctionner sans modification de notre côté. Veuillez [contacter le service d’assistance Miro](https://help.miro.com/hc/articles/360020185799) pour obtenir de l'aide.

**Miro créera-t-il un webhook par équipe, par projet ou par instance Miro ?**

Si vous activez le webhook automatique dans vos paramètres Miro, alors la création des webhooks se fait automatiquement. Si vous utilisez une autorisation au niveau de l'équipe avec Jira, Miro crée des webhooks par équipe. Si vous utilisez une autorisation au niveau de l'organisation, alors Miro crée des webhooks par organisation.

**Le plugin des cartes Jira prend-il en charge les projets nouvelle génération ?**

Oui.

Notez que pour l’instant, aucun lien ou champ Epic n’est disponible lors de la création d’une carte Jira pour un projet nouvelle génération du côté de Miro.

**Les champs personnalisés de Jira sont-ils pris en charge ?**

Oui, nous prenons en charge presque tous les champs personnalisés des types de *base*. Si vous avez un champ de type de données *complexes*, il pourrait ne pas être pris en charge et provoquer un comportement inattendu lors de la mise à jour ou de la création de cartes Jira sur le tableau.

**Que se passera-t-il avec les cartes Jira existantes si nous basculons sur une autre instance Jira ?**

Actuellement, lorsque vous déplacez des tickets Jira d’un projet à un autre dans Jira, ils ne sont plus mis à jour du côté de Miro.

Pour contourner ce problème, nous vous suggérons de copier l’URL d’un ticket Jira (Ctrl/Cmd+C) et de la coller sur le tableau de Miro (Ctrl/Cmd+V). Ainsi, une carte Jira affichera les nouvelles valeurs et sera mise à jour automatiquement.

**Si un tableau est déplacé vers une autre équipe Miro, qu’adviendra-t-il des cartes Jira présentes sur ce tableau ?**

Les cartes Jira resteront sur le tableau, mais personne ne pourra les modifier (même si la même instance Jira est configurée pour l’équipe cible).

Si vous cliquez sur une carte, vous verrez le message suivant : *« La carte JIRA a été importée depuis un autre compte »*. Si vous souhaitez modifier ces cartes, veuillez les réimporter sur le tableau.

**Y a-t-il des frais supplémentaires à prévoir pour l’intégration des cartes Jira ?**

Les cartes Jira sont disponibles sur tous les forfaits payants et Education sans frais supplémentaires (forfaits Starter, Business, Education et Enterprise).

**Un utilisateur peut-il accéder à toutes les cartes Jira sur le tableau ?**

Les autorisations de l'intégration des cartes Jira garantissent que les utilisateurs ne peuvent créer et modifier des cartes que dans les projets Jira auxquels ils ont accès.

Tous les widgets d’un tableau Miro sont visibles par tous les utilisateurs ayant accès à ce tableau. Ainsi, si une personne ne dispose pas d'identifiants Jira ou n'a pas les bons identifiants, elle pourra voir la carte Jira réduite sur le tableau Miro (le titre ainsi que quelques autres champs), mais elle ne pourra pas développer la carte pour consulter son contenu complet ou la modifier.

**Atlassian a-t-il cessé le service d’assistance pour Jira Server ?**

Oui, Atlassian a cessé le service d’assistance pour Jira Server à partir de février 2024.

**La Planification/Jira Cards de Miro prend-elle en charge les champs personnalisés de Jira : types de tickets personnalisés et dépendances personnalisées ?**

Oui, les deux sont pris en charge. Si les champs **types de tickets personnalisés** et **dépendances personnalisées** sont configurés dans Jira, *et* que la Planification de Miro est authentifiée pour cette instance Jira, alors ces champs personnalisés sont disponibles dans la Planification.

**Miro prend-il en charge OAuth 2.0 pour Jira Data Center ?**

Oui. Voir [Connectez-vous à Jira Data Center en utilisant OAuth 2.0.](https://help.miro.com/hc/articles/25753304280466)

**Cartes Jira dans les tables et plannings**

**Comment puis-je importer des tickets Jira dans des tables et plannings ?**

Vous pouvez glisser-déposer une ou plusieurs cartes Jira directement dans une table ou un planning. C'est actuellement la seule façon de procéder.

**Tous les champs de la table sont-ils liés à Jira ?**

Non, seulement cinq champs de la table sont synchronisés avec Jira dans la version initiale :

Trois champs système Jira :

- Titre
- Description
- Date de fin (apparaît comme Date d'échéance dans Jira)

Deux champs personnalisés Jira :

- Date de début
- Estimation

**Quels champs dans la table ne se synchronisent pas avec Jira ?**

Les champs Responsable et État ne se synchronisent pas avec Jira et sont désactivés dans les tables et le planning. Ces champs et leur contenu existent, mais ne sont ni visibles ni modifiables dans les tables et le planning.

Vous pouvez toujours modifier ces champs directement dans les cartes Jira à l'aide du panneau latéral. Il suffit de faire glisser la ligne de la table ou du planning sur le canevas pour que votre carte Jira réapparaisse.

Tous les autres champs, en dehors des cinq listés ci-dessus (Titre, Description, Date de fin, Date de début, et Estimation) sont stockés uniquement sur Miro et ne se synchronisent pas avec Jira.

**Pourquoi ne puis-je pas modifier un champ dans la table ou le planning à partir des cinq champs Jira pris en charge mentionnés ci-dessus ?**

Le champ peut être absent de l'écran de modification de Jira.

Un moyen simple de savoir si le champ est présent dans l’écran de modification ou non :

Sur Miro, ouvrez le panneau latéral de la carte Jira. Vérifiez si le champ est présent dans le panneau latéral. Si le champ est absent, vous devez l'ajouter à l'écran de modification sur Jira.

Il y a quelques cas rares où les champs sont modifiables sur Jira, mais non présents dans l’écran de modification de Jira. Dans ce cas, ces champs ne peuvent pas être modifiés sur Miro.

Le champ que vous ne pouvez pas modifier est-il **la date de début** ou **l’estimation**? Si oui :

Le champ peut être absent de Jira ou manquant dans l’écran de modification (voir point précédent) ;

Il peut y avoir un problème de cartographie pour la date de début ou l’estimation, car ce sont des champs Jira personnalisés.

Nous cartographions ces champs selon cette logique :

- **Date de début** : Nous vérifions les champs nommés : Date de début, StartDate, Cible de début
- **Estimation** : Nous vérifions les champs nommés : Story Points, Estimation des story points, Story Point, StoryPoints, StoryPoint
- Si le champ Date de début ou Estimation n'est pas nommé comme l'un des noms suivants ci-dessus, cela pourrait expliquer pourquoi la modification ne fonctionne pas.

**Pourquoi la modification de la date de début ou de l'estimation sur une table ou un planning Miro ne fonctionne-t-elle pas ou met-t-elle à jour le mauvais champ dans Jira ?**

Nous nous appuyons actuellement sur un mappage automatisé pour les champs de date de début et d'estimation dans Jira. Étant donné que ceux-ci sont personnalisés sur Jira, il peut y avoir des cas où plusieurs champs de votre configuration Jira correspondent aux critères mentionnés ci-dessus.

Nous sélectionnons la première correspondance selon l'ordre des noms de champ mentionnés ci-dessus :

Par exemple, si un ticket Jira a à la fois des champs Story Points et Story point estimate, nous faisons correspondre le premier selon la liste ci-dessus, qui est Story Points. Par conséquent, toute modification du champ d'estimation dans le tableau mettra à jour le champ Story Points dans Jira, et non Story point estimate.

Pour l'instant, il n'y a pas de solution de contournement à ce problème. Si vous rencontrez ce problème, veuillez envoyer un avis à votre service d’assistance afin que nous puissions mieux comprendre vos besoins à mesure que nous développons de meilleures capacités de mappage de champ.

**Pourquoi ne puis-je pas importer des cartes Jira de 2 instances différentes dans une table ou un planning ?**

Actuellement, nous ne supportons qu'une seule instance Jira par table/planning. Une fois qu'une carte Jira est importée dans une table/planning, celle-ci est liée à cette instance Jira spécifique.

Même si tous les enregistrements Jira sont supprimés, le lien avec l'instance Jira d'origine reste. Pour importer des cartes d'une autre instance Jira, il est nécessaire de créer une nouvelle table/planning.

**Pourquoi ne puis-je pas voir ou modifier les champs État et Attributaire pour mes enregistrements Jira dans une table ou un planning ?**

Actuellement, les champs État et Attributaire de Jira ne sont pas pris en charge dans les tables et le planning. Nous avons décidé de désactiver ces champs dans les tables et le planning pour gérer les attentes, éviter toute confusion et potentielle perte de données. Les champs État et Attributaire de Jira et leur contenu existent, mais ils n'apparaissent pas dans les tables ou le planning.

Vous pouvez toujours modifier ces champs directement dans les cartes Jira en utilisant le panneau latéral. Il suffit de faire glisser la ligne de la table ou du planning dans le canevas pour faire réapparaître votre carte Jira.

**Plus d’informations :**

- [Cartes Jira](https://help.miro.com/hc/articles/360017572434)
- [Comment configurer et désinstaller les cartes Jira](https://help.miro.com/hc/articles/360019501754)
- [Comment configurer les webhooks pour les cartes Jira](https://help.miro.com/hc/articles/360017731113)
- [Problèmes possibles avec les cartes Jira et le module complémentaire Jira](https://help.miro.com/hc/articles/360017572654)
