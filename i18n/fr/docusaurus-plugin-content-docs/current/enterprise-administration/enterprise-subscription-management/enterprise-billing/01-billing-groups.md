---
title: Groupes de facturation
article_id: 6574185673874
translation_id: 6574185673874
locale: fr
sidebar_position: 1
created_at: '2022-07-12T12:53:45Z'
updated_at: '2026-02-19T10:50:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: billing-groups
---

Les groupes de facturation permettent aux admins d’entreprise de faire correspondre des utilisateurs à des budgets internes. Étant donné que chaque utilisateur ne peut être assigné qu'à un seul groupe, les admins peuvent facilement suivre le nombre de licences utilisées par chaque centre de coûts. Les admins peuvent également définir un quota conditionnel sur les licences disponibles pour chaque groupe de facturation. Cela simplifie les processus comme la mise à jour, le renouvellement et le refacturation des licences pour les équipes.

> **Disponible pour :** Enterprise Plan
> **Qui peut le faire :** Admins d’entreprise

## Paramètres des groupes de facturation

Vos paramètres de groupe de facturation offrent une vue d'ensemble complète de l'utilisation des licences. Par exemple, les détails de tous les groupes de facturation existants, y compris le nombre d'utilisateurs, le nombre de chaque type de licences, et, si attribué, le [quota conditionnel](02-billing-groups-soft-quotas.md) de licences allouées par groupe. Utilisez le champ de recherche pour trouver rapidement un groupe de facturation spécifique.

### Où trouver vos groupes de facturation

Pour trouver vos paramètres de groupe de facturation, allez dans **Paramètres** **de l'entreprise** > **Abonnement** > **Groupes de facturation.**

:::note
Les utilisateurs non assignés à un groupe de facturation sont automatiquement placés dans le groupe de facturation par défaut de l'entreprise. Vous pouvez voir le nombre d'utilisateurs actifs assignés dans la bannière située en haut des paramètres de votre groupe de facturation.
:::

## Comment créer un groupe de facturation

1. Allez dans **Paramètres de l'entreprise** > **Abonnement** > **Groupes de facturation**.
2. Cliquez sur **Créer un groupe de facturation**.
3. Ajoutez le nom du groupe de facturation.
4. (Optionnel) Pour définir une quota conditionnel sur les licences attribuées à ce groupe de facturation, sélectionnez **Ajouter quota pour les licences Standard** ou **Ajouter quota pour les licences Avancées**, et entrez un nombre.
   Pour en savoir plus sur les quotas conditionnels, voyez la FAQ à la fin de cet article.
5. Pour ajouter de nouveaux utilisateurs au groupe de facturation, vous pouvez charger un fichier CSV contenant la liste des adresses e-mail des utilisateurs, ou attribuer des utilisateurs plus tard.
6. (Facultatif) Attribuez un contact pour le groupe de facturation. Ce contact peut être joint pour obtenir des informations sur l'utilisation des licences.
7. Cliquez sur **Créer un groupe de facturation**.

## Comment modifier un groupe de facturation

Vous pouvez modifier le nom d'un groupe de facturation, définir ou mettre à jour un quota conditionnel, changer le contact du groupe de facturation et ajouter des utilisateurs au groupe de facturation.

:::note
L'ajout d'utilisateurs à un nouveau groupe de facturation les transfère automatiquement de leur groupe précédent.
:::

1. Allez dans **Paramètres de l'entreprise** > **Abonnement** > **Groupes de facturation**.
2. Cliquez sur les trois points à côté d’un groupe de facturation et choisissez **Modifier**.
3. Modifiez n'importe quelle propriété du groupe de facturation. Pour ajouter des utilisateurs au groupe de facturation, chargez un fichier CSV avec la liste des adresses e-mail des utilisateurs, ou attribuez des utilisateurs ultérieurement.
4. Cliquez sur **Enregistrer**.

## Comment supprimer un groupe de facturation

1. Allez dans les **Paramètres de l'entreprise** > **Abonnement** > **Groupes de facturation**.
2. Cliquez sur les trois points à côté d’un groupe de facturation et sélectionnez **Supprimer**.
3. Confirmez la suppression.
4. Tous les utilisateurs qui faisaient partie de ce groupe de facturation seront réassignés au compte principal et ne feront plus partie d’aucun groupe de facturation.

## Comment affecter un utilisateur à un groupe de facturation

Un utilisateur ne peut être membre que d’un seul groupe de facturation au sein de l’organisation.

