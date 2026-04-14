---
title: "D\xE9finir les niveaux de classification"
article_id: 16494683650322
translation_id: 16494683650322
locale: fr
sidebar_position: 6
created_at: '2024-01-19T18:57:35Z'
updated_at: '2025-11-25T15:40:29Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
backstage_link:
  entity_kind: capability
  entity_id: content-classification-configuration
---

Il s'agit de la première étape du flux de configuration de l'auto-classification et des garde-fous. Dans cette étape du flux, vous pouvez définir les niveaux de classification, ce qui implique l'ajout de nouveaux niveaux de classification ou la mise à jour de la configuration d'un niveau de classification, comme le nom de la classification, l'ordre de sensibilité, la couleur du badge, le lien vers les directives de classification, etc. Lors de la définition des niveaux de classification, vous pouvez :

- [Ajouter ou modifier un niveau de classification](07-define-classification-levels.md)
- [Mettre en place la classification des données en important les étiquettes de sensibilité de Microsoft Purview](07-define-classification-levels.md)
- [Mise à jour du niveau de classification par défaut pour les nouveaux tableaux](07-define-classification-levels.md)
- [Mettre à jour l'ordre de sensibilité d'un niveau de classification](07-define-classification-levels.md)
- [Supprimer un niveau de classification](07-define-classification-levels.md)

## Prérequis

