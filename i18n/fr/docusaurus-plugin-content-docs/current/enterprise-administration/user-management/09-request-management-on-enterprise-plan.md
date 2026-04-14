---
title: Gestion des demandes dans le forfait Enterprise
article_id: 360017237379
translation_id: 360017237379
locale: fr
sidebar_position: 9
created_at: '2020-10-27T12:09:40Z'
updated_at: '2026-02-19T11:00:31Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: access-request-management
availability:
  notes: 'Disponible pour: : le forfait Enterprise Qui peut le faire: admins d’entreprise'
---

Dans Miro, les demandes de licences, d’accès aux équipes et aux organisations, ainsi que l'authentification unique (SSO) sont envoyées par défaut aux admins d’entreprise par e-mail. Grâce à des fonctionnalités avancées de gestion des demandes, les admins d’entreprise peuvent adapter la manière dont ces demandes sont reçues et traitées.

### Type de demande

Les types de demandes se répartissent en quatre catégories :

- Demandes d’adhésion à votre organisation
- Demandes d’adhésion à une équipe
- Demandes de licence
- Demandes liées à des problèmes de SSO

Découvrez les différents scénarios de demande pour le forfait Enterprise.

### Options de gestion des demandes

Les admins d’entreprise disposent de plusieurs options de gestion des demandes, ce qui leur permet de personnaliser les processus en fonction du type de demande :

:::note
Les options pour envoyer un e-mail à tous les admins d’entreprise, ou à des admins d’entreprise spécifiques, incluent les admins d’équipe.
:::

- Envoyer un e-mail à tous les admins d'entreprise
- Envoyer un e-mail à certains admins d'entreprise
- Créer un ticket d'assistance
- Rediriger vers une URL personnalisée

## Configurer la gestion des demandes

:::note
Pour [gérer les demandes de licence directement dans Miro](04-license-requests-on-enterprise-plan.md), sélectionnez soit **Envoyer un e-mail à tous les admins d’entreprise** soit **Envoyer un e-mail à des admins spécifiques**. Vous recevrez toutes les futures demandes de licence dans vos paramètres de demande de licence.
:::

### Envoyer un e-mail à tous les admins d’entreprise

Tous les admins d’entreprise recevront une notification par e-mail lorsqu’un utilisateur fait une demande d’accès.

1. Dans les paramètres de **l’Entreprise**, accédez à **Utilisateurs** > **Demandes d'accès** > **Gestion des demandes**.
2. Cliquez sur le **Type de demande** que vous souhaitez gérer.
3. Une fenêtre contextuelle s’ouvre. Cliquez sur le menu déroulant et sélectionnez **Envoyer un e-mail à tous les admins d’entreprise**.

:::note
Les options pour envoyer un e-mail à tous les admins d’entreprise, ou à des admins d’entreprise spécifiques, incluent les admins d’équipe.
:::

### Envoyer un e-mail à des admins d’entreprise spécifiques

Les admins d’entreprise peuvent spécifier jusqu’à cinq adresses e-mail. Seules les adresses e-mails spécifiées recevront la demande. Elles ne doivent pas nécessairement appartenir à des utilisateurs de Miro.

1. Allez dans **Paramètres de l'entreprise** > **Utilisateurs** > **Demandes d'accès** > **Gestion des demandes**.
2. Cliquez sur le **type de demande** que vous souhaitez gérer.
3. Une fenêtre contextuelle s’affiche. Cliquez sur la liste déroulante et sélectionnez **Envoyer un e-mail à certains admins d'entreprise**.
4. Ajoutez jusqu’à cinq adresses e-mail. Cliquez sur **Ajouter** chaque fois que vous saisissez une adresse e-mail dans le champ e-mail.

:::note
Les options pour envoyer un e-mail à tous les admins d'entreprise, ou à des admins spécifiques de l'entreprise, incluent les admins d'équipe.
:::

### Créer un ticket d’assistance

Créez automatiquement un ticket de service desk chaque fois qu’un utilisateur fait une demande d’accès. Cette fonctionnalité est actuellement prise en charge pour **ServiceNow** et **Jira Service Management**.

ServiceNow Jira Service Management

1. Configurez les paramètres de l’e-mail pour ServiceNow. Créez un élément de catalogue pour Miro dans ServiceNow. Ouvrez ServiceNow, allez dans **System Properties** > **Email Properties** et activez la réception des e-mails entrants

