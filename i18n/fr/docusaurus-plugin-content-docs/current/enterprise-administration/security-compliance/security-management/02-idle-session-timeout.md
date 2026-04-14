---
title: Délai d’inactivité de la session
article_id: 360017571454
translation_id: 360017571454
locale: fr
sidebar_position: 2
created_at: '2019-02-11T10:09:05Z'
updated_at: '2025-02-06T08:46:57Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible pour: le forfait Enterprise Rôle requis: admin d’entreprise'
---

Le délai d’inactivité de la session vous permet de fixer une **limite** de temps à l’inactivité des utilisateurs finaux. Le paramètre affecte l’ensemble des membres et des [invités](../../../using-miro/sharing-boards/07-collaboration-with-guests.md). Si la session utilisateur atteint sa limite et expire, l’utilisateur sera automatiquement déconnecté de son profil Miro et il devra à nouveau autoriser pour accéder aux données Enterprise.

:::warning
Faites preuve de prudence lorsque vous définissez des limites de temps d’inactivité. Des délais d’inactivité hautement sécurisés qui sont trop courts entraineront une déconnexion constante des utilisateurs de leurs tableaux. Envisagez une approche équilibrée et sécurisée des délais de session et n’oubliez pas de les communiquer clairement à vos utilisateurs.
:::

### Comment activer le délai d’attente de la session inactive ?

1. Allez dans Paramètres de **l'entreprise** > **Sécurité** > **Authentification** > **Délai de session inactive**
2. Activez la **déconnexion automatique des utilisateurs inactifs** et définissez la limite de temps de **.

   ![](../../../../../../../docs/enterprise-administration/security-compliance/security-management/images/23921804858002_idle-session-timeout.png)
*altidle-session-timeout.pngLa fonction Délai d’inactivité de la session est activée***

L’activation de la fonctionnalité de temporisation de la session inactive pour la première fois remplit la session par défaut d’une durée d’un jour. L’admin peut personnaliser la durée et saisir une valeur entière personnalisée allant de 1 à 9999 et sélectionner les unités : minutes, heures ou jours. La durée minimale autorisée est de 1 heure et la durée maximale autorisée est de 14 jours. Nous vous recommandons de fixer une durée d’au moins 8 heures.

Pour la fonction de temporisation de la session inactive, nous définissons l’inactivité comme l’absence de l’une des actions suivantes, où que ce soit dans l’application pendant la durée définie :

- Mouvement de la souris (ou mouvement sur l’écran tactile)
- Clics avec la souris (ou appuis sur l’écran tactile)
- Pression de touches sur le clavier

Un message d’avertissement sera affiché aux utilisateurs plusieurs minutes avant la déconnexion. Les utilisateurs peuvent simplement déplacer leur souris ou appuyer sur n’importe quelle touche de leur clavier pour rester connectés.

:::note
La valeur par défaut du délai d’attente de la session inactive est de 1 jour. Les réglages peuvent aller de 1 heure à 14 jours.
:::

:::note
Idle Session Timeout fonctionne partout (accès à l’activité de l’utilisateur sur différents appareils, intégrations, etc.)
:::

:::note
Si un utilisateur est un visiteur sur un tableau public stocké dans un forfait Enterprise, mais qu’il ne fait pas partie du forfait Enterprise ayant activé le délai d’inactivité de session, il ne sera pas affecté par le délai.
:::

:::note
Siun utilisateur appartient à plusieurs organisations qui ont mis en place des intervalles de temporisation de session inactive différents, c’est la durée la plus courte qui prévaut. Par exemple, si un utilisateur appartient à une organisation dont le délai de session inactive est de 6 heures et à une organisation dont le délai de session inactive est de 30 minutes, il sera exclu de toutes les sessions actives au bout de 30 minutes.
:::
