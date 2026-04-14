---
title: "Application Miro pour Zoom (Guide de l\u2019administrateur)"
article_id: 360022039379
translation_id: 360022039379
locale: fr
sidebar_position: 1
created_at: '2021-05-28T04:43:09Z'
updated_at: '2025-02-26T11:51:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: zoom
---

L’application Miro pour Zoom permet aux équipes de créer une salle de réunion numérique tout-en-un et de collaborer efficacement pendant les réunions et les ateliers en se servant de Miro depuis Zoom.  L’application offre les capacités de collaboration de Miro depuis Zoom et facilite l’intégration des utilisateurs invités. Pour les personnes arrivant tout juste sur Miro, nous proposons un tableau blanc avec un accès sans inscription.

Ce guide peut être utilisé par les admins de Zoom et Miro pour activer l’expérience pour leurs utilisateurs.

:::note
Consultez le [Guide utilisateur pour l’application Miro pour Zoom](02-miro-app-for-zoom-user-guide.md).
:::

> **Disponible pour :** tous les plans Miro, tous les plans Zoom
> *Pour les plans Zoom Business et Enterprise, l'admin peut avoir besoin de pré-approuver l'application Miro.
> **Disponible sur**: version de bureau

## Comment activer l’expérience de l’application dans Zoom

### Activer la découverte des applications

1. Connectez-vous au portail Web de Zoom en tant qu’administrateur avec le droit de modifier les paramètres compte.
2. Dans le panneau de navigation, cliquez sur **Account Management** (Gestion de compte) puis sur **Account Settings** (Paramètres du compte).
3. Cliquez sur l’onglet **Zoom Apps** (Applications Zoom).
4. Vérifiez que le bouton **Zoom Apps Quick Launch Button** (Lancement rapide des applications Zoom) est activé. Cela permet aux utilisateurs de votre compte de voir le bouton Zoom Applications ![](../../../../../../docs/integrations-apps/zoom/images/21017682787474_mceclip0.png) mceclip0 alt.pngalt sur le client de bureau.
5. Si le paramètre est désactivé, cliquez sur le bouton pour l'activer. Si une boîte de dialogue de vérification s'affiche, cliquez sur **Turn On** pour vérifier la modification.