2. [Créez une action d’e-mail entrant](https://docs.servicenow.com/bundle/tokyo-servicenow-platform/page/administer/notification/task/t_CreatingAnInboundEmailAction.html). Dans le champ **From**Dans le champ **De**, sous la ligne **Seuls les e-mails provenant de cet expéditeur déclencheront cette action de réception**, saisissez [notification@miro.com](mailto:notification@miro.com).

3. [Définissez les valeurs des champs à partir du corps de l'e-mail](https://docs.servicenow.com/bundle/rome-servicenow-platform/page/administer/notification/reference/r_SetFieldValsFromTheEmailBody.html) pour configurer des paramètres supplémentaires et mettre en place le processus de conversion d'un e-mail de Miro en ticket ServiceNow. Par exemple, vous pouvez assigner un ticket nouvellement créé à une personne en particulier.

4. Allez dans Miro, ouvrez les paramètres de l'entreprise > **Utilisateurs** >**Demandes d'accès** > **Gestion des demandes**, et sélectionnez **Créer un ticket dans ServiceNow**. Dans le champ e-mail, saisissez votre adresse e-mail ServiceNow.

1. Configurez les paramètres d’e-mail pour Jira Service Management. Depuis votre projet de service, sélectionnez **Paramètres du projet** > **Demandes par e-mail**. [Choisissez votre fournisseur de service e-mail et suivez les prompts pour lier Miro](https://support.atlassian.com/jira-service-management-cloud/docs/receive-requests-from-an-email-address/).

2. Rendez-vous sur Miro, ouvrez les **Paramètres de l’entreprise** > **Gestion des utilisateurs** > **Demandes d'accès** >
**Gestion des demandes**, et sélectionnez **Créer un ticket dans Jira Service Management**. Dans le champ e-mail, saisissez votre adresse e-mail Jira Service Management.

### Rediriger vers une URL personnalisée

Le demandeur sera redirigé vers l’URL de votre choix pour les étapes suivantes.

1. Dans les **paramètres de l'entreprise** allez à **Utilisateurs** > **Demandes d'accès** > **Gestion des demandes**.
2. Cliquez sur le **type de demande**que vous souhaitez gérer.
3. Une fenêtre contextuelle s'ouvre. Cliquez sur la liste déroulante et sélectionnez **Rediriger vers une URL personnalisée**.
4. Saisissez le lien de redirection dans le champ **URL personnalisée**.

## Scénarios de demande

Les scénarios ci-dessous décrivent comment les différentes demandes sont déclenchées dans Miro. Examinez les scénarios pour décider de la manière dont vous souhaitez gérer chaque type de demande.

|  |  |
| --- | --- |
| **Demandes d'ajout à votre organisation** | - Lorsqu'un nouvel utilisateur demande à rejoindre une équipe souscrite à un abonnement géré par l'entreprise avec [contrôle de domaine](../canvas-25-admin-features/domain-control/01-domain-control.md) (sauf si le contrôle de domaine est configuré pour capturer de nouveaux utilisateurs). |
| **Demandes de licences** | - Lorsqu'un [utilisateur Free Restreint](../enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md) demande une licence Standard ou Complète (ancienne version). - Lorsqu’un membre demande une licence Standard ou Complet (ancienne version) pour un utilisateur disposant d’une licence gratuite restreinte, sauf si les membres sont autorisés à inviter de nouveaux utilisateurs à l'abonnement dans les [paramètres d’invitation](03-invitation-settings-on-enterprise-plan.md). - Lorsqu’un utilisateur Standard ou Complet (ancienne version) demande une licence Avancé. - Lorsqu’un membre tente d’inviter ou de donner un accès de modification à un utilisateur disposant d’une licence gratuite restreinte. |
| **Demandes d'ajout à une équipe** | - Lorsqu'un utilisateur non-admin tente de partager un tableau avec un utilisateur qui *n'est pas* membre de l'équipe, les invitations d'invités sont désactivées dans les [paramètres d'invitation](03-invitation-settings-on-enterprise-plan.md), et seuls les admins peuvent inviter de nouveaux membres dans l'équipe. - Lorsqu'un membre qui n'est pas autorisé à inviter de nouveaux membres tente de conférer un rôle de [propriétaire ou de copropriétaire](../../using-miro/sharing-boards/06-co-owners-of-boards-and-spaces.md) sur un tableau particulier à un utilisateur qui n'est pas membre de l'équipe. - Lorsqu'un utilisateur Enterprise demande à rejoindre une équipe [découvrable par les utilisateurs de leur organisation](../managing-enterprise-teams-and-content/11-manage-team-privacy-and-discovery-on-enterprise-plan.md). - Lorsqu’un [invité](../../using-miro/sharing-boards/07-collaboration-with-guests.md) convié sur les tableaux spécifiques d’une équipe demande à rejoindre cette équipe |
| **Demandes liées à des problèmes de SSO** | - Lorsqu’un utilisateur n’a pas obtenu l’accès à Miro dans l’IdP et qu’il rencontre des problèmes pour se connecter via l’authentification unique. |

## Foire aux questions

**Pourquoi est-ce que je continue à recevoir des e-mails alors que j’ai configuré mes paramètres pour créer des tickets ?**

Si les admins d’équipe sont autorisés à inviter de nouveaux utilisateurs dans une [paramètres d’invitation](03-invitation-settings-on-enterprise-plan.md), ils recevront les demandes d’invitation liées à cette équipe par e-mail, même si les paramètres de gestion des demandes sont définis différemment. Les admins d’entreprise qui sont aussi admin d’équipe recevront également ces e-mails.

**Comment les admins d’équipe peuvent-ils savoir s’il y a une demande pour rejoindre leur équipe ?**

S’ils sont autorisés à inviter des utilisateurs dans leurs équipes, les admins d’équipe recevront un e-mail concernant les demandes, quels que soient les paramètres de gestion des demandes.
