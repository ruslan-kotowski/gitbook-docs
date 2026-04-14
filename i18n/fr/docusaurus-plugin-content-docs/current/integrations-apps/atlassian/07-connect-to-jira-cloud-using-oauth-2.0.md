---
title: Connectez-vous à Jira Cloud en utilisant OAuth 2.0
article_id: 8588617184402
translation_id: 12983105657874
locale: fr
sidebar_position: 7
created_at: '2023-08-09T14:49:52Z'
updated_at: '2025-10-21T12:18:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: jira-cards
availability:
  notes: 'Disponible pour: Jira Cloud, y compris LDAP-protégé Forfaits: Starter, Business,
    Enterprise, Education Configuration par: (Enterprise) admin d’entreprise, ou (Tous
    les autres forfaits) admin d’équipe, avec privilèges d’admin Jira'
---

:::warning
Si des problèmes techniques apparaissent, veuillez vous référer à notre article sur [les problèmes éventuels et sur comment les résoudre](https://help.miro.com/hc/articles/360017572654).
:::

:::tip
En savoir plus sur les cartes Jira dans les articles [FAQ sur les cartes Jira](https://help.miro.com/hc/articles/360013463739)
:::

## Connexion entre Jira et Miro

### Installer l’application

1. Pour activer l’intégration, sur votre [tableau de bord](https://help.miro.com/hc/articles/360017571294-What-is-on-your-dashboard) dans le coin supérieur droit, cliquez sur votre avatar > **Applications et intégrations**:![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)
   *Gérer vos applications*
2. Saisissez « cartes Jira » dans le champ **Recherche**, puis cliquez sur le bouton bleu **Associer** en bas à droite du menu déroulant.
3. Vous verrez une fenêtre vous permettant d'**Ajouter « Cartes Jira »**. Ici, vous devez valider l'installation ou sélectionner l'équipe où vous souhaitez installer l'intégration (si vous êtes membre de plusieurs équipes). Cliquez sur **Ajouter** l'intégration. En haut du tableau de bord, vous verrez le message de confirmation que l'**Application a été installée :**
   ![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)
   *Le message de confirmation*

### Associer votre profil Jira

1. Cliquez à nouveau sur votre avatar dans le tableau de bord et allez dans **Paramètres > Équipes >** *Votre nom d'équipe* **> Applications & Intégrations > Cartes Jira** et cliquez sur **Connecter :
   ![mceclip2.png](../../../../../../docs/integrations-apps/atlassian/images/21017004818066_mceclip2.png)***Les paramètres de l'intégration*
2. Vous arriverez sur la page Jira pour autoriser l'association. Connectez-vous à Jira et cliquez sur **Accepter**.

### Associer des instances Jira à votre équipe Miro

Avec OAuth 2.0, vous pouvez désormais associer plusieurs de vos instances Jira à la même équipe et aux mêmes tableaux. Après avoir autorisé l’application dans Paramètres, vous verrez l’option **Associer une autre instance.**

1. Lancez le sélecteur de cartes Jira depuis la barre d’outils de création (il vous faudra peut-être ajouter l’application à l’aide du bouton **Plus d’applications +**).
2. Dans l’outil Sélecteur, cliquez sur **Paramètres**.
3. Vous accéderez à la rubrique **Applications et intégrations** de vos paramètres. Cherchez l’option **Associer une autre instance** et sélectionnez les instances Jira supplémentaires que vous souhaitez associer.![mceclip0.png](../../../../../../docs/integrations-apps/atlassian/images/21017417672210_mceclip0.png)*Paramètres des cartes Jira dans un compte Miro*

Les admins d’équipe peuvent également voir toutes les instances associées par les membres de l’équipe :

![mceclip1.png](../../../../../../docs/integrations-apps/atlassian/images/21017417673362_mceclip1.png)

:::warning
Notez que chaque utilisateur final devra s’authentifier à partir des tableaux Miro sur chaque instance Jira associée s’il tente de travailler avec les cartes de l’instance.
:::

> ✍️ Notez qu’une seule instance peut être active à la fois afin que les utilisateurs puissent en extraire des cartes. Il est toujours possible de travailler sur les cartes existantes provenant d’instances inactives sur les tableaux Miro.

### Configurer des mises à jour en temps réel depuis Jira

Pour bénéficier pleinement de notre synchronisation bidirectionnelle en temps réel, vous devez configurer les webhooks pour les instances Jira que vous ajoutez. Cela garantira que toutes les mises à jour effectuées dans Jira soient propagées en temps réel dans Miro.

1. Lancez le sélecteur de cartes Jira depuis la barre d’outils de création (il vous faudra peut-être ajouter l’application à l’aide du bouton **Plus d’applications +**).
2. Dans l’outil Sélecteur, cliquez sur **Paramètres**.
3. Vous accéderez à la rubrique **Applications et intégrations** de vos paramètres.
4. Dans la section **Instances connectées**, vous devriez voir une liste des instances que vous avez ajoutées précédemment.
5. À côté de chaque instance, il y a un bouton pour **Ajouter un webhook.** En cliquant dessus, vous configurerez les mises à jour en temps réel de Jira à Miro pour cette instance.
6. Si vous souhaitez supprimer des webhooks de cette instance à l’avenir, vous pouvez suivre les étapes ci-dessus et cliquer sur le bouton **Supprimer le webhook** qui se trouve à côté des instances connectées pour lesquelles vous avez ajouté un webhook.

:::note
Notez que vous devez être admin sur Miro *et* Jira pour pouvoir ajouter des webhooks à vos instances.
:::

Après cela, vous avez terminé ! Vous pouvez désormais ajouter vos tâches Jira sous forme de cartes sur le tableau blanc. Toute modification apportée dans Jira est répercutée dans les cartes Jira sur le tableau et vice versa.

## Désinstallation du plugin

Rendez-vous dans vos **Paramètres de l’équipe > Applications & Intégrations > Cartes Jira** et cliquez sur **Désinstaller pour l'équipe.**

:::tip
N'oubliez pas de consulter l'article principal sur [comment utiliser les cartes Jira](https://help.miro.com/hc/articles/360017572434) !
:::
