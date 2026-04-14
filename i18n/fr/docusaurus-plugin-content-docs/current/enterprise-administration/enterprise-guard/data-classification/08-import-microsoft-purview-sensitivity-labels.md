---
title: "Importer les badges de sensibilit\xE9 Microsoft Purview"
article_id: 22161930709010
translation_id: 22161930709010
locale: fr
sidebar_position: 7
created_at: '2024-10-23T15:05:49Z'
updated_at: '2025-12-01T16:32:38Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Pour les organisations utilisant Microsoft Purview, maintenir une sécurité de données et une classification cohérentes sur plusieurs plateformes est essentiel. L'intégration de Miro avec Microsoft Purview permet aux administrateurs d'importer directement des badges de sensibilité de Microsoft Purview dans Miro, simplifiant ainsi la gestion des schémas de classification sur les deux plateformes.

En tirant parti de cette intégration, les organisations peuvent s'assurer que le contenu au sein de Miro est classé de manière cohérente avec le cadre établi par Microsoft Purview. Cela réduit non seulement la charge opérationnelle liée à la recréation ou à la mise à jour manuelle des badges de classification, mais aussi renforce la sécurité des données. En alignant les capacités de protection des données de Miro avec Microsoft Purview, les administrateurs peuvent gérer en toute confiance les informations sensibles dans l'ensemble de leur écosystème numérique.

## Importer les badges de sensibilité Microsoft Purview dans Miro

Si votre organisation n'a pas encore configuré la classification des données dans Miro, vous pouvez facilement mettre en place la fonctionnalité de classification en important directement les badges de sensibilité existants depuis Microsoft Purview.

Si vous avez déjà une configuration de classification des données, vous pouvez importer des badges de sensibilité depuis Microsoft Purview et transférer les badges de classification existants dans Miro.

## Configurez la fonctionnalité de classification en important des badges de sensibilité depuis Microsoft Purview

### Prérequis

