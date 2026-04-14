---
title: Configurer Miro Insights
article_id: 30122381753106
translation_id: 30122381753106
locale: fr
sidebar_position: 0
created_at: '2025-10-10T10:26:28Z'
updated_at: '2025-11-25T15:54:01Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Connecter vos outils à Miro Insights est une première étape cruciale pour en tirer une réelle valeur. Les intégrations permettent à Miro Insights d'importer automatiquement les retours clients et les données pertinentes à partir de vos systèmes. Ce guide s'adresse aux admins d'entreprise qui vont activer ces connexions.

Si vous êtes un membre de l'équipe souhaitant utiliser Miro Insights après son installation, consultez l'article sur [l'utilisation de Miro Insights](../../miro-insights/use-miro-insights).

## Prérequis

Pour configurer les intégrations de Miro Insights, vous devez satisfaire aux exigences suivantes :

- Vous devez être **admin de l'entreprise dans Miro**.
- Vous devez avoir **un accès admin ou API sur la plateforme externe** que vous connectez.

:::note
Assurez-vous que votre **forfait Miro inclut Miro Insights**. Si Miro Insights est un module complémentaire ou est en version limitée, votre compte doit être éligible. De plus, certaines intégrations peuvent nécessiter des éditions spécifiques du logiciel externe. Par exemple, un accès API à certains CRM est disponible sur des forfaits de niveau supérieur.
:::

## Préparez vos sources de données

Avant de connecter vos sources de données à Miro Insights, il est important de préparer vos données et d'établir une taxonomie claire. Cette préparation vous permettra de tirer les insights les plus précis et exploitables de la plateforme.

### Nettoyez et optimisez vos données

Avant de synchroniser les données avec Miro Insights, nettoyez et optimisez vos sources de données :

- Supprimez les doublons et les éléments périmés.
- Nettoyez les retours incohérents ou non pertinents.
- Assurez-vous de la qualité des données dans vos systèmes source.
- Traitez les principales incohérences ou lacunes des données en amont.

### Établissez votre taxonomie

Bien que Miro Insights propose des catégories de base générées par l'IA, il est recommandé de définir votre propre taxonomie standardisée avant le déploiement. Cela assure la cohérence et améliore la qualité des insights dès le départ.

Considérez l'inclusion de ces catégories standard :

- Demandes de fonctionnalités
- Bugs
- Points de friction UX
- Segments de clientèle
- Niveaux de priorité
- Unités commerciales
- Initiatives stratégiques

Bonnes pratiques pour la taxonomie :

- Utilisez une terminologie qui correspond au langage de votre équipe.
- Créez des lignes directrices claires sur comment et quand utiliser chaque catégorie.
- Partagez la taxonomie avec votre équipe pour garantir une utilisation cohérente.
- Revoyez et peaufinez régulièrement les catégories selon les besoins.
- Envisagez de faire la cartographie avec vos initiatives stratégiques et vos OKRs.

:::tip
Contactez le service d’assistance de Miro Insights pour obtenir de l'aide dans la définition de votre taxonomie. Ils peuvent fournir des exemples et des meilleures pratiques basés sur d'autres clients dans votre secteur.
:::

## Connecter une intégration

Lorsque vos données sont prêtes, vous pouvez connecter vos intégrations. Miro Insights prend en charge une variété d'outils populaires dans les domaines du CRM, du service d’assistance, des appels de l'équipe de vente, de la gestion de projet et des plateformes de chat.

Dans l’onglet de paramètres **Intégrations & Automatisations**, vous pouvez consulter et gérer toutes vos intégrations connectées. Chaque intégration est listée avec son état de connexion et des options pour la configurer ou la déconnecter.

Pour connecter une intégration :

1. Depuis l'application **Miro Insights**, sélectionnez l'icône **Paramètres** en haut de la barre latérale gauche.
2. Dans le panneau **Paramètres**, allez à l'onglet **Intégrations & Automatisations**.
3. Sélectionnez **Connecter** à côté de l'intégration que vous souhaitez ajouter.
4. **Autoriser l'accès**. Une fenêtre contextuelle vous invitera à autoriser Miro Insights à accéder à cet outil.
   Cela implique généralement de se connecter au service externe et d'accorder les permissions. Par exemple, pour connecter Salesforce, vous devez vous connecter avec votre compte admin Salesforce et approuver l'intégration. Pour Slack, sélectionnez un espace de travail et autorisez l'application Slack de Miro Insights. Suivez les invites à l'écran pour chacun.
5. **Configurer les paramètres d'importation**. Une fois connectée, l'intégration apparaîtra comme "Connectée" avec des options de paramètres supplémentaires. Ici, vous pouvez définir :
   - **Importer les conversations depuis** : Pour les sources basées sur les conversations comme Gong ou Zendesk, vous pouvez choisir une date. Cela évite de rapatrier des données anciennes, sauf si vous le souhaitez.
   - **Règles d'importation automatique** : Activez ou désactivez l'importation automatique des nouveaux éléments. Vous pouvez activer cette fonctionnalité pour que les nouveaux appels ou tickets soient importés en continu. Si vous la désactivez, vous pouvez importer manuellement ou sélectivement des éléments.
   - **Si l'IA détecte des demandes avec** : Certaines sources vous permettent de filtrer par confiance de détection par IA.
   - **Détecter les problèmes** : Permet à Miro Insights d'identifier et d'extraire automatiquement les problèmes des retours clients. Ces problèmes peuvent inclure des défis d'utilisation, des problèmes de performance, des préoccupations de sécurité, etc.

D'autres options peuvent varier selon l'intégration. Par exemple, dans Jira, vous pouvez choisir de quels projets tirer les fonctionnalités ou de cartographier des champs personnalisés.

### Filtrage par IA

Certaines intégrations vous permettent de **filtrer par détection IA**. Cela signifie qu'Insights analysera une transcription d'appel et ne créera un élément de feedback que s'il est raisonnablement sûr qu'une demande de produit a été mentionnée. Cela réduit le bruit des conversations sans rapport. Vous pouvez ajuster le seuil de confiance ou désactiver cette option pour tout importer.

### Filtres par étiquette ou champ

Dans des outils comme Zendesk, vous pouvez spécifier une étiquette, par exemple "demande_de_fonctionnalité", afin que seuls les tickets avec cette étiquette soient intégrés. Dans Jira, vous pouvez sélectionner un projet spécifique ou un type de ticket à importer comme fonctionnalités.

### Synchronisation des tickets

Pour les outils de projet comme Jira, vous avez la possibilité de faire la cartographie des champs. La capture d'écran ci-dessus montre un exemple "Envoyer la valeur monétaire de la fonctionnalité au champ personnalisé" – vous pouvez sélectionner un champ personnalisé dans Jira à remplir avec l'impact financier calculé par Miro Insights, bouclant ainsi la boucle avec l'ingénierie. Cette étape est optionnelle mais peut être très efficace.

Connectez tous les systèmes pertinents. Nous recommandons de connecter au minimum un CRM et une source de support ou de feedback pour commencer, de façon à obtenir à la fois le contexte du compte et des retours bruts. Vous pourrez toujours en ajouter d'autres plus tard.

Une fois cette étape terminée, vous avez réussi à connecter vos intégrations à Miro Insights. Le système commencera à synchroniser les données. La synchronisation initiale peut prendre un peu de temps s'il y a beaucoup de données historiques (vous verrez les horodatages de la dernière synchronisation à côté de chaque intégration). Vous pouvez suivre l'état de la synchronisation dans la liste des intégrations — elle montre la dernière heure de synchronisation et offre une option de déconnexion si nécessaire.

## Importer des éléments manuellement

Vous pouvez également importer manuellement des fonctionnalités et des éléments de feedback en utilisant un fichier CSV. Ceci est utile pour des imports uniques ou si vous avez une liste de demandes de fonctionnalités ou de retours d'une autre source.

Pour importer des fonctionnalités via CSV :

1. Dans Miro Insights, allez à la vue **Backlog**.
2. Cliquez sur le bouton **Importer** en haut à droite.
3. Sélectionnez **Téléverser CSV**.
4. Sélectionnez la colonne de votre source de données CSV qui correspond le mieux aux propriétés de Miro Insights.
5. Sélectionnez **Importer la fonctionnalité** pour terminer le processus.

Vos fonctionnalités importées apparaîtront maintenant dans la section [Backlog](../../tools/use-miro-insights/05-backlog.md).

Pour importer des éléments de feedback via CSV :

1. Dans Miro Insights, allez à la vue **Feedback**.
2. Cliquez sur le bouton **Importer** en haut à droite.
3. Sélectionnez **Télécharger CSV**.
4. Faites correspondre les colonnes de votre CSV aux propriétés de feedback de Miro Insights (par ex. titre, description, source).
5. Sélectionnez **Importer le feedback** pour terminer le processus.

Vos items feedback importés apparaîtront maintenant dans la section [Feedback](../../tools/use-miro-insights/07-feedback.md).

## Connecter des outils non pris en charge en utilisant Zapier

Si vous avez un outil qui n'est pas directement pris en charge, vous pouvez souvent utiliser [Zapier](http://zapier.com/) pour transférer des données dans Miro Insights. Par exemple, vous pourriez créer le workflow Zapier suivant : Lorsqu'un Google Form est soumis ou lorsqu'une nouvelle entrée dans une base de données personnalisée apparaît, créer un élément de feedback dans Miro Insights.

Pour des étapes détaillées, consultez l'article sur [l'utilisation de Zapier avec Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/03-connect-tools-with-zapier.md).

