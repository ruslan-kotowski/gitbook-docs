---
title: Ajout de plusieurs fournisseurs d'identité
article_id: 16287287497234
translation_id: 16287287497234
locale: fr
sidebar_position: 1
created_at: '2024-01-10T10:51:24Z'
updated_at: '2026-02-18T08:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
availability:
  notes: 'Disponible pour: Enterprise Configuré par: admins d’entreprise'
---

:::note
L’ajout de plusieurs fournisseurs d’identité est une fonctionnalité privée disponible exclusivement pour les clients Enterprise. Pour accéder et activer cette fonctionnalité, contactez votre responsable de comptes Miro ou Customer Success Manager. Le service d’assistance de Miro ne peut pas activer cette fonctionnalité.
:::

Utilisez plusieurs fournisseurs d’identité (IdPs) pour l’authentification unique (SSO). Ceci est particulièrement utile pour les grandes organisations ayant différentes succursales ou filiales, chacune ayant son propre IdP mais devant avoir accès au même abonnement Miro.

## Préparation à l’ajout de plusieurs fournisseurs d’identité

Pour garantir que [l’authentification unique (SSO)](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md) continue de fonctionner après l’ajout de plusieurs applications de fournisseurs d’identité, vous devez mettre à jour la configuration de l’application fournisseur d’identité existante.

Entra ID et certains autres fournisseurs d’identité ne prendront pas en charge le nouveau format de configuration tant que votre organisation n’aura pas activé la fonction privée de fournisseur d’identité multiple. Pour éviter les interruptions de connexion, nous vous suggérons d’organiser un appel avec votre responsable Customer Success, qui pourra vous guider étape par étape pour activer la fonction privée multi-fournisseurs d’identité en même temps que la configuration est mise à jour.

### Comment configurer vos paramètres Enterprise

1. Désactiver SCIM.
2. Mettre à jour la configuration SSO.
3. Vérifier la fonctionnalité du SSO.

#### Désactiver SCIM

Nous ne prenons actuellement pas en charge [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) avec plusieurs IdP. Pour désactiver SCIM pour votre forfait Enterprise, allez dans les paramètres de **l’entreprise** > **Compte** > **Intégrations Enterprise**, et désactivez le **Provisionnement SCIM**.

#### Mettre à jour la configuration SSO

**Ancienne configuration**

Lors de la configuration initiale de Miro SSO dans votre fournisseur d’identité, il est probable que les valeurs de configuration suivantes aient été utilisées :

- **URL de rappel/ACS :** https://miro.com/sso/saml
- **ID d'entité :** https://miro.com

**Nouvelle configuration**

Pour que le fournisseur d’identité sache à quelle configuration de Miro il se rapporte, les valeurs ci-dessous doivent être mises à jour. Accédez à **Paramètres** > **Sécurité** > **Authentification**.

Ces valeurs sont disponibles dans les paramètres SSO une fois que votre organisation a activé la fonctionnalité privée multi-IdP et auront le format suivant :

- **URL de rappel/ACS :** https://miro.com/sso/saml/&lt;org_id&gt;/&lt;saml_settings_id&gt;
- **ID de l’entité :** "https://miro.com/&lt;org_id&gt;/&lt;saml_settings_id&gt;

![Callback URL and Entity ID in the Enterprise admin console](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/23763575205778_image.png)

*URL de rappel et ID de l’entité dans la console d’admin Enterprise*

#### Vérifiez le bon fonctionnement de votre authentification unique (SSO)

Une fois la mise à jour de votre configuration fournisseur d’identité terminée, testez le bon fonctionnement du SSO en vous déconnectant et en vous reconnectant.

## Ajout d’un nouveau fournisseur d’identité

Le processus pour ajouter de nouveaux IdP est similaire à celui de la [configuration SSO](../../security-integrations/single-sign-on-sso/09-single-sign-on-sso.md), mais inclut quelques changements clés :

- **Nouveaux champs :** « Nom du fournisseur d’identité » et « Description du fournisseur d’identité » (facultatif). Ces champs aident les utilisateurs et les admins à identifier le bon fournisseur d’identité lors de la connexion, en particulier si plusieurs fournisseurs d’identité sont utilisés.

  Étant donné que ces champs sont affichés dans les paramètres d’administration et peuvent être montrés aux utilisateurs lorsqu’ils se connectent via SSO, nous vous recommandons vivement de définir ces noms de manière intentionnelle (par exemple, unité commerciale ou nom du fournisseur d’identité).

  ![idP-name-and-IdP description.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016020733970_idP-name-and-IdP%20description.png)
*L’option d’ajout de nom et de description du fournisseur d’identité*
- **Champs en lecture seule :** 'URL de rappel' (URL de rappel autorisée, URL de service consommateur d'assertion personnalisé, URL de réponse) et 'ID de l’entité' (identifiant, identifiant d’approbation de partie de confiance) sont maintenant générés automatiquement dans vos paramètres IdP de Miro une fois que votre organisation a activé la fonctionnalité privée multi-IdP.

  Auparavant, ces valeurs étaient statiques car elles étaient les mêmes pour toutes les configurations de fournisseur d’identité. Une fois générées, vous devrez également copier et coller ces valeurs dans les champs correspondants des paramètres de votre fournisseur d’identité.

  ![Callback-ID-and-Entity-ID-fields.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034166290_Callback-ID-and-Entity-ID-fields.png)
*Champs URL de rappel et ID de l’entité*

## Gestion de plusieurs fournisseurs d’identité (IdPs)

> **💡** Vous pouvez ajouter et activer jusqu’à 20 fournisseurs d’identité à la fois.

Après avoir ajouté les IdPs, chaque configuration peut être activée ou désactivée selon les besoins. Pour désactiver un IdP, allez dans les paramètres de **Entreprise** > **Compte** > **Authentification**, et désactivez l'IdP.

![Toggle-on-or-off-IdPs.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/21016034165010_Toggle-on-or-off-IdPs.png)
*L’option pour activer ou désactiver un IdP*

## Connexion pour les domaines de messagerie avec plusieurs IdP

Si le domaine de messagerie d’un utilisateur est lié à plusieurs configurations de fournisseur d’identité, il peut en sélectionner une lors de la connexion. Si ces configurations ont des domaines distincts, l’utilisateur est automatiquement redirigé vers le fournisseur d’identité correspondant.

![sso-screenshot.png](../../../../../../../docs/enterprise-administration/security-compliance/single-sign-on-sso/images/22437449166610_sso-screenshot.png)
*Vue de plusieurs IdP lors de la connexion*
