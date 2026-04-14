---
title: "Contr\xF4le de domaine"
article_id: 360034831793
translation_id: 7316242924690
locale: fr
sidebar_position: 1
created_at: '2022-08-25T09:51:17Z'
updated_at: '2026-03-27T15:52:01Z'
draft: false
outdated: true
user_segment_id: null
user_segment: Everyone
availability:
  plans: business, enterprise
  roles: company_admin, system_admin
---

> **Disponible sur :** Business, Enterprise
> **Rôle requis :** admin d’entreprise, admin système

Le contrôle de domaine permet aux admins d’entreprise de gérer l’accès des utilisateurs au sein de leur abonnement. En utilisant le contrôle de domaine, les admins peuvent appliquer la conformité de sécurité de l’entreprise et maintenir une supervision des activités des utilisateurs gérés au sein de leurs domaines.

Apprenez comment configurer et gérer le contrôle de domaine au sein de votre organisation.

**Avec le contrôle de domaine, les admins du forfait Enterprise peuvent :**

- Réaliser des audits pour identifier les utilisateurs associés à un domaine géré qui n’est pas inclus dans votre abonnement, et les inviter à rejoindre.
- Empêcher les utilisateurs d’un domaine de créer des abonnements non autorisés.
- Ajouter automatiquement les utilisateurs nouvellement enregistrés à des équipes désignées.
- [Bloquer les utilisateurs désactivés](../../user-management/02-block-deactivated-users.md) pour empêcher leur accès à Miro en utilisant leur adresse e-mail professionnelle.

**Admins du forfait Business :**

- Peuvent utiliser la vérification automatique du domaine pour gérer les domaines. Seuls les nouveaux domaines ajoutés seront automatiquement vérifiés.
- Ne peuvent pas modifier les politiques de contrôle de domaine.
- Ne peuvent pas demander d’audit de domaine.

![domain-policies-business.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21046889202834_domain-policies-business.png)

*Les politiques de domaine peuvent être consultées sous Domaines gérés pour les utilisateurs du plan Business*

Les utilisateurs du plan Business devront changer de forfait pour d’autres fonctionnalités avancées.

:::note
La gestion en masse des domaines n’est pas prise en charge actuellement.
:::

## Domaine principal

