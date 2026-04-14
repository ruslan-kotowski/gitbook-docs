---
title: "Cr\xE9er des badges et des mots-cl\xE9s pour les informations sensibles de\
  \ l\u2019entreprise"
article_id: 21626517022610
translation_id: 21626517022610
locale: fr
sidebar_position: 11
created_at: '2024-09-26T21:36:45Z'
updated_at: '2026-03-04T22:59:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

Créez des badges pour définir des conditions, comme des mots-clés ou des widgets, que vous souhaitez identifier et localiser sur les tableaux Miro. Vous pouvez créer jusqu'à 100 badges sensibles de l'entreprise. Pour créer un badge, procédez comme suit :

:::note
Pour créer des badges personnalisés, vous devez avoir le rôle [d’admin de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.
:::

1. Accédez à vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard**, cliquez sur **Découverte de données**.
3. Sur la page **Découverte de données**, cliquez sur l'onglet **Configuration**.
4. Dans la section **Sensible de l’entreprise**, cliquez sur le bouton **Créer**.
5. Sur la page **Définir un badge personnalisé**, ajoutez les détails du badge.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Nom du badge** | **Longueur maximale :** 80 caractères  Nom descriptif pour le badge personnalisé. Vous pouvez utiliser un nom de projet interne à l'entreprise, car ce badge n'apparaît pas dans les journaux.  **Remarque :** Le nom du badge n'est pas visible dans les journaux d'audit. Si vous souhaitez consulter/rechercher les journaux d’audit associés à ce badge, vous pouvez utiliser l'identifiant du badge. |
   | **Nom court** | **Longueur maximale :** 10 caractères, alphanumérique  Version abrégée du nom du badge. Le nom court est utilisé pour faire référence à ce badge personnalisé dans la découverte de données, l'explorateur de contenu et la classification. **Remarque :** Le nom court n'est pas visible dans les journaux d’audit. Si vous souhaitez consulter ou rechercher les journaux d’audit associés à ce badge, vous pouvez utiliser l’identifiant du badge. |
   | **Description** | **Longueur maximale :** 500 caractères  Description des informations que ce badge détecte. Ces informations sont utiles pour les autres admins. |
   | **Conditions** | Ajoutez des mots-clés et des types de widget que vous souhaitez détecter et auxquels vous souhaitez ajouter ce badge lors de la détection sur un tableau Miro. Vous devez ajouter au moins une condition.  Si vous ajoutez uniquement des mots-clés et ne sélectionnez aucune case de widget, la découverte de données détecte tous les tableaux contenant des correspondances exactes des mots-clés que vous avez fournis pour tous les widgets pris en charge. La version actuelle prend en charge les éléments suivants pour la détection de mots-clés : Notes adhésives, carte, carte Jira, bloc de code, commentaires, cadre, table, connecteur/ligne, forme, bloc de texte, tableau Kanban, carte utilisateur.  Vous pouvez également choisir de détecter uniquement les blocs de code, les cartes Jira, les cartes Azure ou les écrans de prototypage, sans ajouter de mots-clés. La découverte de données détecte alors tous les tableaux contenant ces widgets.  Si vous ajoutez à la fois des mots-clés et des widgets comme conditions, les critères de mot-clé et de widget doivent être remplis pour que la découverte de données détecte le tableau. Cela vous permet d'affiner votre recherche et de cibler les tableaux plus précisément à l'aide de badges personnalisés.  **Exemples :**  - Si vous souhaitez restreindre la détection des tableaux pour repérer exclusivement ceux liés au développement de produits et non au marketing, et que le tableau doit contenir le nom du projet *Enterprise* *Guard*, et si vous souhaitez ne trouver que les tableaux qui contiennent également une carte Jira (car elle est liée au développement de produits), vous configurerez ce badge pour inclure le mot-clé *Enterprise* *Guard* et sélectionnerez la case à cocher carte Jira. La découverte de données trouve alors les tableaux contenant le mot-clé Enterprise Guard et une carte Jira. La découverte de données trouve également les tableaux qui contiennent des cartes Jira avec le mot-clé Enterprise Guard dans leur titre ou description. Si un tableau contient uniquement le mot-clé *Enterprise* *Guard* mais ne contient pas de carte Jira, le tableau n'est pas détecté car il ne remplit pas les deux conditions spécifiées.  - Si vous souhaitez détecter tous les tableaux contenant le mot *Enterprise* *Guard* pour tous les types de widgets pris en charge, indépendamment des widgets que le tableau contient, dans la section **Ajouter des mots-clés**, ajoutez le mot-clé **Enterprise** **Guard**. Vous n'avez pas besoin d'ajouter de type de widget pour cet exemple.  - Si vous souhaitez détecter tous les tableaux avec des cartes Jira, quel que soit le contenu spécifique, dans la section **Ajouter un type de widget**, cochez la case **Carte Jira**. Vous n'avez pas besoin d'ajouter de mot-clé pour cet exemple.    **Pour ajouter un mot-clé :**  1. Cliquez sur **Ajouter des mots-clés**.  2. Entrez ou collez des mots-clés séparés par des virgules. **Remarques :**  - Les mots-clés prennent en charge les caractères alphanumériques et Unicode. - Vous pouvez ajouter jusqu'à 100 mots-clés ou expressions. - Les espaces avant et après sont ignorés dans les mots-clés. - La découverte de données détecte les correspondances exactes pour les mots-clés que vous fournissez, sans tenir compte de la casse. - Si vous ajoutez un espace avant un mot-clé, la découverte de données trouve également les correspondances exactes qui ont un espace avant ce mot-clé. - La version actuelle prend en charge les éléments de tableau suivants pour la détection de mots-clés : Post-it, Carte, Carte Jira, Bloc de code, Cadre, Table, Connecteur/ligne, Forme, Bloc de texte, Tableau Kanban, Carte de récit utilisateur. Les notes et commentaires ne sont actuellement pas inclus dans les analyses de découverte de données. Nous travaillons à inclure les notes et commentaires dans les prochaines versions d'amélioration des fonctionnalités.  **Exemple :** Pour identifier et étiqueter les tableaux contenant les mots-clés *confidentiel* ou *interne*, ajoutez les mots-clés suivants : *confidentiel, interne* (utilisez une virgule pour séparer chaque mot-clé). La découverte de données trouve alors tous les tableaux incluant l'un de ces mots-clés.  **Pour ajouter un type de widget :**  1. Cliquez sur **Ajouter un type de widget**.  2. Cochez la case du type de widget que vous souhaitez détecter sur les tableaux Miro.  **Exemple :** Si vous souhaitez détecter et étiqueter les tableaux contenant une carte Jira, cochez la case **Carte Jira**. |
6. Cliquez sur **Suivant**.
7. Passez en revue les détails du badge personnalisé.

   Si vous souhaitez modifier les détails du badge personnalisé, cliquez sur le bouton **Précédent**.

   Si les détails du badge personnalisé sont corrects, cliquez sur le bouton **Créer un badge personnalisé**.

   Après la création du badge, la première analyse débute automatiquement. Les résultats correspondant aux conditions sélectionnées seront disponibles après quelques minutes ou heures, selon le nombre de tableaux Miro dans votre organisation.