- Vous devez connaître les détails des niveaux de classification des tableaux que vous souhaitez configurer en fonction de vos exigences en matière de sécurité et de gouvernance.
- Vous devez avoir le [rôle d'administrateur de contenu sensible.](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.

## Ajouter ou modifier un niveau de classification

Vous pouvez ajouter ou modifier un niveau de classification en procédant comme suit :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **Classification des données**.
3. Si vous définissez des niveaux de classification pour la première fois, cliquez sur **Configurer la classification** en bas de l'écran.
   Si vous souhaitez modifier les niveaux de classification, cliquez sur **Modifier les niveaux de classification** en haut à droite de l'écran.
4. Sur la page **Définir les niveaux de classification**:
   Pour ajouter un niveau de classification, cliquez sur **Ajouter un niveau**.
   Pour modifier un niveau de classification, cliquez sur **Modifier les niveaux de classification.**
5. Ajoutez ou modifiez le niveau de classification en fonction de vos besoins. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Niveau** | Indique l'ordre de sensibilité du tableau pour ce niveau de classification.  Actuellement, l'ordre de sensibilité **1** indique le niveau de classification **le moins sensible.**  Cliquez sur les flèches vers le haut ou vers le bas pour attribuer l'ordre de sensibilité du tableau pour ce niveau de classification. |
   | **Nom** | Nom du niveau de classification.  Lorsque les utilisateurs consultent un tableau appartenant à ce niveau de classification, ce nom apparaît sur le badge de classification du tableau à côté du nom du tableau.  La figure 1 illustre un exemple où le nom de la classification du tableau est **INTERNE**.  sample_board_internal.png Figure 1 : Exemple où le nom de la classification du tableau est **INTERNE** |
   | **Description** | Description de ce niveau de classification.  Lorsque les utilisateurs visualisent un tableau appartenant à ce niveau de classification et qu'ils cliquent sur l'insigne de classification du tableau, la description du niveau de classification s'affiche.  Nous vous recommandons d'ajouter une description significative qui oriente vos utilisateurs sur la sensibilité de ce tableau et les précautions ou actions recommandées.  La figure 2 illustre un exemple de **description** ajoutée pour le niveau de classification INTERNE.   exemple_description_interne.png Figure 2 : Exemple de **description** ajoutée pour le niveau de classification INTERNE |
   | **Couleur du badge** | Couleur de fond de l'insigne de classification du tableau.  La figure 3 illustre un exemple où le niveau de classification du tableau INTERNE a une couleur de badge **jaune.**  sample_board_internal.png Figure 3 : Exemple où le niveau de classification du tableau "INTERNE" a une couleur de badge **jaune** |
   | **Lien vers les lignes directrices** | URL qui fournit plus d'informations sur les politiques ou les instructions applicables à ce niveau de classification. Il peut s'agir d'une page qui fournit davantage d'informations aux utilisateurs de votre organisation afin qu'ils en sachent plus sur les niveaux de classification de votre tableau et sur la manière de travailler avec eux. Vous devez fournir l'URL dans le format suivant : `http://www.example.com`  Lorsque l'utilisateur clique sur l'icône " **En savoir plus"** (point d'interrogation) à côté du badge de classification du tableau, cette URL est chargée dans un nouvel onglet du navigateur. |
   | **Utilisé comme niveau par défaut pour les nouveaux tableaux** | Cochez cette case pour définir ce niveau de classification comme classification par défaut pour tous les nouveaux tableaux. |
   | **Aperçu** | Affiche un aperçu du badge de classification du tableau avec sa description et l'icône pour en savoir plus. L'aperçu montre exactement comment l'insigne de classification apparaît aux utilisateurs d'un tableau. |

   Pour enregistrer la configuration du niveau de classification, cliquez sur **Terminé**.
6. Cliquez sur **Suivant**. Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. [**Examiner l'impact**](https://help.miro.com/hc/articles/16494764223378) sur la page Examiner l'impact.

   Vous pouvez ensuite passer à l'une des étapes suivantes :

   - Définir la classification automatique Cette option est facultative. Si vous souhaitez définir la classification automatique ultérieurement, cliquez sur **Suivant.**
   - Définir les garde-fous Cette option est facultative. Si vous souhaitez définir les garde-fous ultérieurement, cliquez sur **Suivant.**
   - Examiner l’impact Il s'agit de la dernière étape du workflow et elle est obligatoire.

## Mettre en place la classification des données en important les étiquettes de sensibilité de Microsoft Purview

### Prérequis

- Assurez-vous que vous disposez des rôles ou privilèges nécessaires pour travailler avec les étiquettes de sensibilité dans Microsoft Purview.
- Vous devez connaître les détails des niveaux de classification des tableaux que vous souhaitez configurer en fonction de vos exigences en matière de sécurité et de gouvernance.
- Vous devez avoir le [rôle d'administrateur de contenu sensible.](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md) Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.

:::note
Notes :
- Selon la documentation de Microsoft, les mises à jour des étiquettes de sensibilité dans Microsoft Purview peuvent prendre jusqu'à 24 heures pour être répliquées dans toutes les applications et tous les services. Veuillez laisser suffisamment de temps pour que les changements soient effectués et importez ensuite les étiquettes de sensibilité. Si les mises à jour que vous avez effectuées dans MS Purview ne sont pas répliquées après 24 heures, veuillez contacter l'équipe d'assistance Microsoft Purview.
- Vous pouvez importer dans Miro jusqu'à 50 étiquettes de sensibilité provenant de Microsoft Purview.
- Si vous disposez déjà d'une configuration de classification des données, vous pouvez importer des étiquettes de sensibilité depuis Microsoft Purview et transférer les étiquettes de classification existantes dans Miro. Pour plus d'informations, voir [Importer des étiquettes de sensibilité de Microsoft Purview dans la configuration existante de la classification des données dans Miro](08-import-microsoft-purview-sensitivity-labels.md).
:::

Pour importer des étiquettes de sensibilité à partir de Microsoft purview et configurer la classification des données dans Miro, procédez comme suit :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **Classification des données**.
3. Sur la page **Classification** , en bas de l'écran, cliquez sur **Commencer**.
4. Dans la boîte **Importer à partir de Microsoft Purview**, cliquez sur **Se connecter.**
5. Sur la page **Microsoft Sign in** qui s'affiche dans un nouvel onglet, entrez vos identifiants Microsoft et connectez-vous. Une fois que vous êtes connecté à votre compte Microsoft, l'onglet est automatiquement fermé,
6. Sur la page **Classification** , dans la boîte **Importer de Microsoft Purview**, cliquez sur **Importer**.
   La page **Importer la classification de Microsoft Purview** s'affiche.
7. Cochez la case des étiquettes de sensibilité Microsoft Purview que vous souhaitez utiliser comme niveaux de classification dans Miro, puis cliquez sur **Suivant.**
   > ✏️ Selon la documentation de Microsoft, les mises à jour des étiquettes de sensibilité dans Microsoft Purview peuvent prendre jusqu'à 24 heures pour être répliquées dans toutes les applications et tous les services. Veuillez laisser suffisamment de temps pour que les changements soient effectués et importez ensuite les étiquettes de sensibilité. Si les mises à jour que vous avez effectuées dans MS Purview ne sont pas répliquées après 24 heures, veuillez contacter l'équipe d'assistance Microsoft Purview.
8. Sur la page **Définir les niveaux de classification**, vous pouvez modifier les niveaux de classification pour attribuer le niveau de classification par défaut ou ajouter un lien vers les lignes directrices. Le tableau suivant présente chaque champ et sa description.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Lien vers les lignes directrices** | URL qui fournit plus d'informations sur les politiques ou les instructions applicables à ce niveau de classification. Il peut s'agir d'une page qui fournit davantage d'informations aux utilisateurs de votre organisation afin qu'ils en sachent plus sur les niveaux de classification de votre tableau et sur la manière de travailler avec eux. Vous devez fournir l'URL dans le format suivant : `http://www.example.com`  Lorsque l'utilisateur clique sur l'icône " **En savoir plus"** (point d'interrogation) à côté du badge de classification du tableau, cette URL est chargée dans un nouvel onglet du navigateur. |
   | **Utilisé comme niveau par défaut pour les nouveaux tableaux** | Cochez cette case pour définir ce niveau de classification comme classification par défaut pour tous les nouveaux tableaux. |
   | **Aperçu** | Affiche un aperçu du badge de classification du tableau avec sa description et l'icône pour en savoir plus. L'aperçu montre exactement comment l'insigne de classification apparaît aux utilisateurs d'un tableau. |

   Pour enregistrer la configuration du niveau de classification, cliquez sur **Terminé**.
9. Cliquez sur **Suivant**. Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. [**Examiner l'impact**](https://help.miro.com/hc/articles/16494764223378) sur la page Examiner l'impact.

   Vous pouvez ensuite passer à l'une des étapes suivantes :

   - Définir la classification automatique Cette option est facultative. Si vous souhaitez définir la classification automatique ultérieurement, cliquez sur **Suivant.**
   - Définir les garde-fous Cette option est facultative. Si vous souhaitez définir les garde-fous ultérieurement, cliquez sur **Suivant.**
   - Examiner l’impact Il s'agit de la dernière étape du workflow et elle est obligatoire.

## Mise à jour du niveau de classification par défaut pour les nouveaux tableaux

Vous pouvez mettre à jour le niveau de classification par défaut en procédant comme suit :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **Classification des données**.
3. Cliquez sur **Modifier les niveaux de classification** en haut à droite de l'écran.
4. Sur la page **Définir les niveaux de classification**, cliquez sur **Modifier les niveaux de classification**.
5. Cliquez sur l' icône **Modifier** (![Screenshot 2024-01-22 at 23.20.18.png](images/21017417813906_Screenshot%202024-01-22%20at%2023.20.18.png)) pour le niveau que vous souhaitez définir comme niveau de classification par défaut.
6. Cochez la case **Utiliser comme niveau par défaut pour les nouveaux tableaux**.
7. Cliquez sur **Done** (Terminé).
   Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. [**Examiner l'impact**](https://help.miro.com/hc/articles/16494764223378) sur la page Examiner l'impact.
8. Cliquez sur **Suivant**. Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. [**Examiner l'impact**](https://help.miro.com/hc/articles/16494764223378) sur la page Examiner l'impact.

   Vous pouvez ensuite passer à l'une des étapes suivantes :

   - Définir la classification automatique Cette option est facultative. Si vous souhaitez définir la classification automatique ultérieurement, cliquez sur **Suivant.**
   - Définir les garde-fous Cette option est facultative. Si vous souhaitez définir les garde-fous ultérieurement, cliquez sur **Suivant.**
   - Examiner l’impact Il s'agit de la dernière étape du workflow et elle est obligatoire.

## Mettre à jour l'ordre de sensibilité d'un niveau de classification

Vous pouvez mettre à jour l'ordre de sensibilité d'un niveau de classification en procédant comme suit :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **Classification des données**.
3. Cliquez sur **Modifier les niveaux de classification** en haut à droite de l'écran.
4. Sur la page **Définir les niveaux de classification**, cliquez sur **Modifier les niveaux de classification**.
5. Les niveaux de classification apparaissent avec leur ordre de sensibilité actuel. Cliquez sur les flèches vers le haut ou vers le bas correspondant aux niveaux de classification pour lesquels vous souhaitez mettre à jour l'ordre de sensibilité.

   > ✏️ Actuellement, l'ordre de sensibilité **1** indique le niveau de classification **le moins sensible.**

   Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. **[Examiner l'impact](https://help.miro.com/hc/articles/16494764223378)** sur la page Examiner l'impact.
6. Cliquez sur **Suivant**. Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. [**Examiner l'impact**](https://help.miro.com/hc/articles/16494764223378) sur la page Examiner l'impact.

   Vous pouvez ensuite passer à l'une des étapes suivantes :

   - Définir la classification automatique Cette option est facultative. Si vous souhaitez définir la classification automatique ultérieurement, cliquez sur **Suivant.**
   - Définir les garde-fous Cette option est facultative. Si vous souhaitez définir les garde-fous ultérieurement, cliquez sur **Suivant.**
   - Examiner l’impact Il s'agit de la dernière étape du workflow et elle est obligatoire.

## Supprimer un niveau de classification

:::note
Vous ne pouvez pas supprimer un niveau de classification s'il est associé à une [politique de conservation](https://help.miro.com/hc/sections/19180529348754).
:::

Vous pouvez supprimer un niveau de classification en procédant comme suit :

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **Classification des données**.
3. Cliquez sur **Modifier les niveaux de classification** en haut à droite de l'écran.
4. Sur la page **Définir les niveaux de classification**, cliquez sur **Modifier les niveaux de classification**.
5. Cliquez sur l'icône de suppression du niveau de classification que vous souhaitez supprimer.
6. Si le niveau de classification que vous souhaitez supprimer a déjà été appliqué à un ou plusieurs tableaux, une fenêtre de notification s'affiche pour vous informer du nombre de tableaux auxquels le niveau de classification a été appliqué.
   Sélectionnez le nouveau niveau de classification que vous souhaitez appliquer aux tableaux concernés.
7. Cliquez sur **Done** (Terminé).
   Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. [**Examiner l'impact**](https://help.miro.com/hc/articles/16494764223378) sur la page Examiner l'impact.
8. Cliquez sur **Suivant**. Votre configuration est sauvegardée, mais elle ne prendra effet que lorsque vous aurez cliqué sur **Publier** dans la fenêtre d'impact de l'examen. [**Examiner l'impact**](https://help.miro.com/hc/articles/16494764223378) sur la page Examiner l'impact.

   Vous pouvez ensuite passer à l'une des étapes suivantes :

   - Définir la classification automatique Cette option est facultative. Si vous souhaitez définir la classification automatique ultérieurement, cliquez sur **Suivant.**
   - Définir les garde-fous Cette option est facultative. Si vous souhaitez définir les garde-fous ultérieurement, cliquez sur **Suivant.**
   - Examiner l’impact Il s'agit de la dernière étape du workflow et elle est obligatoire.