- Assurez-vous de disposer des rôles ou privilèges nécessaires pour travailler avec les étiquettes de sensibilité dans Microsoft Purview.
- Vous devez connaître les détails des niveaux de classification des tableaux que vous souhaitez configurer en fonction de vos exigences en matière de sécurité et de gouvernance.
- Vous devez avoir le [rôle d’admin de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin de contenu sensible, contactez l’admin de votre entreprise.

:::note
Notes :
- Selon la documentation de Microsoft, la mise à jour des badges de sensibilité dans Microsoft Purview peut prendre jusqu'à 24 heures pour se répliquer à toutes les applications et services. Veuillez laisser suffisamment de temps pour que les modifications aient lieu, puis importez les badges de sensibilité. Si les mises à jour que vous avez effectuées dans MS Purview ne sont pas répliquées après 24 heures, veuillez contacter le service d’assistance Microsoft Purview.
- Vous pouvez importer jusqu'à 50 badges de sensibilité depuis Microsoft Purview dans Miro.
- Si vous avez déjà une configuration de classification des données existante, vous pouvez importer des étiquettes de sensibilité de Microsoft Purview et transférer les étiquettes de classification existantes dans Miro. Pour plus d'informations, consultez [Importation d'étiquettes de sensibilité de Microsoft Purview dans une configuration de classification existante dans Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Pour importer des étiquettes de sensibilité de Microsoft Purview et configurer la classification des données dans Miro, suivez les étapes suivantes :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **la fonctionnalité de classification**.
3. Sur la page **Classification**, en bas de l'écran, cliquez sur **Commencer**.
4. Sur la boîte **Importer depuis Microsoft Purview**, cliquez sur **Se connecter**.
5. Sur la page **Microsoft Sign in** qui s'ouvre dans un nouvel onglet, entrez vos identifiants Microsoft et connectez-vous. Une fois connecté à votre compte Microsoft, l'onglet se ferme automatiquement.
6. Sur la **page Classification**, dans la boîte **Import from Microsoft Purview**, cliquez sur **Importer**.
   La page **Importer la classification à partir de Microsoft Purview** apparaît.
7. Sélectionnez la case à cocher pour les badges de sensibilité de Microsoft Purview que vous souhaitez utiliser comme niveaux de classification dans Miro, puis cliquez sur **Suivant**.

   > ✏️ Selon la documentation de Microsoft, la mise à jour des badges de sensibilité dans Microsoft Purview peut prendre jusqu'à 24 heures pour se répliquer dans toutes les applications et services. Veuillez donc prévoir suffisamment de temps pour que les modifications prennent effet, puis importer les badges de sensibilité. Si les mises à jour que vous avez effectuées dans MS Purview ne sont pas répliquées après 24 heures, veuillez contacter le service d’assistance de Microsoft Purview.
8. Sur la page **Définir les niveaux de classification**, vous pouvez modifier les niveaux de classification pour assigner le niveau de classification par défaut ou ajouter un lien vers les directives. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Lien vers les lignes directrices** | URL qui fournit des informations supplémentaires sur les politiques ou instructions applicables à ce niveau de classification. Cela pourrait être une page qui offre plus d'informations aux utilisateurs de votre organisation pour en savoir plus sur vos niveaux de classification de tableaux et comment les utiliser. Vous devez fournir l'URL dans le format suivant : `http://www.example.com`  Quand l'utilisateur clique sur l'icône **En savoir plus** (icône point d'interrogation) à côté du badge de classification du tableau, cette URL est chargée dans un nouvel onglet du navigateur. |
   | **Utiliser comme niveau par défaut pour les nouveaux tableaux** | Sélectionnez cette case pour définir ce niveau de classification comme niveau de classification par défaut pour tous les nouveaux tableaux. |
   | **Aperçu** | Affiche un aperçu du badge de classification du tableau avec sa description et son icône d'information. Cet aperçu montre exactement comment le badge de classification apparaît pour les utilisateurs sur un tableau. |
9. Pour enregistrer la configuration du niveau de classification, cliquez sur **Terminé**.
10. Cliquez sur **Suivant**. Votre configuration est enregistrée, mais elle ne prendra effet qu'après avoir cliqué sur **Publier** sur la page [**Réviser l'impact**](https://help.miro.com/hc/articles/16494764223378).

    Vous pouvez ensuite passer à l'une des étapes suivantes :

    - [Définir l’auto-classification](09-define-auto-classification.md). Ceci est facultatif. Si vous souhaitez définir l’auto-classification ultérieurement, cliquez sur **Suivant**.
    - [Définir des garde-fous](05-define-guardrails.md). C'est facultatif. Si vous souhaitez définir des garde-fous plus tard, cliquez sur **Suivant**.
    - [Examiner l'impact](https://help.miro.com/hc/articles/16494764223378). C'est la dernière étape du workflow et elle est obligatoire.

## Importer les badges de sensibilité de Microsoft Purview dans la configuration existante de la fonctionnalité de classification de Miro

### **Prérequis**

- Assurez-vous de disposer des rôles ou privilèges nécessaires pour travailler avec les étiquettes de sensibilité dans Microsoft Purview.
- Vous devez connaître les détails des niveaux de classification des tableaux que vous souhaitez configurer en fonction de vos exigences en matière de sécurité et de gouvernance.
- Vous devez avoir le [rôle d’admin de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.

:::note
Notes :
- Selon la documentation de Microsoft, les mises à jour des badges de sensibilité dans Microsoft Purview peuvent prendre jusqu'à 24 heures pour se répliquer dans toutes les applications et services. Veuillez laisser suffisamment de temps pour que les modifications prennent effet, puis importez les badges de sensibilité. Si les mises à jour que vous avez effectuées dans MS Purview ne sont pas répliquées après 24 heures, veuillez contacter le service d’assistance de Microsoft Purview.
- Vous pouvez importer jusqu'à 50 badges de sensibilité de Microsoft Purview vers Miro.
- Vous ne pouvez pas transférer les niveaux de classification utilisés dans les politiques de conservation. Vous devez vous assurer que les niveaux de classification ne sont pas utilisés dans aucune politique de conservation avant de procéder. Pour plus d'informations, voir [Modifier la politique de conservation](../content-lifecycle-management/11-edit-retention-policy.md).
:::

Pour importer les étiquettes de sensibilité à partir de Microsoft Purview et les transférer/cartographier avec les étiquettes de classification existantes dans Miro, effectuez les étapes suivantes :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **Classification des données**.
3. Sur la page **Classification**, en haut de l'écran, cliquez sur **Importer**.
4. Si vous êtes déjà connecté à Microsoft, passez cette étape et continuez avec l'étape suivante.
   Si vous n'êtes pas connecté à Microsoft, cliquez sur **Se connecter**. Sur la page **Connexion Microsoft** qui s'ouvre dans un nouvel onglet, entrez vos identifiants Microsoft et connectez-vous. Une fois connecté à votre compte Microsoft, l'onglet se ferme automatiquement.
5. Dans le cadre **Importer depuis Microsoft Purview**, cliquez sur **Importer** à côté de "Importer les badges de sensibilité dans Miro". La page **Importez la classification à partir de Microsoft Purview** s'affiche.
6. Sur la page **Importer des niveaux**, cochez la case des badges de sensibilité de Microsoft Purview que vous souhaitez utiliser comme niveaux de classification dans Miro, puis cliquez sur **Suivant**. La page **Transférer les niveaux existants** s'affiche.

   > ✏️ Selon la documentation de Microsoft, les mises à jour des badges de sensibilité dans Microsoft Purview peuvent prendre jusqu'à 24 heures pour être répliquées dans toutes les applications et services. Veuillez accorder suffisamment de temps pour que les modifications prennent effet, puis importez les badges de sensibilité. Si les mises à jour que vous avez effectuées dans MS Purview ne sont pas répliquées après 24 heures, veuillez contacter le service d'assistance de Microsoft Purview.
7. Pour garantir que le contenu est classifié correctement, vous devez transférer les niveaux de classification existants de Miro vers les nouveaux niveaux importés de Microsoft Purview. Les niveaux listés à gauche sont les niveaux de classification existants de Miro, et ceux listés dans le menu déroulant à droite sont les badges de sensibilité de Microsoft Purview importés. Une fois terminé, cliquez sur **Suivant**.
8. Sur la page **Définir les niveaux de classification**, vous pouvez modifier les niveaux de classification pour attribuer le niveau de classification par défaut ou ajouter un lien vers les directives. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Lien vers les lignes directrices** | URL qui fournit plus d'informations sur les politiques ou instructions applicables à ce niveau de classification. Cela pourrait être une page qui offre des informations supplémentaires aux utilisateurs de votre organisation pour en savoir plus sur vos niveaux de classification de tableau et comment les utiliser. Vous devez fournir l'URL au format suivant : `http://www.example.com`  Lorsque l'utilisateur clique sur l'icône **En savoir plus** (icône de point d'interrogation) à côté de l'insigne de classification du tableau, cette URL s'ouvre dans un nouvel onglet du navigateur. |
   | **Utiliser comme niveau par défaut pour les nouveaux tableaux** | Sélectionnez cette case pour définir ce niveau de classification comme classification par défaut pour tous les nouveaux tableaux. |
   | **Aperçu** | Affiche un aperçu du badge de classification du tableau avec sa description et l'icône d'apprentissage supplémentaire. L'aperçu montre exactement comment le badge de classification apparaît pour les utilisateurs sur un tableau. |

   Pour enregistrer la configuration du niveau de classification, cliquez sur **Terminé**.
9. Cliquez sur **Suivant**. Votre configuration est enregistrée, mais elle ne prendra effet que lorsque vous cliquerez sur **Publier** sur la page [**Vérifier l'impact**](https://help.miro.com/hc/articles/16494764223378).

   Vous pouvez ensuite continuer avec l'une des étapes suivantes :

   - [Définissez l'auto-classification](09-define-auto-classification.md). Ceci est facultatif. Si vous souhaitez définir l'auto-classification plus tard, cliquez sur **Suivant**.
   - [Définir les garde-fous](05-define-guardrails.md). Ceci est facultatif. Si vous souhaitez définir les garde-fous plus tard, cliquez sur **Suivant**.
   - [Revoir l'impact](https://help.miro.com/hc/articles/16494764223378). C'est la dernière étape du workflow et elle est obligatoire.

## Se déconnecter de Microsoft Purview

Lorsque vous êtes connecté à Purview, vous ne pouvez pas ajouter ou modifier les noms de classification, mettre à jour les niveaux de classification, etc. Si vous souhaitez effectuer ces actions, vous devez vous déconnecter de Microsoft Purview. Vous ne pouvez pas importer de mises à jour de Microsoft Purview dans Miro une fois déconnecté de Purview.

Pour vous déconnecter de Microsoft Purview, suivez les étapes suivantes :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard**, cliquez sur **classification des données**.
3. Sur la page **Classification**, en haut de l'écran, cliquez sur le bouton **Dernière Importation**, puis cliquez sur **Déconnecter de Purview**.
