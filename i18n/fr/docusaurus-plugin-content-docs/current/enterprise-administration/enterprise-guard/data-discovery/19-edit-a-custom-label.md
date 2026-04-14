---
title: "Modifier un badge personnalis\xE9"
article_id: 21690361870354
translation_id: 21690361870354
locale: fr
sidebar_position: 18
created_at: '2024-09-30T13:43:27Z'
updated_at: '2026-03-04T23:02:00Z'
draft: false
outdated: false
user_segment_id: null
user_segment: Everyone
---

:::note
Nous recommandons de modifier les badges uniquement avant d'associer le badge avec un niveau de classification.
:::

Modifiez les badges pour mettre à jour les conditions, comme les mots-clés ou les widgets, que vous souhaitez identifier et localiser sur les tableaux Miro. Pour modifier un badge, procédez comme suit :

:::note
Pour modifier les badges personnalisés, vous devez avoir le rôle d’[admin de contenu sensible](../../enterprise-subscription-management/enterprise-guard-overview/03-understand-admin-roles-and-their-privileges.md). Pour demander le rôle d’admin du contenu sensible, contactez l’admin de votre entreprise.
:::

1. Allez dans vos [paramètres Miro](https://miro.com/app/settings).
2. Dans le volet de gauche, sous **Enterprise Guard,** cliquez sur **Découverte de données**.
3. Sur la page **Aperçu** de la **Découverte de données**, cliquez sur les trois points à la fin de la ligne du badge que vous souhaitez modifier, puis cliquez sur **Modifier le badge**.
4. Sur la page **Modifier le badge personnalisé**, modifiez les détails du badge.

   |  |  |
   | --- | --- |
   | **Champ** | **Description** |
   | **Nom du badge** | **Longueur maximale :** 80 caractères  Nom descriptif pour le badge personnalisé. Vous pouvez utiliser un nom de projet interne à l'entreprise car ce badge n'apparaît pas dans les journaux.  **Remarque :** Le nom du badge n'est pas visible dans les journaux d'audit. Si vous souhaitez consulter les journaux d’audit associés à ce badge, vous pouvez utiliser l’identifiant du badge. |
   | **Nom court** | **Longueur maximale :** 10 caractères, alphanumérique  Version courte du nom du badge. Le nom court est utilisé pour faire référence à ce badge personnalisé dans la découverte de données et l’explorateur de contenu. **Remarque :** Le nom court n’est pas visible dans les journaux d’audit. Si vous souhaitez consulter ou rechercher les journaux d'audit associés à ce badge, vous pouvez utiliser l’identifiant du badge. |
   | **Description** | **Longueur maximale :** 500 caractères  Description des informations que ce badge détecte. Cette information est utile pour les autres admins. |
   | **Conditions** | Ajoutez des mots-clés et des types de widgets que vous souhaitez détecter et associer à ce badge lors de leur détection sur un tableau Miro. Vous devez ajouter au moins une condition.  Si vous ajoutez uniquement des mots-clés et ne sélectionnez aucune case de widget, la découverte de données détecte tous les tableaux contenant des correspondances exactes des mots-clés que vous avez fournis pour tous les widgets pris en charge. La version actuelle prend en charge les éléments de tableau suivants pour la détection de mots-clés : Sticky, Carte, Carte Jira, Bloc de code, Commentaires, Cadre, Table, Connecteur/ligne, Forme, Bloc de texte, Tableau Kanban, User story map.  Vous pouvez également choisir de détecter uniquement les blocs de code, cartes Jira, cartes Azure, ou les écrans de prototypage, sans ajouter de mots-clés. La découverte de données détecte alors tous les tableaux contenant ces widgets.  Si vous ajoutez à la fois des mots-clés et des widgets comme conditions, les critères de mots-clés et de widgets doivent être satisfaits pour que la découverte de données détecte le tableau. Cela vous permet d'affiner votre recherche et de cibler plus précisément les tableaux à l'aide de badges personnalisés.  **Exemples :**  - Si vous souhaitez restreindre la détection aux tableaux spécifiquement liés au développement de produits, mais pas aux tableaux liés au marketing, et que le tableau doit contenir le nom du projet *Enterprise* *Guard*, et que vous souhaitez trouver uniquement les tableaux qui contiennent également une carte Jira (car elle est liée au développement de produits), vous configurerez ce badge pour contenir le mot-clé *Enterprise* *Guard* et sélectionnerez la case carte Jira. La découverte de données trouvera ainsi les tableaux qui contiennent le mot-clé Enterprise Guard et une carte Jira. La découverte de données trouvera également les tableaux qui contiennent des cartes Jira avec le mot-clé Enterprise Guard dans leur titre ou description. Si un tableau contient uniquement le mot-clé *Enterprise* *Guard* mais ne contient pas de carte Jira, le tableau ne sera pas détecté car il ne remplit pas les deux conditions spécifiées.  - Si vous souhaitez détecter tous les tableaux contenant le mot *Enterprise* *Guard* pour tous les types de widgets pris en charge, quel que soit le type de widget que le tableau contient, dans la section **Ajouter des mots-clés**, ajoutez le mot-clé **Enterprise** **Guard**. Vous n’avez pas besoin d’ajouter de type de widget pour cet exemple.  - Si vous souhaitez détecter tous les tableaux avec des cartes Jira quel que soit le contenu spécifique, dans la section **Ajouter un type de widget**, sélectionnez la case à cocher **Carte Jira**. Vous n’avez pas besoin d’ajouter de mot-clé pour cet exemple.    **Pour ajouter un mot-clé :**  1. Cliquez sur **Ajouter des mots-clés**.  2. Entrez ou collez des mots-clés séparés par des virgules. **Remarques :**  - Les mots-clés prennent en charge les caractères alphanumériques et Unicode.  - Vous pouvez ajouter jusqu'à 100 mots-clés ou expressions. - La découverte de données détecte les correspondances exactes pour les mots-clés que vous fournissez, sans tenir compte de la sensibilité des majuscules ou minuscules. - La version actuelle prend en charge les éléments de tableau suivants pour la détection de mots-clés : pense-bête, carte, carte Jira, bloc de code, cadre, table, connecteur/ligne, forme, bloc de texte, tableau Kanban, carte d'histoire utilisateur. Actuellement, les notes et commentaires ne sont pas inclus dans les analyses de découverte de données. Nous travaillons à inclure les notes et commentaires dans les prochaines améliorations des fonctionnalités.  **Exemple :** Pour identifier et marquer les tableaux contenant les mots-clés *confidentiel* ou *interne*, ajoutez les mots-clés suivants : *confidentiel, interne* (utilisez une virgule pour séparer chaque mot-clé). La découverte de données trouve alors tous les tableaux qui incluent l'un ou l'autre de ces mots-clés.  **Pour ajouter un type de widget :**  1. Cliquez sur **Ajouter un type de widget**.  2. Sélectionnez la case à cocher pour le type de widget que vous souhaitez détecter sur les tableaux Miro.  **Exemple :** Si vous souhaitez détecter et étiqueter les tableaux qui contiennent une carte Jira, sélectionnez la case **Jira card**. |
5. Cliquez sur **Suivant**.
6. Passez en revue les détails du badge personnalisé.

   Si vous souhaitez mettre à jour les détails du badge personnalisé, cliquez sur le bouton **Précédent**.

   Si les détails du badge personnalisé sont corrects, cliquez sur le bouton **Mettre à jour le badge personnalisé**.

   Après avoir mis à jour le badge personnalisé, le scan commence automatiquement. Les résultats correspondant aux conditions sélectionnées seront disponibles après quelques minutes ou heures, selon le nombre de tableaux Miro dans votre organisation.