De plus, Zoom propose de la documentation supplémentaire expliquant comment activer les applications Zoom uniquement pour des groupes ou des utilisateurs spécifiques. Pour plus d’informations, consultez le centre Centre d’assistance Zoomici/span>[.](https://support.zoom.us/hc/articles/360061555152)

Zoom_apps_quick_launch.jpg
Activation du bouton de lancement rapide des applications Zoom

Cela activera les applications Zoom dans la barre supérieure du client principal de Zoom et dans la barre inférieure des clients de réunion pour les utilisateurs de votre compte.

### Comment pré-approuver l’application dans Zoom

Si vous êtes un admin Zoom pour un plan Zoom Business ou Enterprise, vous devrez peut-être pré-approuver l’application Miro [ici](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) pour ouvrir l’accès aux utilisateurs.

![pré-approbation de l'application Miro.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653155474_pre-approve%20Miro%20app.jpg)*Pré-approbation de l'application Miro*

### Sélectionner les utilisateurs du compte qui peuvent installer l’application

En plus de pré-approuver l’application Miro vous pouvez sélectionner quels utilisateurs ou quels groupes sont en mesure de l’installer.

allow_users_to_install_the_app.jpg
/span>Sélectionner les utilisateurs et les groupes qui peuvent installer l’application Miro

Une fois que vous aurez approuvé l’application Miro et que vous l’aurez installée sur votre compte d’entreprise, les utilisateurs pourront y accéder et l’installer à partir du client Zoom.

Consultez[la documentation de Zoom](https://support.zoom.us/hc/articles/360061555152) pour plus d’informations.

## Comment activer l’expérience de l’application dans Miro

> **Installation par :** Administrateurs d'entreprise sur le plan Enterprise

Si vous êtes sur un [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md) et que vous avez limité l’installation aux applications approuvées, assurez-vous d’inclure l’application Miro pour Zoom dans votre liste d’applications approuvées dans **Company settings (paramètres de l’entreprise) > Apps (Applications) > Manage apps (Gestion des apps)**.  Vous pouvez le faire en collant le clientID 3074457354625507111 dans la recherche et en autorisant l’application pour installation.

approve_Zoom_on_Enterprise_plan.jpg
Applications approuvées dans les paramètres de l’entreprise

## Comment les utilisateurs peuvent installer l’application

Les utilisateurs peuvent trouver l’application Miro pour Zoom sur le [Marketplace Zoom](https://marketplace.zoom.us/apps/HVFvOpFKRIi6b6ikMKkrWA) ou sur le Marketplace Miro .

La première étape du processus d’installation est d’autoriser l’application Miro pour Zoom.

install_Miro_app_for_Zoom.jpg
/span>Permettre à Miro d’accéder à votre compte Zoom

Une fois l'autorisation obtenue, l'application redirige les utilisateurs vers leur application de bureau Zoom et affiche l'application Miro nouvellement installée. **Notez qu'ils devront être connectés à leur compte Zoom pour ajouter l'application.**.

Les utilisateurs Miro devront **se connecter** pour voir leurs tableaux. Cela les redirigera vers leur navigateur de système où nous leur demandons de se connecter à Miro ou d’autoriser directement l’application dans Miro. Ils peuvent choisir d’installer l’application pour n’importe quelle équipe à laquelle ils ont accès.

install_Zoom_for_a_Miro_team.jpg
Installez l’application pour l’une de vos équipes Miro./span>

Les utilisateurs seront alors redirigés vers l’application de bureau Zoom où ils verront leur tableau de bord Miro listant l’ensemble de leurs équipes et de leurs tableaux existants.

![Miro_dashboard_in_Zoom.jpg](../../../../../../docs/integrations-apps/zoom/images/21017653159442_Miro%20dashboard%20in%20Zoom.jpg)*Les utilisateurs pourront sélectionner un tableau dans leur tableau de bord et l'ouvrir dans Zoom.*

## Comprendre les paramètres d’accès de partage du tableau

Les utilisateurs peuvent définir les autorisations de partage appropriées d’un tableau depuis une réunion Zoom. Ils ont le choix entre quatre options : **N'importe qui dans Zoom peut modifier/commenter/visualiser** ou **Privé** (ce qui signifie que les paramètres de partage seront les mêmes que ceux définis du côté de Miro).

board_embed_sharing_settings.jpg

*Configuration des paramètres d’accès pour votre tableau*

Les options des paramètres d’accès suivront les contrôles d’accès à l’échelle de l’organisation.  Si vous avez limité le partage de liens publics pour les intégrations de tableau sur le [plan Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md), cette option ne sera pas disponible pour les utilisateurs. En savoir plus : Gestion de la politique de partage de l’entreprise pour les intégrations embarquées[.](../../enterprise-administration/managing-apps-on-enterprise-plan/05-how-to-allow-or-restrict-embedding-miro-boards-in-supported-apps.md)

publi_editing_is_turned_off.jpg
/span>L’édition publique est désactivée par l’admin d’entreprise

## Foire aux questions

1. *À quelles données l'application Miro pour Zoom accède-t-elle ?*
   - L'application Miro pour Zoom demande des informations sur le profil de l'utilisateur pour associer un tableau à un utilisateur donné. Notre application n’a **pas** accès aux contenus de la réunion, tels que les fichiers vidéo, audio, chat et/ou les fichiers de réunion et n’apparaît donc pas dans Zoom’s Active Apps Notifier. (Notificateur d’applications actives de Zoom).
2. *L'application peut-elle être installée sur des tablettes ou des applications mobiles ?*
   - Non, l'application Miro pour Zoom n'est disponible que sur le bureau.
3. *Pour quel système d'exploitation Zoom Apps fonctionne-t-il ?*
   - Mac OS et Windows.
4. *Quelle version de Zoom est nécessaire pour utiliser les applications Zoom ?*
   Version : 5.7.3.