1. Accédez aux paramètres de **l’entreprise** > **Utilisateurs actifs**.
2. Cliquez sur les trois points à côté d’un utilisateur.
3. Choisissez **Changer de groupe de facturation**.
4. Sélectionnez un groupe de facturation et cliquez sur **Affecter un utilisateur**. L’utilisateur sera ajouté au nouveau groupe de facturation.

## Comment affecter plusieurs utilisateurs à la fois à un groupe de facturation

Affectez plusieurs utilisateurs à un groupe de facturation en une seule fois.

1. Accédez aux paramètres de **Société** > **Utilisateurs actifs**.
2. Sélectionnez les utilisateurs manuellement ou appliquez des filtres et sélectionnez-en jusqu’à 50 à la fois.
3. Cliquez sur **Actions groupées** et sélectionnez **Affecter un groupe de facturation**.
4. Choisissez un groupe et cliquez sur **Affecter des utilisateurs**. Si certains utilisateurs sont déjà membres d’autres groupes de facturation, vous pourrez les désélectionner ou modifier leur affectation à un groupe de facturation.

## Comment vérifier quels utilisateurs sont dans un groupe de facturation

Vérifiez qui est dans un groupe de facturation pour mieux gérer l'accès des utilisateurs et la facturation.

1. Allez dans les **Paramètres** de l'entreprise > **Abonnement** > **Groupes de facturation**.
2. Cliquez sur un groupe de facturation spécifique pour voir les utilisateurs qui y sont assignés.

## Comment supprimer un utilisateur d'un groupe de facturation

Si un utilisateur n'est pas assigné à un groupe de facturation spécifique ou est retiré d'un groupe, il est automatiquement placé par défaut dans le groupe de facturation standard de l'entreprise.

1. Accédez aux **Paramètres de l’entreprise** > **Utilisateurs actifs**.
2. Cliquez sur les trois points à côté d’un utilisateur.
3. Choisissez **Changer de groupe de facturation**.
4. Sélectionnez **Groupe de facturation par défaut du compte**. L’utilisateur sera supprimé du groupe de facturation et fera maintenant partie du groupe de facturation général de l’entreprise.

## Comment affecter des utilisateurs à un groupe de facturation via un fichier CSV

Affectez plusieurs utilisateurs à un groupe de facturation en chargeant un fichier CSV avec des adresses e-mail d’utilisateurs. Si un utilisateur fait déjà partie d’un autre groupe de facturation, il est déplacé vers le nouveau groupe de facturation.

:::note
Assurez-vous que votre fichier CSV ne comporte qu’une seule colonne avec l’en-tête « e-mail ». Cette colonne doit contenir votre liste d’adresses e-mail à ajouter au groupe de facturation. Vérifiez que votre fichier CSV utilise bien des virgules pour séparer les valeurs. Les informations contenues dans les colonnes supplémentaires ne seront pas traitées. Miro n’enregistre pas les fichiers CSV.
:::

1. Allez dans les paramètres de la **Société** > **Abonnement** > **Groupes de facturation**.
2. Cliquez sur les trois points à côté d’un groupe de facturation et sélectionnez **Modifier**.
3. Chargez un fichier CSV contenant la liste des adresses e-mail des utilisateurs.
4. Cliquez sur **Enregistrer**.

## Comment affecter des utilisateurs à un groupe de facturation via SCIM

Configurez [SCIM](../../security-integrations/system-for-cross-domain-identity-management-scim/02-scim.md) pour attribuer automatiquement les utilisateurs à un groupe de facturation selon un centre de coût.

#### Étape 1 : configurez votre fournisseur d’identité

Assurez-vous que votre fournisseur d’identité est configuré pour ajouter le centre de coût à Miro. Consultez les guides pour :

- [Configurer le provisionnement automatisé avec OKTA](../../security-integrations/system-for-cross-domain-identity-management-scim/05-setting-up-automated-provisioning-with-okta.md)
- [Configurer le provisionnement automatisé avec Azure AD](../../security-integrations/system-for-cross-domain-identity-management-scim/03-setting-up-automated-provisioning-with-entra-id.md)

#### Étape 2 : attribuez des centres de coût à votre groupe de facturation

Ajoutez un ou plusieurs centres de coûts à un groupe de facturation. Tous les utilisateurs actuels et futurs de ces centres de coûts rejoindront automatiquement le groupe de facturation.

**Comment ajouter un centre de coûts**

