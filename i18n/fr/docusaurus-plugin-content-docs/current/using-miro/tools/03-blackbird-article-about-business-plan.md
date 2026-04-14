---
title: Article de test Blackbird sur SCIM
article_id: 25902000474898
translation_id: 25902000474898
locale: fr
sidebar_position: 3
created_at: '2025-04-08T15:00:21Z'
updated_at: '2025-05-07T11:29:05Z'
draft: false
outdated: false
user_segment_id: 360000855373
user_segment: Agents and admins
backstage_link:
  entity_kind: capability
  entity_id: dependencies
---

!!!Article de test!!!

Le système de gestion des identités inter-domaines (SCIM) vous permet d'automatiser la gestion des utilisateurs et le provisionnement entre Miro et votre fournisseur d'identité (IdP).

> **Disponible pour :**[Offre Enterprise](../../plans-billing/miro-plans/04-enterprise-plan.md)
> **Configuré par :** les admins d'entreprise

## Important à savoir

- **Le SSO basé sur SAML doit être correctement configuré et fonctionnel dans votre forfait Enterprise avant de commencer à configurer le provisionnement automatisé.**
  Consultez [le guide](../../enterprise-administration/security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) pour configurer le SSO SAML.
- **La synchronisation des groupes avec les équipes Miro est facultative.**
  Vous pouvez éventuellement synchroniser vos groupes IdP avec les équipes dans Miro. Cependant, pour éviter les problèmes où un groupe IdP est supprimé involontairement ou temporairement, ce qui entraîne la désactivation de tous les utilisateurs de ce groupe dans Miro et déclenche la réaffectation des tableaux et Espaces, ne synchronisez pas les groupes IdP avec les équipes Miro. Les équipes peuvent être créées et gérées à l'aide de l'[API Teams](https://developers.miro.com/reference/enterprise-create-team). Pour plus d’informations sur la façon dont l’API SCIM vous permet de gérer les groupes, consultez [Miro Developers](https://developers.miro.com/docs/groups).
- **Les changements d'adresse e-mail dans SCIM incluent les règles de validation suivantes :**
  - **Vérification des utilisateurs gérés :** Si le domaine actuel de l'utilisateur n'est pas revendiqué par l'organisation initiant la demande SCIM, la mise à jour de l'e-mail est bloquée et génère une erreur 400.
  - **Vérification du domaine de l'e-mail cible :** Si le domaine de l'email cible est revendiqué par une organisation autre que celle qui initie la demande SCIM, la mise à jour de l'email est bloquée et un code d'erreur 400 est généré. Si le domaine de l'e-mail cible est revendiqué par l'organisation initiant la requête SCIM, la mise à jour de l'e-mail est autorisée sans nécessiter de confirmation de l'e-mail. Les journaux d’audit enregistrent la mise à jour dans chaque organisation où l'utilisateur est membre.
  - **Contrôle de domaine et SSO :** Les mises à jour par e-mail sont autorisées en fonction de la vérification du domaine via le contrôle de domaine (IDC) ou l'authentification unique (SSO). Si le domaine de l'e-mail cible est vérifié via CD ou SSO par l'organisation initiatrice, la mise à jour peut se poursuivre.
    ![scim-diagram-2.png](images/26547048888082_scim-diagram-2.png)
    *Diagramme du flux de validation du changement d'e-mail SCIM*

### Les règles sur lesquelles se fonde le SCIM de Miro

- Les modifications synchronisées par le SCIM sont principalement appliquées aux utilisateurs nouvellement affectés. Le statut de ceux qui sont déjà sous votre abonnement sera complété mais ne sera peut-être pas écrasé dans la mesure où les changements sont appliqués au niveau du groupe/de l’équipe. Par exemple :
  a) si un utilisateur est membre de l’équipe 1 du côté de Miro et que votre IDP envoie une mise à jour pour l’ajouter à l’équipe 2, son statut dans l’équipe 1 n’est pas affecté.
  b) si votre IDP envoie une mise à jour contenant des modifications à User1, les autres membres de l’équipe ne sont pas affectés. Comme mentionné dans **Fonctionnalités prises en charge** > **Sync et push groups** pour écraser le statut de l'équipe et resynchroniser tous les utilisateurs en une fois, essayez et initiez un nouveau push.