Votre domaine principal détermine comment Miro identifie les utilisateurs internes et externes dans votre organisation. Pour savoir comment consulter, modifier ou gérer votre domaine principal, consultez [Gérer votre domaine principal](https://help.miro.com/hc/en-us/articles/34249718672274).

## Configurer le contrôle de domaine

### Étape 1 : Ajouter des domaines

1. Ouvrez votre tableau de bord Miro.
2. Cliquez sur votre photo de profil dans le coin supérieur droit.
3. Sélectionnez **Paramètres** dans le menu déroulant.
4. Dans le volet de gauche, allez à **Sécurité et conformité**, et cliquez sur **Domaines gérés**

   > ✏️ Pour les forfaits Business, **Domaines gérés** se trouve sous **Compte**.
5. Cliquez sur **+ Ajouter un domaine** et saisissez le nom de domaine complet (par ex., votresociété.com).
   ![Managed-domains-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318776338_Managed-domains-settings.png)
*Paramètres de domaine géré*

:::note
Si vous avez activé [**Blocage des utilisateurs désactivés**](../../user-management/02-block-deactivated-users.md), alors tous les utilisateurs désactivés associés à un domaine nouvellement vérifié sont automatiquement bloqués.
:::

### Étape 2 : Vérifier les domaines

1. Après avoir ajouté un domaine, vous recevrez un code de vérification dans vos paramètres de **domaine géré**. Copiez ce code.

   ![Complete-domain-verification.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318779282_Complete-domain-verification.png)
*Copie du code de vérification*
2. Si vous gérez vos entrées DNS, mettez à jour vos paramètres DNS en ajoutant une entrée TXT avec le code de vérification comme sa **Valeur**. (Si quelqu’un d’autre gère vos entrées DNS, transmettez-lui le code de vérification avec les instructions pour mettre à jour les entrées DNS.)
3. Connectez-vous au site de votre fournisseur de domaine (GoDaddy, Amazon, Cloudflare, etc.), et accédez à la section **DNS** **enregistrements**.
4. Créez une nouvelle **entrée TXT** avec les spécifications suivantes :
   **Valeur/Réponse/Description :** *"miro-verification=[INSÉRER LE CODE DE VÉRIFICATION]"*
   **Nom/Hôte/Alias :** Laissez ce champ vide ou tapez @ pour inclure un sous-domaine.
   **Durée de validité (TTL) :** "86400" (peut également être hérité de la configuration par défaut).

   ![Creating-new-TXT-record.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318775314_Creating-new-TXT-record.png)
   *Création d’une nouvelle entrée TXT*

:::note
Vous pouvez mettre à jour l’enregistrement TXT via la console d’administration ou le tableau de bord de l’hébergeur DNS du domaine. Consulter la [liste des fournisseurs DNS](https://support.google.com/a/topic/1409901).
:::

### Étape 3 : Vérifier la vérification du domaine

1. Après avoir mis à jour l’enregistrement DNS, vérifiez immédiatement l’état de la vérification de votre domaine dans vos paramètres de **domaine géré** en cliquant sur **Vérifier la vérification**.
2. Si le domaine n’est pas vérifié immédiatement, Miro vérifiera automatiquement la présence du code de vérification toutes les 2 heures pendant les 30 prochains jours.

### Étape 4 : Notification de l’état de vérification

1. Une fois que votre domaine est vérifié avec succès, vous recevrez une notification par e-mail confirmant l’état de vérification.
2. Veuillez ne pas supprimer l’entrée DNS après vérification, car elle pourrait être nécessaire pour de futures vérifications.
   ![Check-domain-verification.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017348597650_Check-domain-verification.png)
*Vérification du domaine*

## Règles qui s’appliquent lors de la vérification des domaines

- Vous devrez créer un enregistrement TXT distinct pour chaque domaine de premier niveau et chaque sous-domaine que vous utilisez. Suivez les étapes 1 à 4 ci-dessus pour chaque domaine ou sous-domaine que vous souhaitez vérifier.
- Votre domaine doit correspondre exactement.

  > ✏️ Les sous-domaines ne sont pas autorisés.
- Assurez-vous que toutes les zones utilisées dans la configuration du domaine vérifié sont incluses.
- Le nom de domaine pleinement qualifié (FQDN, Fully Qualified Domain Name) doit correspondre à votre adresse de domaine. Par exemple, [www.mycompanydomain.com](http://www.mycompanydomain.com).
- Si vous utilisez à la fois des DNS internes et externes, nous recommandons de vérifier les deux pour assurer un contrôle de domaine complet.

## Gestion des utilisateurs et des accès

### Modifier les paramètres de domaine

Les paramètres de domaine déterminent la façon dont les utilisateurs existants et nouvellement enregistrés dans votre ou vos domaines sont gérés.

1. Une fois un domaine vérifié, cliquez sur les trois points (**...**), puis sélectionnez **Modifier les paramètres de domaine**.
   ![Edit-domain-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318773138_Edit-domain-settings.png)
*Modification des paramètres de domaine*
2. Vous verrez ici des options permettant de gérer les nouveaux utilisateurs de votre domaine :

- **Capture automatique des nouveaux utilisateurs** : Ajoute automatiquement les utilisateurs qui s’inscrivent à Miro avec une adresse e-mail d’un domaine géré à l’abonnement de ce domaine, avec le type de licence par défaut. Vous pouvez également définir les équipes auxquelles les utilisateurs seront ajoutés (obligatoire).
- **Empêcher les utilisateurs de créer leurs propres abonnements** : Interdire aux utilisateurs gérés dans votre ou vos domaines de créer de nouvelles équipes en dehors de votre abonnement. Cependant, ces utilisateurs peuvent toujours être invités dans des équipes de votre ou de vos domaines et collaborer en externe.

  ![Managed-domain-settings.png](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/21017318773778_Managed-domain-settings.png)
*Options pour gérer les nouveaux utilisateurs de votre domaine*

  > ✏️ Si vous activez **Empêcher les utilisateurs de créer leurs propres abonnements**, alors les utilisateurs ne peuvent pas s’enregistrer eux-mêmes, à moins d’être invités, ou si l’auto-capture ou JIT est activé.

### Utilisateurs internes et externes

Lorsqu’un domaine est revendiqué, les détails de l’utilisateur indiquent une classification **Interne** ou **Externe**.

![](../../../../../../../docs/enterprise-administration/security-compliance/domain-control/images/33613933595794_image.png) *Les détails de l’utilisateur montrent si l’utilisateur est externe ou interne à votre domaine vérifié*

Les utilisateurs internes possèdent une adresse e-mail d’un domaine revendiqué par votre compte Enterprise. Par exemple, `user@acme.com` où `acme.com` est l’un de vos domaines vérifiés.

Les utilisateurs externes ont une adresse e-mail en dehors de tout domaine revendiqué par votre compte Enterprise. Par exemple, `user@not-domain.com` où `not-domain.com` n’est pas l’un de vos domaines vérifiés.

:::note
Les détails de l’utilisateur sont visibles dans le profil utilisateur. Dans la console d’admin, les détails de l’utilisateur sont également visibles dans la liste des utilisateurs, où vous pouvez éventuellement filtrer par **Interne** ou **Externe** classification.
:::

La classification interne ou externe est automatique et basée sur le fait que le domaine de l’utilisateur est revendiqué et vérifié par votre compte Enterprise.

## Regroupement des équipes en libre-service vers le forfait Enterprise

En tant qu’admin d’entreprise, vous pouvez rassembler toutes les équipes créées à partir de vos domaines dans votre forfait Enterprise. Cela assure une meilleure sécurité, collaboration et gestion en regroupant toutes les équipes en un seul endroit. De plus, vous pouvez également auditer les domaines pour identifier et consolider les utilisateurs et équipes qui font partie de votre domaine géré mais actuellement en dehors de votre abonnement.

Pour plus d’informations, [consultez la documentation sur la consolidation d’équipe](../../managing-enterprise-teams-and-content/06-self-serve-teams-to-enterprise-plan-consolidation.md).

## Demandes de modification de l’adresse e-mail

Si votre entreprise a revendiqué un domaine, tout utilisateur associé à ce domaine sera dans l’incapacité de changer son adresse e-mail dans Miro sans l’approbation de l’admin d’entreprise. Lorsqu’ils tenteront de modifier leur e-mail, les utilisateurs recevront le message d’erreur suivant : **Vous ne pouvez pas changer votre adresse e-mail vers ou depuis un domaine appartenant à une organisation**. Il est recommandé que les utilisateurs contactent l’admin de leur entreprise, qui elle-même se mettra en relation avec le service d’assistance de Miro pour obtenir de l’aide.

## Foire aux questions

Puis-je utiliser le contrôle de domaine avec un sous-domaine ?

Oui, les sous-domaines sont traités comme des entités distinctes des domaines principaux. Suivez le processus de configuration pour chaque sous-domaine que vous souhaitez vérifier.

Comment utiliser l’authentification unique avec le contrôle de domaine ?

Vous devrez configurer le contrôle de domaine avant d’activer l’[authentification unique](../../security-integrations/single-sign-on-sso/09-single-sign-on-(sso).md).

Que faire si mon nom de domaine change ou si je veux ajouter un sous-domaine ?

Si votre nom de domaine change, supprimez le domaine et redémarrez le processus de vérification avec le nouveau domaine ou les sous-domaines que vous ajoutez.

Où puis-je trouver les enregistrements DNS de mon domaine ?

Pour localiser les enregistrements DNS de votre domaine, vous devrez accéder à la plateforme de votre registrar où vous avez enregistré votre domaine. Si vous ne savez pas qui est votre registrar, vous pouvez trouver cette information en utilisant **who.is** pour rechercher le domaine. Une fois que vous avez identifié votre registrar, connectez-vous à leur site Web et accédez à la section généralement intitulée **Domains** ou **Gestion DNS**. Vous y trouverez les paramètres DNS ou les enregistrements de votre domaine.

Pourquoi ne puis-je pas voir **Domaines gérés** dans les paramètres de **Sécurité et conformité** ?

Si vous ne pouvez pas voir l’option **Domaines gérés**, cela peut être dû à deux raisons :

- Vous n’êtes pas abonné à un forfait Enterprise qui inclut cette fonctionnalité.
- Vous n’avez pas le rôle d’admin d’entreprise requis pour accéder à ce paramètre.

Veuillez vérifier les détails de votre forfait et votre rôle auprès d’un admin d’entreprise pour obtenir plus d’assistance.

Puis-je supprimer l’enregistrement TXT de mon domaine une fois qu’il a été vérifié ?

Bien que la suppression de l’enregistrement TXT après vérification n’affecte pas immédiatement le fonctionnement de votre contrôle de domaine, il est fortement recommandé de conserver cet enregistrement. Maintenir l’enregistrement TXT en place est crucial pour d’éventuels processus de re-vérification dans le futur. Supprimer l’enregistrement TXT pourrait compliquer ces processus et nécessiter de refaire les étapes de vérification.