## Étapes supplémentaires

Après avoir connecté vos intégrations, vous pouvez effectuer quelques étapes facultatives pour vous assurer que tout est correctement configuré :

### Importer ou vérifier les fonctionnalités

Si vous avez connecté un outil de suivi des tâches comme Jira, vérifiez le backlog dans Miro Insights pour voir si vos fonctionnalités ou vos épopées existantes sont apparues. Si ce n'est pas le cas, vous pouvez utiliser le bouton Importer dans la vue de backlog pour charger un fichier CSV ou déclencher une extraction depuis Jira. Assurez-vous que chaque fonctionnalité importée a un titre et une description clairs ; l'IA s'appuie sur ce texte pour faire correspondre les retours pertinents.

### Configurer les commandes Slack ou le transfert d'e-mails

Si vous avez ajouté Slack, informez votre équipe sur la façon d'envoyer des messages à Insights. Par exemple, cliquez droit sur un message > « Envoyer à Miro Insights ».

Pour les e-mails ou d'autres canaux, vous pouvez configurer le transfert. Certaines équipes créent une adresse e-mail spécifique qui se transfère automatiquement dans un outil comme Intercom ou un hook Zapier pour l'absorption.

> **Astuce** : Il est judicieux de revoir périodiquement vos paramètres d'intégration. Par exemple, si vous remarquez qu'un trop grand nombre de feedbacks triviaux proviennent d'une source, resserrez les filtres ou augmentez le seuil de confiance de l'IA. À l'inverse, si des données attendues manquent, assurez-vous que l'intégration est connectée avec le bon périmètre (par exemple, le bon projet ou la bonne étiquette). Une configuration d'intégration bien réglée maintient vos insights clairs et minimise les nuisances.

