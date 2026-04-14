---
title: Obsolète – Paramétrer et désactiver les cartes Jira en utilisant OAuth 1.0
article_id: 360019501754
translation_id: 7316339693586
locale: fr
sidebar_position: 14
created_at: '2022-08-25T09:57:38Z'
updated_at: '2025-11-25T16:03:53Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Disponible pour: Jira Cloud, Jira Server (sur site) et Datacenter (également
    protégé par LDAP) Installation par: admin d''équipe Miro et admin système Jira
    avec les autorisations administratives du projet'
---

:::note
La méthode d'authentification OAuth1.0 suivante ne sera plus prise en charge dans Miro à partir du 31 juillet 2025. OAuth1.0 est un [protocole d'authentification déprécié dans Jira](https://developer.atlassian.com/cloud/jira/software/jira-rest-api-oauth-authentication/#:~:text=Deprecation%20Warning&text=Additionally%2C%20if%20you%20have%20existing,OAuth%202.0%20and%20JWT%20respectively.) et ne devrait pas être utilisé. Ce changement fait partie d'une transition plus large vers OAuth2.0, qui est recommandée conformément aux meilleures pratiques en matière de sécurité. Il est conseillé aux utilisateurs de migrer vers OAuth2.0 pour garantir la continuité du support et la compatibilité avec les services de Miro.
:::

## Configuration de Miro sur Jira

:::warning
Si des problèmes techniques apparaissent, veuillez vous référer à notre article sur [Possible issues and how to resolve them](https://help.miro.com/hc/articles/360017572654).
:::

:::tip
En savoir plus sur les cartes Jira dans les articles [FAQ sur les cartes Jira](https://help.miro.com/hc/articles/360013463739) et [Comment configurer un webhook pour les cartes Jira](https://help.miro.com/hc/articles/360017731113).
:::

Configuration de Jira Cloud Jira Server et Jira Data Center

:::note
Notez queles menus de Jira peuvent varieren fonction de la version de Jira que vous utilisez, cependant, le flux général devrait être le même. Les instructions ci-dessous peuvent également être trouvées sur [cette page d’aide d’Atlassian](https://confluence.atlassian.com/adminjiraserver071/using-applinks-to-link-to-other-applications-802592232.html).
:::

### Étape 1 - Lien d’application

Commencez par créer un lien avec l’application et configurez-le.

1. Accédez à **Paramètres Jira** > **Produits** > **Intégrations** > **Liens d'application**  > **Créer un lien
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)***Notez que l'interface de Jira peut différer en fonction de votre version de Jira*
2. Choisissez **lien direct de l’application** et saisissez `https://miro.com/` dans le champ **URL de l’application**.
   Important : vous devez entrer l’URL dans ce format exact. Cliquez sur **Continuer**.
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)
    *Créer le lien*
3. Dans le menu suivant, cliquez simplement sur **Continuer** à nouveau.
4. Dans le menu **Réviser le lien**, vérifiez bien que l’URL est toujours exactement `https://miro.com/` et saisissez le **nom de l’application** de votre choix. Faites défiler vers le bas, et en bas, cochez la case **Créer un lien entrant**. *Ignorez le reste des champs* et cliquez sur **Continuer**.
   ![mceclip3.png](../../../../../../docs/integrations-apps/atlassian/images/21017004819346_mceclip3.png)  *Seul le champ Nom de l'application doit être rempli.*
5. Vous verrez ici les champs pour les valeurs Miro. Pour obtenir les valeurs, connectez-vous à Miro.
   - Pour l'intégration au niveau de l'équipe, allez dans **[Paramètres de l'équipe](https://help.miro.com/hc/articles/360021841280)** > **Applications et intégrations** > **Cartes Jira.**
   - Pour une intégration au niveau de l'organisation, allez dans [**Paramètres de l'entreprise**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **Applications** > **Gérer les applications** > **Cartes Jira** > **Paramètres**.
     > Si vous n’avez pas de cartes Jira dans votre liste d'applications, faites défiler jusqu'au haut de la section, cliquez sur **Installer des applications** et procédez à l'installation de l'application à partir du Marketplace de Miro. Une fois que vous voyez les cartes Jira sur la liste, cliquez pour les ouvrir.


     L’onglet du plugin s’ouvrira et vous pourrez voir **l’étape 1** pour obtenir les valeurs requises :

     ![Jira_Cards_values.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017515668626_Jira Cards values.jpg)*Valeurs des cartes Jira*
     Copiez les valeurs et ajoutez-les au menu **Réviser le lien** d'Atlassian.
6. Vous verrez le message de traitement pendant un instant ou deux :
   ![mceclip4.png](../../../../../../docs/integrations-apps/atlassian/images/21017528655634_mceclip4.png)
    *La dernière étape de la création du lien*

Et cela termine les étapes du côté Atlassian. Le lien apparaîtra dans la liste de vos liens d’application.

### Étape 2 - Connexion

Retournez à vos paramètres de carte Jira dans Miro et choisissez l’une des deux options : créer un webhook manuellement ou automatiquement. Si vous choisissez manuellement, décochez l'option. Veuillez voir plus d'informations dans [cet article](https://help.miro.com/hc/articles/360017731113). Nous vous recommandons vivement d’utiliser le webhook automatique pour ne pas avoir à le réinitialiser en cas de grosses mises à jour du plugin.

Enfin, saisissez votre URL Jira et cliquez sur **Connecter :**

![step_2.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017528650898_step%202.jpg)*Connexion des cartes Jira*

Pour obtenir l’URL de Jira, copiez l’URL de base de votre instance Jira. Nous acceptons les formats suivants :

`https://your-server.example.com/`
[https://your-server.example.com/
https://your-ip-address/](https://your-server.example.com/)[https://your-ip-address/](https://your-server.example.com/)

Si votre URL Jira n’est pas acceptée, veuillez vous référer à [cet article.](https://help.miro.com/hc/articles/360017572654) Veuillez également vérifier que Miro dispose d’un accès suffisant à votre Jira pour [établir la connexion.](https://help.miro.com/hc/articles/360017572694)

Vous avez maintenant connecté votre instance Jira à votre équipe Miro.

:::warning
Bien qu'Atlassian ait arrêté le support de Jira Server à partir de février 2024, Miro continuera de soutenir l'intégration des cartes Jira pour Jira Server dans un avenir prévisible.
:::

1. Allez à `https://your-jira-server/plugins/servlet/applinks/listApplicationLinks`[.](https://your-jira-server/plugins/servlet/applinks/listApplicationLinks) Si "Liens d'application" n'est pas sélectionné, cliquez dessus. ![jira_server_create_application_links.png](../../../../../../docs/integrations-apps/atlassian/images/21017515683858_jira_server_create_application_links.png)*Liens d'application du serveur Jira*
2. Cliquez sur **Créer un lien**. Sélectionnez « produit Atlassian » et fournissez l'**URL de l'application**, "https://miro.com". Cliquez sur **Continuer**. ![jira_server_create_link.png](../../../../../../docs/integrations-apps/atlassian/images/21017528656274_jira_server_create_link.png)*Configuration de l'URL de l'application*
3. Vous serez dirigé vers la boîte de dialogue "Lier des applications". Ajoutez un **Nom d'application** (par exemple, Miro Jira Card) et sélectionnez "Application Générique" pour le **Type d'application**.
   Vous devriez voir l'URL de votre application Jira sous "Vous créez un lien depuis :", et vous devriez voir `https://miro.com` sous "Vers cette application :". Cliquez sur **Continuer**.![jira_server_link_applications.jpg](../../../../../../docs/integrations-apps/atlassian/images/21017528658834_jira_server_link_applications.jpg)*Configurer les détails des applications de liaison*
4. La configuration du lien va être traitée. Lorsque cela se termine, vous verrez votre nouveau lien dans la zone "Liens d'application" de Jira Server. ![jira_server_application_links_created.png](../../../../../../docs/integrations-apps/atlassian/images/21017515685522_jira_server_application_links_created.png)*Votre application configurée dans Jira Server*
5. Ensuite, vous devrez configurer les détails de votre application. Cliquez sur l’icône du crayon pour votre application afin de modifier les détails de l’application.
6. Dans la boîte de dialogue Configurer, cliquez sur l'option **Authentification entrante**. Renseignez la **clé du consommateur, le nom du consommateur, la clé publique** et éventuellement une description.
   - Pour l'intégration au niveau de l'équipe, cette information est disponible dans [**Paramètres de l'équipe**](https://help.miro.com/hc/articles/360021841280) > **Applications et intégrations** > **Cartes Jira**.
   - Pour une intégration au niveau de l'organisation, cette information est disponible sur [**Paramètres de l'entreprise**](https://help.miro.com/hc/articles/360021841280-I-am-a-new-Miro-Admin-Where-to-start) > **Applications** > **Gérer les applications** > **Cartes Jira** > **Paramètres**.
     ![jira_server_config_oauth.png](../../../../../../docs/integrations-apps/atlassian/images/21017528687506_jira_server_config_oauth.png)*Configurer les détails d'authentification entrants dans Jira Server*
     ![jira_webhooks_jira_server_config.png](../../../../../../docs/integrations-apps/atlassian/images/21017515686418_jira_webhooks_jira_server_config.png)*Détails du lien application Jira dans Miro*
7. Faites défiler jusqu'à la fin des options d'authentification entrante et cliquez sur **Enregistrer**. Votre statut de vérification devrait maintenant être confirmé, et ce serveur Jira peut désormais être utilisé dans Miro avec des cartes Jira. Assurez-vous de choisir "Jira Server" et "OAuth 1.0" du côté Miro.![jira_server_welcome_to_jira.png](../../../../../../docs/integrations-apps/atlassian/images/21017515690258_jira_server_welcome_to_jira.png)

### Autorisation de l’utilisateur

Une fois l'intégration connectée, chacun de vos utilisateurs finaux doit connecter son profil Jira personnel pour établir les autorisations appropriées - cela garantit que l'accès de chaque utilisateur du côté Miro est *exactement le même que du côté de votre instance Jira*. Lorsque les utilisateurs finaux essaient d’importer ou de modifier une carte Jira pour la première fois, il leur sera demandé de se connecter à Jira à l’aide de leurs identifiants individuels.

Une fois cela fait, les utilisateurs peuvent ajouter des tâches sous forme de cartes sur le tableau blanc. Toute modification apportée dans Jira est répercutée dans les cartes Jira sur le tableau.

:::note
Si un utilisateur n'a pas d'identifiants Jira et qu'il a accès au tableau sur lequel la carte a été ajoutée, il verra le titre de la carte, le type de ticket, la priorité, l'assigné et tous les attributs configurés pour s'afficher sur la carte Jira. Cependant, ils ne pourront pas développer la carte pour voir les autres attributs et la modifier à moins d’en avoir l’autorisation. Si l'utilisateur ne se connecte pas avec ses identifiants Jira, il ne verra pas l'avatar de l'assigné et l'aspect général de la carte sera différent.
:::

### Utilisation d'une instance Jira pour plusieurs équipes Miro

Vous pouvez installer des cartes au niveau de l’équipe ou au niveau de l'organisation. Si vous avez plusieurs équipes, vous pouvez tirer parti des paramètres au niveau de l'organisation pour éviter de répéter la procédure de configuration pour chaque équipe. Le lien d'application existant est utilisé pour toutes les équipes.

Une fois que vous connectez votre équipe ou organisation à une instance Jira, un nouveau WebHook est créé dans vos WebHooks Jira pour cette équipe ou organisation Miro. Créer un WebHook établit un canal pour les demandes de mise à jour.

Si vous spécifiez des paramètres au niveau de l'organisation, les équipes déjà connectées conservent leurs paramètres actuels. Cependant, ils peuvent passer aux paramètres du niveau organisationnel à tout moment.

De plus, si nécessaire, les équipes peuvent contourner les paramètres au niveau de l'organisation afin de se connecter à une instance Jira différente.

Si vous êtes un client Enterprise qui souhaite migrer plusieurs connexions au niveau de l'équipe vers la connexion par défaut au niveau de l'organisation, contactez l'équipe chargée de votre compte.

:::warning
Si vous voulez connecter plusieurs équipes séparément, nous vous recommandons de donner à chaque webhook un nom unique. Allez sur votre page Jira WebHooks et modifiez chaque webhook nouvellement créé.
:::

La connexion de plusieurs instances Jira à une seule équipe Miro n’est pas prise en charge.

## Désactiver le plugin

Pour l'intégration au niveau de l'équipe, allez dans **Paramètres de l’équipe** > **Applications et intégrations** > **Cartes Jira**. Puis sélectionnez **Supprimer pour l’équipe**.

Pour une intégration au niveau de l'organisation, afin de restreindre l'utilisation de l'application Jira, allez dans **Paramètres de l'entreprise** > **Applications** > **Gérer les applications** > **Cartes Jira**. Ensuite, déplacez le commutateur en position d'arrêt.

:::warning
Si vous désactivez Jira pour l'organisation, alors les utilisateurs de toutes les équipes Enterprise ne pourront pas utiliser les cartes Jira. Pour en savoir plus sur la gestion et la restriction des applications, consultez [Gestion des applications](https://help.miro.com/hc/articles/4404659741458).
:::

**Plus d'informations :** Voir [Comment utiliser les cartes Jira](https://help.miro.com/hc/articles/360017572434).