1. Ouvrez la page **Modifier le groupe de facturation**.
2. Saisissez votre centre de coûts dans le champ **Insérer le centre de coûts**.
3. Appuyez sur **Entrée** sur votre clavier.
4. Ajoutez d'autres centres de coûts selon vos besoins.
5. Cliquez sur **Enregistrer**.

:::note
*Miro ne vérifie pas les informations que vous entrez pour les centres de coût. Assurez-vous d'entrer des noms de centres de coût précis. Ce champ n'est pas sensible à la casse.*
:::

### Géré par le badge SCIM

Les utilisateurs ayant un centre de coût assigné lié à un groupe de facturation, sont étiquetés comme **Géré par SCIM**. Vous verrez ce badge à côté du nom de l'utilisateur.

Ces utilisateurs ne peuvent pas être ajoutés manuellement à des groupes de facturation et ne peuvent recevoir un centre de coût que par une mise à jour SCIM.

### Directives pour les centres de coût et les groupes de facturation

- Un groupe de facturation peut contenir plusieurs centres de coûts, mais un seul centre de coûts peut être lié à un seul groupe de facturation.
- Pour réaffecter un centre de coûts, vous devez d'abord retirer le centre de coûts de son groupe de facturation actuel.
- Les utilisateurs assignés à un groupe de facturation en fonction de leur centre de coûts ne peuvent pas être assignés manuellement à un autre groupe de facturation.
- Supprimer un centre de coûts de votre groupe de facturation supprimera également tous les utilisateurs provisionnés par SCIM de ce groupe de facturation.
- Les utilisateurs non provisionnés par SCIM peuvent être manuellement assignés à tout groupe de facturation.

### Comment retirer un centre de coûts d'un groupe de facturation

1. Ouvrez la page **Modifier le groupe de facturation**.
2. Cliquez sur le **X**à côté du centre de coût que vous souhaitez supprimer.
3. Cliquez sur **Sauvegarder**.

## Comment exporter les données d’un groupe de facturation ?

Les admins d’entreprise peuvent exporter un fichier CSV contenant la liste des utilisateurs dans les **Paramètres de l’entreprise** > **Utilisateurs actifs**. Vous pouvez ensuite utiliser l’attribut des groupes de facturation dans la feuille de calcul CSV exportée pour filtrer les budgets.

## Foire aux questions

Que se passe-t-il lorsque mes utilisateurs changent de centre de coût du côté du fournisseur d’identité ?

Après une mise à jour SCIM :

- si ce nouveau centre de coût est assigné à un groupe de facturation, l'utilisateur sera automatiquement déplacé dans ce nouveau groupe de facturation.
- si ce nouveau centre de coût n'est pas assigné à un groupe de facturation ou si le centre de coût a été supprimé pour l'utilisateur dans le fournisseur d'identité, l'utilisateur sera automatiquement déplacé dans le groupe de facturation par défaut de l'entreprise.

Que se passe-t-il avec les utilisateurs qui ont été assignés manuellement à un groupe de facturation après l'implémentation de SCIM pour les groupes de facturation ?

Ils sont automatiquement assignés à un nouveau groupe de facturation selon leur centre de coût, tandis que ceux sans centre de coût correspondant ou sans centre de coût restent dans leur groupe de facturation actuel.

Pourquoi ne puis-je plus assigner manuellement un utilisateur à des groupes de facturation ?

Les utilisateurs assignés à un groupe de facturation par leur centre de coûts SCIM ne peuvent pas être déplacés manuellement vers un autre groupe.

Que se passe-t-il si mon IdP cesse de synchroniser l'attribut centre de coût avec Miro ?

Les nouveaux utilisateurs ne seront pas automatiquement affectés à un groupe de facturation sans centres de coûts synchronisés, mais peuvent être affectés manuellement jusqu'à ce que la synchronisation reprenne.

Qu'est-ce qu'une quota conditionnel pour un groupe de facturation ?

Une quota conditionnel vous permet de définir éventuellement une limite sur le nombre de licences Advanced, Standard ou Full (legacy) disponibles pour un groupe de facturation.

Lorsque vous créez ou modifiez un groupe de facturation, vous pouvez activer **Ajouter une quota pour les licences Standard** ou **Ajouter une quota pour les licences Advanced** et saisir un nombre.

La quota conditionnel apparaît, sous la forme du nombre que vous avez défini et d'une barre de progression indiquant la consommation, en haut de la vue d'ensemble du groupe de facturation.

Pour en savoir plus sur les quotas conditionnels, consultez [Quotas conditionnels pour les groupes de facturation](02-billing-groups-soft-quotas.md).