## Déconnecter une intégration

Si vous avez besoin de déconnecter une intégration :

1. Allez dans **Paramètres** > **Intégrations & Automations**.
2. Trouvez l'intégration que vous souhaitez supprimer.
3. Sélectionnez **Déconnecter** à côté.
4. Confirmez la déconnexion dans l'invite contextuelle.

Cela arrêtera toute synchronisation de données future depuis cette source.

> **Important** : Dans certains cas, par exemple Gong, déconnecter peut également supprimer les éléments de retours précédemment importés. Dans d'autres cas, comme Jira, les fonctionnalités existantes peuvent rester mais ne recevront pas de mises à jour. Consultez le comportement spécifique de chaque intégration dans la documentation ou contactez le service d’assistance en cas de doute.

Assurez-vous de communiquer avec votre équipe si vous déconnectez une source majeure, car cela pourrait affecter l'exhaustivité du backlog et des retours dans Miro Insights.

## Et ensuite ?

En connectant les intégrations, vous avez jeté les bases pour que Miro Insights offre des insights produits riches et continus. Les données commenceront à affluer, et l'IA commencera à établir des connexions.

Vous pouvez maintenant procéder à [l'utilisation de Miro Insights](../../miro-insights/use-miro-insights) ou en apprendre davantage sur les tâches administratives en cours, y compris les paramètres généraux, la gestion des équipes, les notifications et l'accès API dans le [guide d'administration de Miro Insights](../../miro-insights/set-up-and-manage-miro-insights/02-manage-miro-insights.md).