- Tous les utilisateurs provisionnés sous SCIM se voient attribuer la *licence par défaut* de votre abonnement.
  a) Pour les abonnements Enterprise sans programme de licences flexibles : une licence complète. Si votre abonnement n’a plus de licences, les utilisateurs commencent à être approvisionnés sous [licence gratuite restreinte](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/04-free-restricted-license.md).
  b) Pour les abonnements Enterprise avec le [>programme de licences flexibles](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/03-flexible-licensing-program-flp.md) activé : Licence gratuite ou gratuite restreinte en fonction de la [licence d’abonnement par défaut](../../enterprise-administration/enterprise-subscription-management/enterprise-licensing/05-license-management-on-the-flexible-licensing-program-flp.md).
  *- Si vous avez besoin que certains utilisateurs soient provisionnés sous une licence différente de celle par défaut :*
  *comme indiqué ci-dessus, tous les utilisateurs sont dotés de la licence par défaut. Cependant, vous pouvez immédiatement mettre à jour tout ou partie d’entre eux en utilisant l’attribut **UserType** avec une valeur Full. Les utilisateurs mis à jour avec l’attribut seront mis à niveau vers la licence complète sans interruption de service de la part de l’utilisateur.*
- Tous les utilisateurs provisionnés sous SCIM sont également concernés par la fonctionnalité [Contrôle du domaine](../../enterprise-administration/canvas-25-admin-features/domain-control/01-domain-control.md). Cela signifie que si un utilisateur est membre d'un seul groupe de sécurité dans votre fournisseur d'identité mais que vos paramètres de contrôle de domaine définissent 3 équipes comme désignées, l'utilisateur sera également ajouté à ces 3 équipes.
- Pour protéger le service, Miro limite le nombre d’appels API disponibles toutes les 30 secondes :

  | Type de demande | Niveau limite |
  | --- | --- |
  | GET scim/users    GET scim/users/\{userId\} | Niveau de limite de premier plan 1 |
  | POST scim/users/\{userId\}    PUT scim/users/\{userId\}    PATCH scim/users/\{userId\}    DELETE scim/users/\{userId\} | Niveau de limite de troisième plan 3 |
  | GET scim/Groups    PATCH scim/Groups/\{groupId\} | Niveau de limite de quatrième plan 4 |
  | GET scim/Groups/\{groupId\} | Niveau de limite de troisième plan 4 |

  Pour plus de détails sur les niveaux de limite, veuillez consulter [**ici.**](https://developers.miro.com/reference#ratelimiting)Si le nombre de requêtes dépasse la limite, Miro renverra le message standard **429 Trop de requêtes**.

## Fonctionnalités prises en charge

Le schéma détaillé du SCIM de Miro se trouve [**ici**](https://developers.miro.com/docs/scim).

Miro prend en charge les fonctionnalités d’approvisionnement suivantes :

- **Créer de nouveaux utilisateurs**
  Les nouveaux utilisateurs attribués à l’application Miro dans l’IdP seront créés dans votre abonnement Miro Enterprise en tant que membres Enterprise.</span> Les utilisateurs ajoutés à un groupe d’utilisateurs synchronisé avec une équipe Miro portant le même nom seront ajoutés à l’équipe en tant que membres de l’équipe.
- **Pousser les mises à jour du profil utilisateur**
  Pour les attributs et les modifications pris en charge, voir ci-dessous
- **Synchroniser et pousser des groupes**
  Synchronisez vos groupes IdP et leurs membres avec les équipes de votre abonnement Miro Enterprise pour gérer automatiquement l'adhésion des utilisateurs.</span> La synchronisation continue enverra des mises à jour spécifiques concernant les utilisateurs de votre groupe à l'équipe Miro synchronisée, tandis qu'une poussée écrasera l'état de l'équipe en considérant le groupe comme la source de vérité (s'il y a eu des changements manuels par vos admins d'entreprise du côté de Miro)
- **Dissocier les noms des groupes/équipes**
  Miro synchronise les groupes et les équipes par leur nom, ils doivent donc porter le même nom exact. Cependant, après la création de la synchronisation initiale, vous pourrez attribuer à l'un ou aux deux des noms qui vous conviennent. Vous pouvez voir l'exemple du découplage [ici](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)
- **Supprimer les utilisateurs d’un groupe/d’une équipe (pas de l’abonnement Enterprise, voir ci-dessous)**
  La suppression d'un utilisateur d'un groupe entraînera sa suppression de l'équipe Miro synchronisée (au cours du prochain Push de groupe)
- **Désactiver les utilisateurs**
  La désactivation/suppression d’un utilisateur ou la désactivation de l’accès d’un utilisateur à l’application dans l’IdP entraînera la *désactivation* de cet utilisateur dans votre plan Miro Enterprise.</span> Selon les circonstances, la désactivation d’un utilisateur peut entraîner la réaffectation de son contenu aux plus anciens admins de l’équipe :
  - si vous désactivez l’utilisateur du côté de l'IDP mais que vous le laissez affecté à l’application Miro, son appartenance à l’équipe du côté de Miro n’est pas modifiée, et son contenu n’est pas réaffecté - il passe simplement de l’état **Actif** à l’état **Désactivé** (et à la section des utilisateurs, respectivement) et cesse de consommer une licence.
  - si vous déclenchez la désactivation en supprimant l’utilisateur dans l'IDP ou en le désassignant de l’application Miro, alors que l’utilisateur est membre de certaines *équipes synchronisées*, l’utilisateur sera également supprimé de *ces* équipes Miro et son contenu dans lesdites équipes sera réassigné aux admins d’équipes les plus anciens.
  - si vous déclenchez la désactivation en *supprimant* l'utilisateur dans l’IDP ou en le *désaffectant* de l'application Miro, lorsque l'utilisateur n'est membre d'aucune équipe *synchronisée*, son appartenance aux équipes ne sera pas modifiée et son contenu ne sera pas réaffecté.
  **La suppression d’un utilisateur** de l’abonnement Enterprise n’est pas prise en charge *par défaut.* Vous pouvez néanmoins [ajouter manuellement la fonctionnalité à l’aide de l’API](https://developers.miro.com/docs/scim#section-delete-user-by-id) pour supprimer complètement l’utilisateur de l’abonnement au lieu de lui attribuer le statut **Désactivé**. Dans ce scénario, le contenu est réattribué aux membres respectifs de l’équipe. Il est impossible de définir quels seront les admins qui récupéreront la propriété du contenu lors de sa réaffectation automatique. Mais cela peut être défini lorsque vous [désactivez manuellement un utilisateur dans les paramètres de Miro.](../../enterprise-administration/user-management/01-deactivated-users.md)
- **Réactiver les utilisateurs**
  La réassignation d'un utilisateur à l'application ou la réactivation de son profil dans l'IDP le réactivera dans votre abonnement Miro Enterprise s'il a été préalablement provisionné et désactivé.
- **Automatisation de l’attribution des groupes de facturation**
  Affecter automatiquement les nouveaux utilisateurs aux [billing groups](../../enterprise-administration/enterprise-subscription-management/enterprise-billing/01-billing-groups.md) à l'aide de SCIM. Une fois votre fournisseur d’identité (IdP) configuré, reliez vos centres de coûts à vos groupes de facturation. Ainsi, chaque utilisateur actuel et futur de ces centres de coûts est automatiquement classé dans la bonne catégorie de facturation.

Vous pouvez également supprimer des utilisateurs de votre plan Enterprise en envoyant un appel API de **suppression** direct - veuillez consulter la documentation [ici](https://developers.miro.com/docs/scim#section-delete-user-by-id). Notez que seuls les appels *directs* supprimeront les utilisateurs. **Les événements de suppression** initiés *par votre solution d’identité* seront traités comme une demande de **désactivation**.

### Attributs pris en charge

:::warning
Notez que :
- **E-mail** / Le paramètre principal / Identifiant unique / **Nom d’utilisateur**) est la seule valeur requise par Miro et doit se présenter sous la forme d’un e-mail.
- la mise à jour de l’e-mail n’est possible que pour les utilisateurs déjà synchronisés.</span> En d’autres termes, la première synchronisation doit avoir lieu lorsque l’e-mail dans l’IdP et Miro est le même, sinon Miro ne reconnaîtra pas l’utilisateur et un profil Miro en double sera créé sous le nouvel e-mail.
- la mise à jour de l'e-mail doit se faire dans le profil IdP de l'utilisateur, et non dans la liste des affectations.
- Contrairement aux autres attributs, la mise à jour de l'**Adresse e-mail** de l’utilisateur lui enverra une notification : l’ancienne et la nouvelle adresse e-mail recevront toutes deux une lettre indiquant à l’utilisateur qu’il doit désormais utiliser sa nouvelle adresse e-mail pour se connecter à Miro.
:::

| Nom de l’attribut | Attribut SCIM (Revendication) |
| --- | --- |
| E-mail | Nom d'utilisateur.  **Doit être présent et sous la forme d'une adresse e-mail** |
| *Les attributs énumérés ci-dessous ne sont pas requis et seront acceptés par Miro s'ils sont présents (les autres attributs envoyés à Miro seront ignorés).* | |
| Nom complet | displayName;      formaté;      givenName + " " + familyName;      Nom d’utilisateur |
| Type d’utilisateur | type d'utilisateur       valeur prise en charge: Plein" |
| Actif | actif       valeur prise en charge : "true" ou "false" |
| Photo de profil | **photos.^[type=='photo'].value** ou     **photos.^[type==photo].value** (Okta)     **photos[type eq "photo"].value** (Entra)        Il doit s’agit d’une URL textuelle vers l’image.  Types de fichiers pris en charge : jpg, jpeg, bmp, png, gif       Pour définir le type de fichier, vous devez avoir défini l'extension du fichier dans l'url       (par exemple `https://host.com/avatar_user1.jpg`) ou la requête à l'url             doit renvoyer avec le contenu du fichier un en-tête Content-            Type (par exemple Content-Type = 'image/jpeg')        La taille maximale du fichier à télécharger est de : </span> 31457280 octets |
| Rôle de l’utilisateur | roles.^[primary==true].value (Okta)      roles[primary eq "True"].value (Entra)        valeurs prises en charge :  **ORGANISATION_INTERNAL_ADMIN** **UTILISATEUR_INTERNE_ORGANISATION** |
| Numéro d’employé | employeeNumber |
| Centre de coûts | costCenter |
| Organisation | organisation |
| Division | division |
| Département | département |
| Nom du manager | AffichageNomDuGestionnaire |
| ID du gestionnaire | manager.value  Le champ "value" est de type String dans le standard SCIM mais managerId       Le champ interne Miro est de type Long. Si l’attribut "value" n’est pas       valeur du nombre nous ignorons cette valeur |

:::warning
Les changements de mot de passe ne sont pas pris en charge et il n’est pas prévu de le faire dans l’immédiat.
⚠️ **Nom d'utilisateur**, **Type d'utilisateur** et **roles.value** ne peuvent pas être mis à jour pour [les utilisateurs désactivés](../../enterprise-administration/user-management/01-deactivated-users.md).
:::

Tous les attributs seront affichés dans le fichier CSV des utilisateurs exporté qui peut être téléchargé depuis la [section Utilisateurs actifs](../../enterprise-administration/user-management/12-user-management-overview-on-enterprise-plan.md).

![download_as_CSV_in_company_settings.jpg](images/26547048889490_download%20as%20CSV%20in%20company%20settings.jpg)
*L’option permettant de télécharger une liste d’utilisateurs*

![mceclip3.png](images/26547048890514_mceclip3.png)

## Configuration du SCIM

### Étape 1 : Activer l’option SCIM dans Miro

Pour activer le SCIM pour votre forfait Miro Enterprise, allez dans les **paramètres de l’entreprise** > **Intégrations Enterprise,** activez la fonction SCIM Provisioning**.</strong>** Vous y trouverez l’URL de base et le jeton API pour configurer votre IdP.

![scim.png](images/26547048892562_scim.png)
*SCIM dans les paramètres Miro*

### Étape 2 : Configurez votre fournisseur d’identité

La configuration dépendra du fournisseur d’identité que vous utilisez.</span> Miro prend en charge Okta et Entra ID préconfigurés, mais vous pouvez utiliser n’importe quel fournisseur d’identité de votre choix tant qu’il permet de configurer le SCIM.

OKTA - consultez les instructions de configuration [ici](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md).

Entra ID - voir les instructions de configuration [ici](../../enterprise-administration/security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md).

## Générer un nouveau jeton

1. Accédez aux **paramètres de l’entreprise** > **Intégrations Enterprise.**

2. Dans la **section SCIM Provisioning**, cliquez sur **Générer un nouveau jeton**.

![scim.png](images/26547048892562_scim.png)
*SCIM dans les paramètres Miro*

2. Dans la fenêtre **Générer un nouveau jeton SCIM**, cliquez sur **Générer**.

![generate_token.png](images/26547048895506_generate_token.png)

3. Après avoir généré un nouveau jeton, vous devez configurer le nouveau jeton dans votre fournisseur IDP.

## Problèmes éventuels et comment les résoudre

*1. Les utilisateurs ne sont pas provisionnés en raison d’une erreur dans la liste d’autorisation.*
![mceclip0.png](images/26547048896786_mceclip0.png)
*Exemple d’erreur provenant du fournisseur d’identité Okta*

Assurez-vous que l’adresse du domaine de l’utilisateur est ajoutée à votre liste d’autorisations [dans les **paramètres de sécurité**](../../enterprise-administration/canvas-25-admin-features/data-security/07-sharing-policy-on-enterprise-plan.md).

*2. <em>Si vous authentifiez vos utilisateurs finaux avec une solution d'identité (IDP1) mais que vous souhaitez activer SCIM via une autre solution (IDP2), cela est possible à deux conditions :*

1. l’IdP2 peut faire des appels d’API avec le jeton titulaire.
2. Les deux fournisseurs d’identité sont synchronisés (c’est-à-dire que les utilisateurs approvisionnés par le SCIM existent dans l’IDP1 également et peuvent donc s’authentifier avec Miro).

Pour plus d'informations, veuillez [contacter l'équipe d'assistance Miro](https://help.miro.com/hc/en-us/requests/new?referer=help-center-article).
